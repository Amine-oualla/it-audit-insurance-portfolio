# 02 – Tests techniques IT

## 1. Introduction

Les tests techniques IT permettent d’évaluer la robustesse, la sécurité et la fiabilité du système de gestion des sinistres.  
Ils complètent les tests organisationnels et documentaires en apportant des preuves factuelles basées sur :

- des extractions techniques  
- des analyses de logs  
- des revues de configurations  
- des tests de cohérence  
- des vérifications de sécurité  

Ces tests sont réalisés en collaboration avec les équipes IT, Sécurité et Data.

---

## 2. Tests techniques sur les habilitations et les accès

### Test 2.1 – Extraction des comptes utilisateurs
- **Objectif :** identifier les comptes actifs, inactifs, orphelins  
- **Méthode :** extraction de la base IAM ou Active Directory  
- **Vérifications :**  
  - comptes sans connexion depuis > 90 jours  
  - comptes non rattachés à un manager  
  - comptes techniques non documentés  

### Test 2.2 – Analyse des droits et rôles
- **Objectif :** vérifier l’application du principe du moindre privilège  
- **Méthode :** comparaison des rôles attribués vs rôles attendus  
- **Vérifications :**  
  - droits excessifs  
  - accès transverses non justifiés  
  - absence de séparation des tâches (SoD)  

### Test 2.3 – Revue des accès privilégiés
- **Objectif :** contrôler les comptes administrateurs  
- **Méthode :** revue des groupes Admin + logs associés  
- **Vérifications :**  
  - justification des accès  
  - traçabilité des actions  
  - absence de comptes partagés  

---

## 3. Tests techniques sur la sécurité et les vulnérabilités

### Test 3.1 – Analyse des rapports de vulnérabilité
- **Objectif :** évaluer la gestion des vulnérabilités  
- **Méthode :** revue des scans internes et externes  
- **Vérifications :**  
  - vulnérabilités critiques non corrigées  
  - délais de patching  
  - composants obsolètes  

### Test 3.2 – Vérification du patch management
- **Objectif :** s’assurer que les serveurs sont à jour  
- **Méthode :** revue des versions OS / middleware  
- **Vérifications :**  
  - serveurs non patchés  
  - versions non supportées  
  - absence de calendrier de patching  

### Test 3.3 – Analyse des journaux (logs)
- **Objectif :** vérifier la capacité de détection des incidents  
- **Méthode :** revue des logs applicatifs, systèmes et sécurité  
- **Vérifications :**  
  - complétude des logs  
  - conservation (rétention)  
  - alertes générées par le SOC  

---

## 4. Tests techniques sur les données

### Test 4.1 – Tests de cohérence des données sinistres
- **Objectif :** identifier incohérences, doublons, erreurs  
- **Méthode :** extraction SQL ou export CSV  
- **Vérifications :**  
  - dates incohérentes  
  - montants négatifs  
  - doublons de dossiers  
  - champs obligatoires manquants  

### Test 4.2 – Vérification de la traçabilité des modifications
- **Objectif :** s’assurer que les modifications sont tracées  
- **Méthode :** revue des logs + tests sur un échantillon  
- **Vérifications :**  
  - auteur  
  - date  
  - ancienne valeur / nouvelle valeur  

### Test 4.3 – Vérification des règles de validation
- **Objectif :** tester les contrôles automatiques  
- **Méthode :** saisie de cas tests + revue des logs  
- **Vérifications :**  
  - contrôles bloquants  
  - contrôles d’alerte  
  - messages d’erreur  

---

## 5. Tests techniques sur les environnements et l’architecture

### Test 5.1 – Revue des environnements (Prod / Préprod / Dev)
- **Objectif :** vérifier la séparation des environnements  
- **Méthode :** revue des configurations et accès  
- **Vérifications :**  
  - accès Dev en production  
  - données de production en Dev  
  - absence de cloisonnement  

### Test 5.2 – Vérification des sauvegardes
- **Objectif :** s’assurer que les sauvegardes sont opérationnelles  
- **Méthode :** revue des rapports de backup  
- **Vérifications :**  
  - fréquence  
  - succès / échecs  
  - tests de restauration  

### Test 5.3 – Revue de l’architecture technique
- **Objectif :** comprendre les dépendances critiques  
- **Méthode :** analyse des schémas d’architecture  
- **Vérifications :**  
  - SPOF (Single Point of Failure)  
  - dépendances externes  
  - composants obsolètes  

---

## 6. Conclusion

Les tests techniques permettent d’obtenir des preuves factuelles sur :

- la sécurité du système  
- la qualité des données  
- la robustesse des environnements  
- la conformité des accès  
- la maturité des pratiques IT  

Les résultats alimenteront les **fiches d’analyse**, les **constats**, et les **recommandations** du rapport final.


