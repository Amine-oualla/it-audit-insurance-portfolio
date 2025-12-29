# 02 – Concepts clés en Audit IT, Cybersécurité, Data et IA

## 1. Introduction

Cette annexe présente les concepts fondamentaux utilisés dans l’audit IT, la cybersécurité, la gestion des données et l’audit des modèles d’intelligence artificielle.  
Elle permet de comprendre les notions mobilisées dans les tests, analyses et recommandations du rapport d’audit.

---

# 2. Concepts d’Audit IT

## 🔹 2.1 ITGC – IT General Controls
Les contrôles généraux IT couvrent les fondations de la maîtrise informatique :
- gestion des accès  
- gestion des changements  
- gestion des sauvegardes  
- sécurité des environnements  
- continuité d’activité  
- gestion des incidents  

Ils garantissent la fiabilité des systèmes et des données.

---

## 🔹 2.2 Gestion des habilitations
Processus permettant de contrôler **qui a accès à quoi** :
- principe du moindre privilège  
- séparation des tâches  
- revue périodique des accès  
- suppression des comptes inactifs  
- traçabilité des actions  

---

## 🔹 2.3 Journalisation et traçabilité
Capacité à enregistrer les actions sensibles :
- accès aux données  
- modifications  
- actions administrateur  
- anomalies ou comportements suspects  

Indispensable pour la détection d’incidents et la conformité RGPD / ISO 27001.

---

## 🔹 2.4 Gestion des changements (Change Management)
Processus garantissant que les évolutions applicatives sont :
- validées  
- testées  
- documentées  
- déployées de manière contrôlée  

Réduit les risques d’incidents en production.

---

## 🔹 2.5 Continuité d’activité (PRA / PCA)
- **PRA** : reprise après sinistre (disaster recovery)  
- **PCA** : continuité des opérations  

Objectif : assurer la disponibilité du système en cas d’incident majeur.

---

# 3. Concepts Data & Qualité des données

## 🔹 3.1 Dimensions de la qualité des données
- **Exactitude** : données correctes  
- **Complétude** : données non manquantes  
- **Cohérence** : absence de contradictions  
- **Unicité** : pas de doublons  
- **Traçabilité** : origine et transformations connues  

---

## 🔹 3.2 Règles de validation
Contrôles automatiques appliqués aux données :
- formats  
- dates  
- montants  
- champs obligatoires  
- relations entre tables  

---

## 🔹 3.3 Monitoring de la qualité des données
Suivi continu via :
- dashboards  
- alertes  
- indicateurs (KPI)  
- scripts SQL / Python  

---

# 4. Concepts Cybersécurité

## 🔹 4.1 Confidentialité, Intégrité, Disponibilité (CIA)
Les trois piliers de la sécurité :
- **Confidentialité** : accès réservé aux personnes autorisées  
- **Intégrité** : données non altérées  
- **Disponibilité** : système accessible quand nécessaire  

---

## 🔹 4.2 Gestion des incidents
Processus structuré :
- détection  
- analyse  
- containment  
- résolution  
- post-mortem  

---

## 🔹 4.3 Vulnérabilités et menaces
- vulnérabilité = faiblesse  
- menace = événement pouvant exploiter la faiblesse  
- risque = menace × vulnérabilité × impact  

---

# 5. Concepts IA & Gouvernance des modèles

## 🔹 5.1 Cycle de vie d’un modèle IA
- collecte des données  
- préparation  
- entraînement  
- validation  
- déploiement  
- suivi de performance  
- recalibrage  

---

## 🔹 5.2 Dérive du modèle (Model Drift)
Perte de performance due à :
- changement des données  
- évolution des comportements  
- biais non détectés  

Nécessite un suivi régulier.

---

## 🔹 5.3 Biais algorithmiques
Types de biais :
- biais de données  
- biais de conception  
- biais d’interprétation  

Impact : décisions injustes ou discriminatoires.

---

## 🔹 5.4 Supervision humaine
Exigence ACPR :
- validation humaine des décisions sensibles  
- documentation des arbitrages  
- traçabilité des corrections  

---

## 🔹 5.5 Versioning des modèles
Permet de suivre :
- versions du modèle  
- données d’entraînement  
- hyperparamètres  
- métriques de performance  

Indispensable pour la conformité et l’auditabilité.

---

# 6. Concepts réglementaires

## 🔹 6.1 RGPD
Principes clés :
- minimisation  
- sécurité  
- traçabilité  
- droits des personnes  
- documentation  

---

## 🔹 6.2 ACPR – Gouvernance des algorithmes
Exigences pour les assureurs :
- explicabilité  
- supervision humaine  
- documentation complète  
- suivi de performance  
- gestion des biais  

---

# 7. Conclusion

Ces concepts constituent la base méthodologique de l’audit IT, Data, Cyber et IA.  
Ils permettent d’évaluer la maturité de l’organisation, d’identifier les risques et de formuler des recommandations alignées avec les meilleures pratiques du secteur.


