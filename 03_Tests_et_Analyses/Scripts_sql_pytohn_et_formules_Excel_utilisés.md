📁 04_Exemples_Scripts
│
├── 01_SQL_Examples.md
│     └── Contenu :
│
│     # 01 – Exemples de requêtes SQL
│
│     ## 1. Détection de doublons de sinistres
│     ```sql
│     SELECT 
│         numero_contrat,
│         date_sinistre,
│         type_sinistre,
│         COUNT(*) AS nb_doublons
│     FROM Sinistre
│     GROUP BY numero_contrat, date_sinistre, type_sinistre
│     HAVING COUNT(*) > 1;
│     ```
│
│     ## 2. Dates incohérentes
│     ```sql
│     SELECT *
│     FROM Sinistre
│     WHERE date_declaration < date_sinistre
│        OR date_cloture < date_declaration;
│     ```
│
│     ## 3. Paiements sans sinistre associé
│     ```sql
│     SELECT p.*
│     FROM Paiement p
│     LEFT JOIN Sinistre s ON p.id_sinistre = s.id
│     WHERE s.id IS NULL;
│     ```
│
│
├── 02_Excel_Examples.md (PS: A2 = date sinistre, B2 = date déclaration)
│     └── Contenu :
│
│     # 02 – Exemples d’analyses Excel
│
│     ## 1. Détection des valeurs extrêmes (outliers)
│     ```excel
│     =SI(ABS(A2 - MOYENNE($A$2:$A$500)) > 3 * ECARTYPE($A$2:$A$500); "Outlier"; "")
│     ```
│
│     ## 2. Vérification des doublons
│     ```excel
│     =NB.SI($A$2:$A$500; A2) > 1
│     ```
│
│     ## 3. Contrôle de cohérence des dates
│     ```excel
│     =SI(B2 < A2; "Erreur"; "")
│     ```
│
│
└── 03_Python_Examples.md
      └── Contenu :
      
      # 03 – Exemples de scripts Python

      ## 1. Détection de dérive du modèle IA
      ```python
      import pandas as pd

      baseline = pd.read_csv("baseline_scores.csv")
      current = pd.read_csv("current_scores.csv")

      drift = abs(current["score"].mean() - baseline["score"].mean())

      if drift > 0.05:
          print("Risque de dérive détecté")
      else:
          print("Modèle stable")
      ```

      ## 2. Analyse des logs pour détecter des accès suspects
      ```python
      import pandas as pd

      logs = pd.read_csv("logs.csv")

      suspicious = logs[logs["heure"].str.contains("23:|00:|01:")]

      print(suspicious)
      ```


5_Exemples_règles_de_validation_métier:
 5.1 Montant d’indemnisation
Montant > 0

Montant ≤ plafond du contrat

Montant ≤ montant déclaré

 5.2 Dates
Date sinistre ≤ date déclaration

Date clôture ≥ date déclaration

Paiement après validation
