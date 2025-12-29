# 03 – Reperforming des tests (validation des actions)

## 1. Objectif du reperforming

Le reperforming consiste à **refaire les tests** après la mise en œuvre des actions correctives afin de :

- vérifier que les recommandations ont été appliquées correctement  
- confirmer que le risque est réellement réduit  
- valider la clôture de la recommandation  
- documenter les preuves de conformité  
- garantir la durabilité des mesures mises en place  

Le reperforming est une étape obligatoire avant la clôture officielle d’une recommandation.

---

## 2. Méthodologie de reperforming

Le reperforming suit une démarche structurée en quatre étapes :

### 🔹 Étape 1 – Analyse des preuves fournies
- Vérification de la complétude des preuves  
- Vérification de la pertinence (preuve liée à l’action)  
- Vérification de la date (preuve récente)  
- Vérification de la traçabilité  

### 🔹 Étape 2 – Reproduction des tests initiaux
L’auditeur refait **exactement les mêmes tests** que lors de l’audit initial :

- tests techniques IT  
- requêtes SQL  
- analyses de logs  
- tests de qualité des données  
- tests de gouvernance IA  
- vérification PRA  

### 🔹 Étape 3 – Analyse des résultats
- Comparaison avant / après  
- Vérification de la réduction du risque  
- Identification d’éventuels risques résiduels  
- Vérification de la conformité aux standards (ISO 27001, RGPD, ACPR, ITGC)  

### 🔹 Étape 4 – Conclusion et décision
- **Clôture** si les actions sont efficaces  
- **Maintien ouvert** si les actions sont insuffisantes  
- **Replanification** si des actions complémentaires sont nécessaires  

---

## 3. Exemple de reperforming par recommandation

### 🔹 R1 – Revue trimestrielle des habilitations
**Test initial :** comptes inactifs, droits excessifs  
**Action :** revue trimestrielle + nettoyage  
**Reperforming :**  
- Exécution d’une extraction IAM  
- Vérification des comptes supprimés  
- Vérification des rôles mis à jour  
**Résultat attendu :** aucun compte orphelin, droits alignés  

---

### 🔹 R2 – Activation des logs + SOC
**Test initial :** actions sensibles non tracées  
**Action :** activation logs + intégration SOC  
**Reperforming :**  
- Analyse des logs récents  
- Vérification des alertes SOC  
- Vérification de la rétention  
**Résultat attendu :** traçabilité complète  

---

### 🔹 R3 – Qualité des données
**Test initial :** dates incohérentes, doublons  
**Action :** règles de validation + monitoring  
**Reperforming :**  
- Requête SQL sur les incohérences  
- Analyse des doublons  
- Vérification des contrôles automatiques  
**Résultat attendu :** réduction significative des anomalies  

---

### 🔹 R4 – Gouvernance IA
**Test initial :** absence de versioning, métriques  
**Action :** documentation + suivi mensuel  
**Reperforming :**  
- Vérification du versioning  
- Analyse des métriques récentes  
- Vérification de la supervision humaine  
**Résultat attendu :** modèle stable et documenté  

---

### 🔹 R5 – Test PRA
**Test initial :** PRA non testé depuis 18 mois  
**Action :** test PRA annuel  
**Reperforming :**  
- Vérification du rapport de test  
- Vérification des actions correctives  
- Vérification des dépendances critiques  
**Résultat attendu :** PRA opérationnel  

---

## 4. Critères de validation

Une recommandation est considérée comme **clôturée** si :

- les preuves sont complètes et vérifiables  
- les tests reproduits confirment l’efficacité  
- le risque résiduel est faible ou acceptable  
- les actions sont durables (pas temporaires)  
- les processus ont été mis à jour  

---

## 5. Documentation du reperforming

Chaque reperforming doit être documenté dans :

- le tableau de suivi  
- un dossier de preuves (captures, exports, logs, scripts)  
- une note de validation audit interne  

Cette documentation garantit la traçabilité et la conformité.

---

## 6. Conclusion

Le reperforming est une étape essentielle pour garantir que les recommandations de l’audit IT sont réellement mises en œuvre et efficaces.  
Il permet de sécuriser le système, de réduire les risques et d’assurer une amélioration continue des pratiques IT, Data, Sécurité et IA.


