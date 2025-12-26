# 03 – Analyses de données

## 1. Introduction

Les analyses de données permettent de confirmer ou d’infirmer les hypothèses de risques identifiées lors du diagnostic et de la cartographie.  
Elles apportent des preuves factuelles basées sur :

- des extractions de données sinistres  
- des règles de validation  
- des tests de cohérence  
- des analyses statistiques  
- des contrôles automatisés  

Ces analyses sont essentielles pour détecter anomalies, incohérences, doublons, erreurs ou signaux faibles de fraude.

---

## 2. Sources de données utilisées

Les analyses reposent sur les sources suivantes :

- Base de données **Sinistres** (production ou extraction anonymisée)  
- Tables : `Sinistre`, `Client`, `Contrat`, `Paiement`, `Fraude_Scoring`  
- Journaux applicatifs (logs)  
- Exports CSV fournis par les équipes Data  
- Données d’entraînement des modèles IA (version anonymisée)  

---

## 3. Analyses réalisées

---

## 🔹 3.1 Analyse des doublons de sinistres

### Objectif  
Identifier les dossiers potentiellement dupliqués.

### Méthode  
Recherche de doublons sur :

- numéro de contrat  
- date de sinistre  
- type de sinistre  
- montant déclaré  

### Résultats attendus  
- Détection de doublons exacts  
- Détection de doublons “fuzzy” (similaires mais pas identiques)  
- Analyse des causes (erreur humaine, bug, tentative de fraude)  

---

## 🔹 3.2 Analyse des incohérences de dates

### Objectif  
Détecter les anomalies temporelles.

### Tests réalisés  
- Date de sinistre > date de déclaration  
- Date de déclaration > date de clôture  
- Date de paiement < date de déclaration  
- Durées anormalement longues ou courtes  

### Risques associés  
- erreurs de saisie  
- contournement des contrôles  
- fraude potentielle  

---

## 🔹 3.3 Analyse des montants anormaux

### Objectif  
Identifier les montants atypiques ou incohérents.

### Méthode  
- Analyse statistique (moyenne, médiane, écart‑type)  
- Détection des outliers (valeurs extrêmes)  
- Comparaison par type de sinistre  

### Risques associés  
- erreurs de saisie  
- fraude interne ou externe  
- absence de règles de validation  

---

## 🔹 3.4 Analyse des paiements

### Objectif  
Vérifier la cohérence entre sinistres et paiements.

### Tests réalisés  
- Paiements sans sinistre associé  
- Paiements en double  
- Paiements supérieurs au montant validé  
- Paiements effectués après clôture du dossier  

### Risques associés  
- fraude  
- erreurs de traitement  
- absence de contrôles automatisés  

---

## 🔹 3.5 Analyse des performances du modèle IA

### Objectif  
Évaluer la qualité du modèle de détection de fraude.

### Tests réalisés  
- Analyse du taux de faux positifs  
- Analyse du taux de faux négatifs  
- Détection de dérive du modèle (model drift)  
- Comparaison des performances entre versions du modèle  
- Analyse de la distribution des scores  

### Risques associés  
- baisse de performance  
- fraude non détectée  
- biais algorithmique  
- absence de supervision humaine  

---

## 🔹 3.6 Analyse des logs applicatifs

### Objectif  
Vérifier la traçabilité et la sécurité.

### Tests réalisés  
- Recherche d’actions non tracées  
- Analyse des accès sensibles  
- Détection d’anomalies (pics d’activité, accès hors horaires)  
- Vérification de la complétude des logs  

### Risques associés  
- absence de traçabilité  
- accès non autorisés  
- détection tardive d’incidents  

---

## 4. Synthèse des anomalies détectées

| Analyse | Type d’anomalie | Risque associé | Criticité |
|--------|------------------|----------------|-----------|
| Doublons | Dossiers dupliqués | Fraude / erreur | Moyenne |
| Dates | Dates incohérentes | Qualité des données | Moyenne |
| Montants | Outliers | Fraude / erreur | Élevée |
| Paiements | Paiements en double | Fraude / erreur | Élevée |
| IA | Dérive du modèle | Performance IA | Moyenne |
| Logs | Actions non tracées | Sécurité | Élevée |

---

## 5. Conclusion

Les analyses de données permettent de :

- confirmer plusieurs risques identifiés  
- détecter des anomalies significatives  
- fournir des preuves factuelles pour les constats  
- orienter les recommandations du rapport final  

Elles constituent un élément clé de la mission d’audit IT.


