# 02 – Rapport d’audit IT – Système de gestion des sinistres

## 1. Introduction

Ce rapport présente les résultats de la mission d’audit IT portant sur le système de gestion des sinistres de la compagnie d’assurance.  
L’objectif de la mission est d’évaluer :

- la sécurité du système  
- la qualité et l’intégrité des données  
- la gouvernance IT et IA  
- la robustesse des processus  
- la continuité d’activité  

Le rapport s’appuie sur :

- le diagnostic initial  
- la cartographie des risques  
- le plan de travail validé  
- les tests techniques et analyses de données  
- les entretiens avec les équipes IT, Sécurité, Data et Métiers  

---

## 2. Synthèse exécutive

L’audit met en évidence un niveau global de maîtrise **partiel**, avec plusieurs points forts mais aussi des risques significatifs nécessitant des actions prioritaires.

### 🔹 Points forts observés
- Architecture applicative globalement stable  
- Collaboration efficace entre équipes IT et métiers  
- Existence d’un PRA documenté  
- Modèle IA performant sur les cas standards  

### 🔹 Points de vigilance majeurs
- Habilitations excessives et absence de revue périodique  
- Traçabilité incomplète des actions sensibles  
- Incohérences dans les données sinistres  
- Gouvernance IA insuffisante  
- PRA non testé récemment  

### 🔹 Conclusion générale
Le système est fonctionnel et relativement mature, mais plusieurs faiblesses exposent l’organisation à des risques opérationnels, réglementaires et de fraude.  
Des actions correctives prioritaires sont recommandées.

---

## 3. Périmètre de l’audit

L’audit couvre :

- le système de gestion des sinistres (application principale)  
- les bases de données associées  
- les processus IT (incidents, changements, accès, sauvegardes)  
- les modèles IA de détection de fraude  
- les environnements (Prod / Préprod / Dev)  
- le PRA / PCA  

Ne sont pas inclus :

- les applications hors périmètre sinistres  
- les processus métiers non liés au traitement des sinistres  

---

## 4. Méthodologie

La mission a été réalisée selon les standards :

- ITGC (IT General Controls)  
- ISO 27001  
- RGPD  
- ACPR – Gouvernance des algorithmes  
- Bonnes pratiques d’audit interne (IIA)  

Les travaux incluent :

- revue documentaire  
- tests techniques IT  
- analyses de données (SQL, Excel, Python)  
- entretiens avec les équipes  
- revue des logs et configurations  
- analyse des performances du modèle IA  

---

## 5. Résultats détaillés de l’audit

### 5.1 Gestion des habilitations – **Criticité : Élevée**

**Constat :**  
Des utilisateurs disposent d’habilitations supérieures à leurs besoins, et aucune revue périodique n’est réalisée.

**Risques :**  
Accès non autorisé, fraude interne, violation RGPD.

**Recommandations :**  
- Mettre en place une revue trimestrielle des accès  
- Appliquer le principe du moindre privilège  
- Supprimer les comptes inactifs  

---

### 5.2 Traçabilité et logs – **Criticité : Élevée**

**Constat :**  
Les actions sensibles ne sont pas toutes tracées (modifications, accès privilégiés).

**Risques :**  
Impossibilité d’investigation, non‑conformité, détection tardive d’incidents.

**Recommandations :**  
- Activer la journalisation complète  
- Intégrer les logs au SOC  
- Définir une politique de rétention  

---

### 5.3 Qualité des données – **Criticité : Moyenne à Élevée**

**Constat :**  
Présence d’incohérences : dates incorrectes, doublons, montants atypiques.

**Risques :**  
Décisions erronées, fraude non détectée, reporting faussé.

**Recommandations :**  
- Renforcer les règles de validation  
- Mettre en place un monitoring qualité  
- Automatiser la détection des doublons  

---

### 5.4 Gouvernance IA – **Criticité : Élevée**

**Constat :**  
Le modèle IA manque de documentation, de versioning et de suivi de performance.

**Risques :**  
Dérive du modèle, biais, augmentation des faux négatifs.

**Recommandations :**  
- Documenter le modèle (données, versions, métriques)  
- Mettre en place un suivi mensuel  
- Assurer une supervision humaine systématique  

---

### 5.5 Continuité d’activité – **Criticité : Moyenne**

**Constat :**  
Le PRA existe mais n’a pas été testé depuis plus de 18 mois.

**Risques :**  
Indisponibilité prolongée en cas d’incident majeur.

**Recommandations :**  
- Planifier un test annuel  
- Documenter les résultats  
- Vérifier les dépendances critiques  

---

## 6. Conclusion générale

Le système de gestion des sinistres présente une base solide, mais plusieurs faiblesses doivent être corrigées rapidement pour garantir :

- la sécurité des données  
- la conformité réglementaire  
- la performance du modèle IA  
- la continuité d’activité  
- la fiabilité du traitement des sinistres  

Les recommandations proposées constituent un plan d’action réaliste et priorisé permettant d’améliorer significativement la maîtrise des risques IT.

---

## 7. Annexes (pour plus de détails voire le chapitre 06_Annexes)

- Synthèse des tests réalisés  
- Exemples de scripts SQL / Python  
- Extraits de logs anonymisés  
- Cartographie des risques  
- Matrice de criticité  

