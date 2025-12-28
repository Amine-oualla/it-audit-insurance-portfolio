# 01 – Fiches d’analyse

## 1. Introduction

Les fiches d’analyse synthétisent les résultats des tests réalisés dans le cadre de la mission d’audit IT.  
Elles permettent de documenter :

- les constats observés  
- les risques associés  
- les causes probables  
- les impacts potentiels  
- les recommandations proposées  
- la criticité du constat  

Chaque fiche constitue une preuve structurée et exploitable pour le rapport final.

---

## 2. Fiche d’analyse – Habilitations et accès

### 🔹 Constat
Plusieurs comptes utilisateurs disposent d’habilitations supérieures à leurs besoins opérationnels (droits transverses, accès non justifiés).

### 🔹 Risque
Accès non autorisé à des données sensibles, violation RGPD, fraude interne.

### 🔹 Cause
Absence de revue périodique des habilitations, manque de séparation des tâches.

### 🔹 Impact
Exposition accrue aux risques de fuite de données et d’erreurs critiques.

### 🔹 Recommandation
Mettre en place une revue trimestrielle des habilitations et appliquer strictement le principe du moindre privilège.

### 🔹 Criticité
Élevée

---

## 3. Fiche d’analyse – Logs et traçabilité

### 🔹 Constat
Les journaux applicatifs ne tracent pas l’ensemble des actions sensibles (modifications de données, accès privilégiés).

### 🔹 Risque
Impossibilité de reconstituer un incident ou une fraude.

### 🔹 Cause
Configuration incomplète des logs, absence de supervision.

### 🔹 Impact
Détection tardive d’incidents, non‑conformité réglementaire.

### 🔹 Recommandation
Activer la journalisation complète des actions critiques et intégrer les logs au SOC.

### 🔹 Criticité
Élevée

---

## 4. Fiche d’analyse – Qualité des données sinistres

### 🔹 Constat
Présence d’incohérences (dates incorrectes, doublons, montants atypiques).

### 🔹 Risque
Décisions erronées, fraude non détectée, reporting faussé.

### 🔹 Cause
Absence de règles de validation robustes, erreurs de saisie.

### 🔹 Impact
Perte financière, mauvaise expérience client, non‑conformité.

### 🔹 Recommandation
Renforcer les contrôles automatiques et mettre en place un monitoring de la qualité des données.

### 🔹 Criticité
Moyenne à élevée

---

## 5. Fiche d’analyse – Modèle IA de détection de fraude

### 🔹 Constat
Absence de documentation complète et de suivi de performance du modèle IA.

### 🔹 Risque
Dérive du modèle, augmentation des faux négatifs, biais algorithmique.

### 🔹 Cause
Manque de gouvernance IA, absence de versioning formel.

### 🔹 Impact
Fraude non détectée, décisions injustes, non‑conformité ACPR.

### 🔹 Recommandation
Mettre en place un processus de gouvernance IA incluant versioning, supervision humaine et suivi des métriques.

### 🔹 Criticité
Élevée

---

## 6. Fiche d’analyse – Continuité d’activité

### 🔹 Constat
Le PRA existe mais n’a pas été testé depuis plus de 18 mois.

### 🔹 Risque
Indisponibilité prolongée du système sinistres en cas d’incident majeur.

### 🔹 Cause
Manque de coordination entre IT et métiers.

### 🔹 Impact
Arrêt de l’activité, perte financière, atteinte à la réputation.

### 🔹 Recommandation
Planifier un test PRA annuel et documenter les résultats.

### 🔹 Criticité
Moyenne

---

## 7. Conclusion

Les fiches d’analyse permettent de structurer les constats et d’alimenter directement le rapport final.  
Elles constituent la base des recommandations et du plan d’action à suivre par les équipes IT, Sécurité, Data et Métier.


