# 05 – Fichiers CSV fictifs (exemples pour analyses)

## 1. Introduction

Ces fichiers CSV fictifs illustrent les données analysées dans le cadre de l’audit IT :  
- données sinistres  
- habilitations  
- logs applicatifs  
Ils permettent de démontrer les analyses SQL, Python et Excel réalisées.

---

## 2. Exemple : sinistres.csv

| id_sinistre | numero_contrat | date_sinistre | date_declaration | montant | type_sinistre |
|-------------|----------------|---------------|------------------|---------|---------------|
| 1001 | C-45821 | 2024-01-12 | 2024-01-15 | 850 | Bris de glace |
| 1002 | C-45821 | 2024-01-12 | 2024-01-15 | 850 | Bris de glace |
| 1003 | C-99877 | 2024-02-03 | 2024-02-01 | 1200 | Incendie |
| 1004 | C-77412 | 2024-03-10 | 2024-03-11 | 300 | Vol |
| 1005 | C-77412 | 2024-03-10 | 2024-03-11 | 300 | Vol |

**Utilité :**
- détection de doublons  
- incohérences de dates  
- montants atypiques  

---

## 3. Exemple : habilitations.csv

| user_id | nom | role | acces_admin | dernier_login |
|---------|-----|------|-------------|----------------|
| U001 | Martin | Gestionnaire | Non | 2024-03-01 |
| U002 | Dupont | Admin | Oui | 2023-11-15 |
| U003 | Leroy | Gestionnaire | Oui | 2024-02-20 |
| U004 | Karim | Analyste | Non | 2024-03-05 |
| U005 | Durand | Admin | Oui | 2022-09-10 |

**Utilité :**
- audit des droits  
- détection des comptes inactifs  
- séparation des tâches  

---

## 4. Exemple : logs.csv

| timestamp | user | action | objet | resultat |
|-----------|------|--------|--------|----------|
| 2024-03-01 22:15 | U003 | MODIFICATION | Sinistre 1001 | OK |
| 2024-03-01 22:16 | U003 | SUPPRESSION | Sinistre 1001 | OK |
| 2024-03-02 01:12 | U002 | ACCES_ADMIN | Table Paiements | OK |
| 2024-03-02 14:22 | U001 | CONSULTATION | Sinistre 1004 | OK |

**Utilité :**
- analyse des actions sensibles  
- détection d’activités nocturnes  
- supervision des accès admin  

---

## 5. Conclusion

Ces fichiers CSV fictifs permettent d’illustrer les analyses techniques réalisées dans le cadre de l’audit IT et renforcent la crédibilité du projet.
