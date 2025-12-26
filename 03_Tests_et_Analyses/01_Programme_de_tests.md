# 01 – Programme de tests de la mission d’audit IT

## 1. Introduction

Le programme de tests décrit l’ensemble des vérifications, analyses et contrôles qui seront réalisés pour évaluer la maîtrise des risques IT, cyber, data et IA du système de gestion des sinistres.

Il est construit à partir :

- du diagnostic initial  
- de la cartographie des risques  
- du plan de travail validé  
- des exigences réglementaires (RGPD, ACPR, EIOPA)  
- des politiques internes du groupe  

---

## 2. Objectifs des tests

Les tests visent à :

- Vérifier l’efficacité des contrôles IT  
- Identifier les écarts et faiblesses  
- Confirmer ou infirmer les hypothèses de risques  
- Évaluer la qualité des données et des processus  
- Examiner la sécurité et la gouvernance des modèles IA  
- Produire des constats factuels et documentés  

---

## 3. Tests prévus par axe d’audit

---

## 🔹 Axe 1 : Gouvernance IT & Organisation

### Test 1.1 – Revue des procédures IT
- **Objectif :** vérifier l’existence, la mise à jour et l’application des procédures  
- **Méthode :** revue documentaire + interviews  
- **Échantillon :** procédures clés (incidents, changements, sauvegardes)  
- **Critères :** conformité aux standards internes  

### Test 1.2 – Analyse des incidents
- **Objectif :** évaluer la gestion des incidents et leur récurrence  
- **Méthode :** extraction des tickets + analyse des tendances  
- **Critères :** délais de résolution, causes racines, actions correctives  

### Test 1.3 – Revue du processus de gestion des changements
- **Objectif :** vérifier que les changements sont validés, testés et documentés  
- **Méthode :** revue d’un échantillon de changements récents  
- **Critères :** conformité au processus, documentation, approbations  

---

## 🔹 Axe 2 : Sécurité & Cybersécurité

### Test 2.1 – Analyse des habilitations
- **Objectif :** vérifier que les accès sont adaptés aux rôles  
- **Méthode :** extraction des comptes + analyse des droits  
- **Échantillon :** utilisateurs métiers, IT, comptes privilégiés  
- **Critères :** principe du moindre privilège  

### Test 2.2 – Revue des accès privilégiés
- **Objectif :** s’assurer que les comptes sensibles sont contrôlés  
- **Méthode :** revue des comptes admin + logs associés  
- **Critères :** justification, traçabilité, revue périodique  

### Test 2.3 – Analyse des vulnérabilités
- **Objectif :** évaluer la gestion des vulnérabilités  
- **Méthode :** revue des rapports de scans + patch management  
- **Critères :** délais de correction, criticité des vulnérabilités  

### Test 2.4 – Analyse des journaux (logs)
- **Objectif :** vérifier la capacité de détection des incidents  
- **Méthode :** revue des logs applicatifs et systèmes  
- **Critères :** complétude, conservation, alertes  

---

## 🔹 Axe 3 : Données & Qualité

### Test 3.1 – Tests de cohérence des données sinistres
- **Objectif :** identifier incohérences, doublons, erreurs  
- **Méthode :** extraction d’un échantillon + règles de validation  
- **Critères :** exactitude, complétude, intégrité  

### Test 3.2 – Vérification des règles de validation
- **Objectif :** s’assurer que les contrôles automatiques fonctionnent  
- **Méthode :** tests sur formulaires + revue des logs  
- **Critères :** existence, efficacité, documentation  

### Test 3.3 – Traçabilité des modifications
- **Objectif :** vérifier que les modifications sont tracées  
- **Méthode :** revue des logs + tests sur un échantillon  
- **Critères :** auteur, date, ancienne valeur, nouvelle valeur  

---

## 🔹 Axe 4 : Modèles IA (détection de fraude)

### Test 4.1 – Revue de la documentation du modèle
- **Objectif :** vérifier la complétude et la traçabilité  
- **Méthode :** revue documentaire  
- **Critères :** versioning, explicabilité, données d’entraînement  

### Test 4.2 – Analyse des performances du modèle
- **Objectif :** évaluer la précision, le rappel, la dérive  
- **Méthode :** revue des métriques + tests sur échantillon  
- **Critères :** stabilité, dérive, taux de faux positifs  

### Test 4.3 – Vérification de la supervision humaine
- **Objectif :** s’assurer que les décisions IA sont contrôlées  
- **Méthode :** interviews + revue des processus  
- **Critères :** double validation, documentation  

### Test 4.4 – Sécurité du modèle IA
- **Objectif :** vérifier que le modèle est protégé  
- **Méthode :** revue des accès + logs  
- **Critères :** accès restreints, traçabilité  

---

## 🔹 Axe 5 : Continuité d’activité

### Test 5.1 – Revue du PRA / PCA
- **Objectif :** vérifier l’existence et la mise à jour du PRA  
- **Méthode :** revue documentaire  
- **Critères :** complétude, scénarios, responsabilités  

### Test 5.2 – Vérification des tests PRA
- **Objectif :** s’assurer que le PRA a été testé  
- **Méthode :** revue des rapports de tests  
- **Critères :** fréquence, résultats, actions correctives  

---

## 6. Conclusion

Le programme de tests permet de couvrir l’ensemble des risques identifiés et garantit une évaluation complète du système sinistres, des données et des modèles IA.  
Les résultats de ces tests alimenteront les **fiches d’analyse**, les **constats** et les **recommandations** du rapport final.


