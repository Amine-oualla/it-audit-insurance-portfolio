# 07 – Extraits de logs (fictifs)

## 1. Introduction

Cette annexe présente des extraits de logs fictifs utilisés dans le cadre de l’audit IT.  
Ils illustrent les analyses réalisées sur :

- les actions sensibles  
- les accès administrateurs  
- les anomalies horaires  
- les suppressions ou modifications de données  
- les événements de sécurité Windows  

Ces exemples permettent de démontrer la capacité à analyser la traçabilité et à identifier des risques opérationnels ou de sécurité.

---

# 2. Logs applicatifs – Actions sur les sinistres

| timestamp | user | action | objet | resultat | commentaire |
|-----------|------|--------|--------|----------|-------------|
| 2024-03-01 22:15 | U003 | MODIFICATION | Sinistre 1001 | OK | Action hors horaires |
| 2024-03-01 22:16 | U003 | SUPPRESSION | Sinistre 1001 | OK | Suppression sensible |
| 2024-03-02 09:12 | U001 | CONSULTATION | Sinistre 1004 | OK | Normal |
| 2024-03-02 14:22 | U001 | MODIFICATION | Sinistre 1004 | OK | Normal |
| 2024-03-03 01:05 | U002 | ACCES_ADMIN | Table Paiements | OK | Accès admin nocturne |

**Points d’analyse possibles :**
- actions sensibles (modification / suppression)  
- activités nocturnes  
- accès administrateurs sur des tables critiques  
- absence de justification métier  

---

# 3. Logs de sécurité Windows (fictifs)

| TimeCreated | EventID | Level | Source | Message |
|-------------|---------|--------|---------|---------|
| 2024-03-01 21:58 | 4624 | Information | Security | Connexion réussie – U003 |
| 2024-03-01 22:14 | 4670 | Warning | Security | Tentative de modification d’un objet protégé |
| 2024-03-01 22:16 | 4660 | Information | Security | Suppression d’un objet – Sinistre 1001 |
| 2024-03-02 01:12 | 4624 | Information | Security | Connexion réussie – U002 (admin) |
| 2024-03-02 01:13 | 4688 | Information | Security | Processus PowerShell lancé |

**Points d’analyse possibles :**
- connexions nocturnes  
- actions PowerShell non justifiées  
- événements liés à la suppression d’objets  
- tentatives de modification d’objets protégés  

---

# 4. Logs de base de données (fictifs)

| timestamp | user | requete | table | statut |
|-----------|------|---------|--------|--------|
| 2024-03-01 22:15 | U003 | UPDATE | sinistres | OK |
| 2024-03-01 22:16 | U003 | DELETE | sinistres | OK |
| 2024-03-02 01:12 | U002 | SELECT * | paiements | OK |
| 2024-03-02 01:13 | U002 | UPDATE | paiements | OK |
| 2024-03-02 09:30 | U001 | SELECT | sinistres | OK |

**Points d’analyse possibles :**
- accès admin sur la table *paiements*  
- modifications nocturnes  
- suppression de données sensibles  
- absence de séparation des tâches  

---

# 5. Logs réseau (fictifs)

| timestamp | ip_source | ip_destination | port | action | resultat |
|-----------|-----------|----------------|------|--------|----------|
| 2024-03-01 22:10 | 10.0.12.45 | 10.0.0.5 | 443 | Connexion | OK |
| 2024-03-01 22:16 | 10.0.12.45 | 10.0.0.5 | 443 | Upload | OK |
| 2024-03-02 01:12 | 10.0.3.12 | 10.0.0.5 | 3389 | RDP | OK |
| 2024-03-02 01:13 | 10.0.3.12 | 10.0.0.5 | 5985 | WinRM | OK |

**Points d’analyse possibles :**
- connexions RDP nocturnes  
- transferts de fichiers suspects  
- accès à distance par comptes admin  

---

# 6. Conclusion

Ces extraits de logs fictifs permettent d’illustrer les analyses techniques réalisées dans le cadre de l’audit IT.  
Ils renforcent la crédibilité du projet en montrant la capacité à :

- analyser la traçabilité  
- identifier des anomalies  
- détecter des risques de sécurité  
- comprendre les comportements utilisateurs  
- auditer les accès administrateurs  

