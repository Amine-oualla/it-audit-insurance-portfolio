# 04 – Scripts d’entretiens (fictifs)

## 1. Introduction

Cette annexe présente des scripts d’entretiens fictifs menés dans le cadre de l’audit IT du système de gestion des sinistres.  
Ils illustrent la manière dont les informations ont été collectées auprès des différentes parties prenantes : IT, Sécurité, Data, IA et Métiers.

---

## 2. Entretien 1 – Responsable IT / Production

**Profil interviewé :** Responsable IT Production  
**Durée :** 45 minutes  
**Objectif :** Comprendre l’architecture du système, la gestion des changements, les sauvegardes et le PRA.

### Extraits de questions

- **Q1 :** Pouvez-vous décrire l’architecture technique du système de gestion des sinistres (environnements, bases de données, interfaces principales) ?  
- **Q2 :** Comment sont gérées les mises en production ? Existe-t-il un processus formalisé de gestion des changements ?  
- **Q3 :** Comment les sauvegardes sont-elles organisées (fréquence, périmètre, tests de restauration) ?  
- **Q4 :** Disposez-vous d’un PRA formel pour cette application ? Quand a-t-il été testé pour la dernière fois ?  
- **Q5 :** Quels sont, selon vous, les principaux risques IT liés à cette application ?

### Extraits de réponses fictives

- **R (sur la gestion des changements) :**  
  « Les mises en production passent par un comité de changement hebdomadaire, mais certains correctifs urgents sont parfois déployés en direct pour des raisons métiers. La documentation n’est pas systématiquement mise à jour. »

- **R (sur le PRA) :**  
  « Le PRA existe sur le papier, mais le dernier test complet remonte à plus d’un an et demi. On a fait quelques tests partiels, mais rien de global récemment. »

---

## 3. Entretien 2 – RSSI / Responsable Sécurité

**Profil interviewé :** Responsable Sécurité des Systèmes d’Information (RSSI)  
**Durée :** 45 minutes  
**Objectif :** Évaluer la sécurité, la gestion des habilitations, la journalisation et la conformité RGPD / ISO 27001.

### Extraits de questions

- **Q1 :** Comment sont gérées les habilitations sur l’application sinistres (rôles, profils, revues périodiques) ?  
- **Q2 :** Réalisez-vous des revues régulières des comptes et des droits ? À quelle fréquence ?  
- **Q3 :** Quelles actions sont journalisées aujourd’hui (accès, modifications, suppressions) ?  
- **Q4 :** Les logs sont-ils centralisés dans un SOC ? Y a-t-il des alertes sur les actions sensibles ?  
- **Q5 :** Avez-vous identifié des risques critiques spécifiques sur cette application ?

### Extraits de réponses fictives

- **R (sur les habilitations) :**  
  « Les droits sont gérés par l’équipe IT, sur demande des managers métiers. Il n’y a pas de revue systématique des habilitations, sauf en cas de départ. »

- **R (sur la journalisation) :**  
  « Les logs techniques sont activés, mais les journaux fonctionnels ne couvrent pas encore toutes les actions sensibles. Nous travaillons à les étendre. »

---

## 4. Entretien 3 – Data / Responsable Qualité des données

**Profil interviewé :** Responsable Data / BI  
**Durée :** 45 minutes  
**Objectif :** Comprendre la gouvernance des données sinistres, les contrôles de qualité et les usages analytiques.

### Extraits de questions

- **Q1 :** Quels sont les principaux usages des données sinistres (reporting, analyse, tarification, fraude) ?  
- **Q2 :** Disposez-vous de règles de validation à l’entrée (contrôles de format, de cohérence, de doublons) ?  
- **Q3 :** Suivez-vous des indicateurs de qualité des données (KPI, dashboards) ?  
- **Q4 :** Comment sont gérées les corrections de données après détection d’anomalies ?  
- **Q5 :** Quels sont, selon vous, les principaux points faibles sur la qualité des données sinistres ?

### Extraits de réponses fictives

- **R (sur les contrôles) :**  
  « Il existe quelques règles de validation basiques, mais elles ne couvrent pas toutes les situations. Par exemple, il n’y a pas de contrôle automatique sur les doublons de sinistres. »

- **R (sur le monitoring) :**  
  « Nous n’avons pas encore de dashboard de qualité des données dédié aux sinistres, mais c’est un sujet prioritaire pour l’année prochaine. »

---

## 5. Entretien 4 – Data Scientist / Responsable modèle IA fraude

**Profil interviewé :** Data Scientist en charge du modèle de détection de fraude  
**Durée :** 60 minutes  
**Objectif :** Évaluer la gouvernance du modèle IA, le suivi de performance, la gestion des dérives et des biais.

### Extraits de questions

- **Q1 :** Pouvez-vous décrire le modèle de détection de fraude (type de modèle, variables principales, données d’entraînement) ?  
- **Q2 :** Comment suivez-vous la performance du modèle en production (métriques, fréquence) ?  
- **Q3 :** Avez-vous mis en place un mécanisme de détection de dérive (model drift) ?  
- **Q4 :** Comment sont gérés les biais potentiels (discrimination, variables sensibles) ?  
- **Q5 :** Quel est le niveau de supervision humaine sur les décisions du modèle ?

### Extraits de réponses fictives

- **R (sur la performance) :**  
  « Nous suivons la performance globale du modèle tous les trimestres, mais il n’y a pas encore de monitoring automatisé en continu. »

- **R (sur la gouvernance) :**  
  « La documentation existe, mais elle n’est pas totalement à jour sur les dernières versions du modèle. Le versioning est en partie manuel. »

---

## 6. Entretien 5 – Responsable métier Sinistres

**Profil interviewé :** Responsable métier Sinistres  
**Durée :** 45 minutes  
**Objectif :** Comprendre les attentes métiers, les irritants, les risques perçus et l’usage du système au quotidien.

### Extraits de questions

- **Q1 :** Quels sont, selon vous, les principaux points forts et points faibles du système de gestion des sinistres ?  
- **Q2 :** Avez-vous déjà rencontré des problèmes d’indisponibilité ou de lenteur impactant les clients ?  
- **Q3 :** Avez-vous confiance dans la qualité des données et des reportings générés ?  
- **Q4 :** Comment percevez-vous l’utilisation du modèle IA de détection de fraude dans vos processus ?  
- **Q5 :** Si vous deviez prioriser trois actions d’amélioration, lesquelles seraient-elles ?

### Extraits de réponses fictives

- **R (sur la qualité des données) :**  
  « Il arrive que nous ayons des erreurs de dates ou de montants qui nécessitent des corrections manuelles. Ça prend du temps et peut générer des incompréhensions avec les clients. »

- **R (sur l’IA fraude) :**  
  « Le modèle nous aide, mais parfois il bloque des dossiers qui semblent légitimes. Nous aimerions avoir plus de transparence sur les raisons de certains scores. »

---

## 7. Conclusion

Ces scripts d’entretiens fictifs illustrent la démarche d’audit IT menée auprès des différentes parties prenantes.  
Ils montrent comment les constats et recommandations du rapport ont été construits à partir d’échanges structurés, orientés risques et solutions.

