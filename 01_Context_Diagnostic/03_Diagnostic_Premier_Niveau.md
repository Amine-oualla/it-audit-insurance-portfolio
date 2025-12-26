# 03 – Diagnostic de premier niveau

## 3.1 Objectifs du diagnostic initial

Le diagnostic de premier niveau a pour objectif de :

- Comprendre rapidement le fonctionnement du périmètre audité  
- Identifier les zones de risque potentielles  
- Déterminer les priorités du plan de travail  
- Valider les informations clés avec les parties prenantes  
- Détecter les signaux faibles nécessitant des tests approfondis  

Ce diagnostic repose sur des interviews, une revue documentaire et une analyse préliminaire des processus et systèmes.

---

## 3.2 Interviews réalisées

Les interviews suivantes ont été menées :

- **Responsable IT – Applications Sinistres**  
  → Architecture, incidents, évolutions, dépendances techniques  

- **Responsable Sécurité / Cyber**  
  → Gestion des accès, vulnérabilités, surveillance, incidents cyber  

- **Responsable Data / IA**  
  → Modèles de détection de fraude, gouvernance, supervision, qualité des données  

- **Responsable Métier Sinistres**  
  → Processus métier, points de douleur, risques opérationnels  

- **Conformité / RGPD**  
  → Données personnelles, registres, droits d’accès, conservation  

---

## 3.3 Points forts identifiés

- **Architecture applicative documentée** et relativement stable  
- **Processus de gestion des incidents** structuré  
- **Contrôles d’accès centralisés** via un IAM (Identity & Access Management)  
- **Présence d’un SOC** (Security Operations Center) pour la surveillance cyber  
- **Modèles IA performants** pour la détection de fraude (taux de détection élevé)  

---

## 3.4 Points de vigilance

### 🔸 Gouvernance IT
- Documentation technique parfois obsolète  
- Manque de revue régulière des habilitations  
- Dépendance forte à certains prestataires externes  

### 🔸 Sécurité / Cyber
- Faible fréquence des tests de vulnérabilité  
- Journaux applicatifs incomplets ou non analysés  
- Absence de revue formelle des accès privilégiés  

### 🔸 Données & Qualité
- Incohérences ponctuelles dans les données sinistres  
- Absence de règles de validation systématiques  
- Manque de traçabilité sur certaines modifications de données  

### 🔸 IA & Détection de fraude
- Documentation limitée sur les modèles IA  
- Pas de processus formel de validation métier avant mise en production  
- Risque de dérive du modèle non surveillé  

---

## 3.5 Premières hypothèses de risques

À ce stade, les risques potentiels suivants sont identifiés :

- **Risque de disponibilité** du système sinistres  
- **Risque d’accès non autorisé** aux données sensibles  
- **Risque de fraude** en cas de contournement des contrôles IA  
- **Risque de non‑conformité RGPD** (données personnelles mal gérées)  
- **Risque de dérive ou biais du modèle IA**  
- **Risque d’intégrité des données** (erreurs, doublons, incohérences)  

Ces hypothèses seront confirmées ou infirmées lors de la cartographie des risques et du plan de travail.

---

## 3.6 Conclusion du diagnostic initial

Le diagnostic met en évidence :

- Une organisation globalement structurée  
- Des efforts importants en cybersécurité  
- Une dépendance croissante aux modèles IA  
- Plusieurs zones de risque nécessitant des tests approfondis  

Ces éléments serviront de base à la **cartographie des risques** et à la **construction du plan de travail**.


