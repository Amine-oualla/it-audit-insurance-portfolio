# 02 – Constats et risques

## 1. Introduction

Cette section présente les constats issus des tests et analyses réalisés dans le cadre de la mission d’audit IT.  
Chaque constat est associé à un risque, une cause probable, un impact potentiel et une évaluation de criticité.  
Ces éléments constituent la base du rapport final et du plan d’action.

---

## 2. Constat 1 – Habilitations excessives

### 🔹 Description du constat
Plusieurs utilisateurs disposent d’habilitations supérieures à leurs besoins opérationnels (accès transverses, droits d’administration non justifiés).

### 🔹 Risque associé
Accès non autorisé à des données sensibles, fraude interne, violation RGPD.

### 🔹 Cause probable
Absence de revue périodique des habilitations, manque de séparation des tâches.

### 🔹 Impact potentiel
Fuite de données, erreurs critiques, non‑conformité réglementaire.

### 🔹 Criticité
Élevée

---

## 3. Constat 2 – Traçabilité insuffisante des actions sensibles

### 🔹 Description du constat
Les logs applicatifs ne tracent pas toutes les actions critiques (modifications de données, accès privilégiés).

### 🔹 Risque associé
Impossibilité de reconstituer un incident ou une fraude.

### 🔹 Cause probable
Configuration incomplète des journaux, absence de supervision.

### 🔹 Impact potentiel
Détection tardive d’incidents, non‑conformité RGPD/ACPR.

### 🔹 Criticité
Élevée

---

## 4. Constat 3 – Incohérences dans les données sinistres

### 🔹 Description du constat
Présence d’incohérences dans les données : dates incorrectes, doublons, montants atypiques.

### 🔹 Risque associé
Décisions erronées, fraude non détectée, reporting faussé.

### 🔹 Cause probable
Erreurs de saisie, absence de contrôles automatiques robustes.

### 🔹 Impact potentiel
Perte financière, mauvaise expérience client, non‑conformité.

### 🔹 Criticité
Moyenne à élevée

---

## 5. Constat 4 – Gouvernance IA insuffisante

### 🔹 Description du constat
Le modèle IA de détection de fraude manque de documentation, de versioning et de suivi de performance.

### 🔹 Risque associé
Dérive du modèle, augmentation des faux négatifs, biais algorithmique.

### 🔹 Cause probable
Absence de processus formel de gouvernance IA.

### 🔹 Impact potentiel
Fraude non détectée, décisions injustes, non‑conformité ACPR.

### 🔹 Criticité
Élevée

---

## 6. Constat 5 – PRA non testé récemment

### 🔹 Description du constat
Le Plan de Reprise d’Activité (PRA) n’a pas été testé depuis plus de 18 mois.

### 🔹 Risque associé
Indisponibilité prolongée du système sinistres en cas d’incident majeur.

### 🔹 Cause probable
Manque de coordination entre IT et métiers.

### 🔹 Impact potentiel
Arrêt de l’activité, perte financière, atteinte à la réputation.

### 🔹 Criticité
Moyenne

---

## 7. Conclusion

Les constats identifiés mettent en évidence des risques significatifs liés à la sécurité, à la qualité des données, à la gouvernance IA et à la continuité d’activité.  
Ces constats serviront de base aux recommandations détaillées dans la section suivante.


