# 02 – Tableau de suivi des recommandations

## 1. Introduction

Ce tableau permet de suivre l’avancement des recommandations issues de l’audit IT du système de gestion des sinistres.  
Il constitue un outil central pour :

- piloter les actions correctives  
- suivre les risques résiduels  
- informer la Direction IT, la Sécurité, la Data et les Métiers  
- préparer les comités de suivi et les revues d’audit interne  

---

## 2. Tableau de suivi

| ID | Recommandation | Criticité | Responsable | Date cible | Statut | Avancement | Preuves attendues |
|----|----------------|-----------|-------------|------------|--------|------------|--------------------|
| R1 | Revue trimestrielle des habilitations | Élevée | IT / Sécurité | 30/06/2025 | En cours | 40% | Export IAM, procédure mise à jour |
| R2 | Activation complète de la journalisation + SOC | Élevée | Sécurité | 31/07/2025 | Non démarré | 0% | Configuration logs, rapport SOC |
| R3 | Renforcement des règles de validation des données | Moyenne à Élevée | Data / BI | 15/09/2025 | En cours | 25% | Documentation règles, tests SQL |
| R4 | Gouvernance IA formelle (versioning, suivi) | Élevée | Data Science | 30/08/2025 | En retard | 10% | Documentation modèle, métriques |
| R5 | Test annuel du PRA | Moyenne | IT / Continuité | 31/12/2025 | Non démarré | 0% | Rapport de test PRA |
| R6 | Nettoyage des comptes inactifs | Élevée | IT | 15/05/2025 | Terminé | 100% | Export comptes supprimés |
| R7 | Mise en place d’un monitoring qualité des données | Moyenne | Data | 30/10/2025 | En cours | 20% | Dashboard qualité, règles automatiques |
| R8 | Supervision humaine systématique des décisions IA | Élevée | Métiers / Data Science | 30/09/2025 | En cours | 30% | Procédure, journal des validations |
| R9 | Politique de rétention des logs | Moyenne | Sécurité | 31/07/2025 | Non démarré | 0% | Politique validée, configuration |
| R10 | Documentation des dépendances critiques | Moyenne | IT Architecture | 31/08/2025 | En cours | 50% | Schémas d’architecture mis à jour |

---

## 3. Légende des statuts

- **Non démarré** : aucune action engagée  
- **En cours** : actions en progression  
- **En retard** : date cible dépassée  
- **Bloqué** : dépendance ou obstacle majeur  
- **Terminé** : actions réalisées, en attente de validation audit  
- **Clôturé** : validé par l’audit interne après reperforming  

---

## 4. Points d’attention pour le prochain comité

- R2 (journalisation + SOC) : action critique non démarrée  
- R4 (gouvernance IA) : retard significatif, risque élevé  
- R5 (test PRA) : à planifier rapidement  
- R7 (qualité des données) : dépendance avec les équipes métiers  

---

## 5. Conclusion

Le tableau de suivi permet une vision claire et opérationnelle de l’avancement des recommandations.  
Il facilite la prise de décision, la priorisation et la communication entre les équipes IT, Sécurité, Data, Métiers et Audit interne.


