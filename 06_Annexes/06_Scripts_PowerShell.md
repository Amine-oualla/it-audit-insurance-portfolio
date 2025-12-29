# 06 – Scripts PowerShell (exemples d’audit IT)

## 1. Introduction

PowerShell est un outil essentiel pour les audits IT :  
- audit des habilitations  
- analyse des logs  
- vérification des configurations  
- collecte de preuves techniques  

Les scripts ci-dessous sont fictifs mais réalistes et utilisés dans un contexte d’audit.

---

## 2. Script – Détection des comptes inactifs (Active Directory)

```powershell
# Liste des comptes inactifs depuis plus de 90 jours
Search-ADAccount -AccountInactive -TimeSpan 90.00:00:00 |
Select-Object Name, SamAccountName, LastLogonDate |
Export-Csv "comptes_inactifs.csv" -NoTypeInformation
```
Objectif :  
Identifier les comptes orphelins ou non utilisés.

## 3. Script – Liste des utilisateurs avec droits admin

```powershell
Get-ADGroupMember -Identity "Administrateurs" |
Select-Object Name, SamAccountName |
Export-Csv "admins.csv" -NoTypeInformation
```
Objectif :  
Contrôler les accès privilégiés.

## 4. Script – Vérification de la journalisation Windows

```powershell
# Vérifie si l’audit des accès est activé
Get-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Control\Lsa" |
Select-Object AuditBaseObjects, AuditBaseDirectories
```
Objectif :  
Vérifier la conformité ISO 27001 / RGPD.

## 5. Script – Export des logs de sécurité

```powershell
Get-WinEvent -LogName Security -MaxEvents 500 |
Select-Object TimeCreated, Id, LevelDisplayName, Message |
Export-Csv "logs_securite.csv" -NoTypeInformation
```

Objectif :  
Analyser les événements sensibles.





