# 02 – Risques Cyber et Risques liés à l’Intelligence Artificielle

## 1. Introduction

Cette section présente les risques spécifiques liés à la cybersécurité et à l’utilisation de modèles d’intelligence artificielle dans le système de gestion des sinistres d’AssurOne Group.  
Ces risques complètent la cartographie générale et nécessitent une attention particulière en raison :

- de l’augmentation des cyberattaques dans le secteur assurantiel  
- de la dépendance croissante aux modèles IA pour la détection de fraude  
- des exigences réglementaires renforcées (ACPR, RGPD, EIOPA)  

---

## 2. Risques Cyber

### 🔐 2.1 Risque d’accès non autorisé aux données sensibles
- **Cause :** habilitations trop larges, absence de revue périodique, comptes orphelins  
- **Impact :** fuite de données personnelles, violation RGPD, sanctions  
- **Probabilité :** Moyenne  
- **Criticité :** Élevée  

### 🛡️ 2.2 Risque de ransomware ou d’intrusion
- **Cause :** vulnérabilités non corrigées, absence de tests de pénétration réguliers  
- **Impact :** paralysie du système sinistres, perte d’exploitation, chantage  
- **Probabilité :** Élevée  
- **Criticité :** Élevée  

### 📉 2.3 Risque de défaillance des contrôles de sécurité
- **Cause :** logs incomplets, absence de corrélation d’événements, SOC sous‑dimensionné  
- **Impact :** détection tardive d’incidents, propagation d’attaques  
- **Probabilité :** Moyenne  
- **Criticité :** Élevée  

### 🔄 2.4 Risque lié aux prestataires externes
- **Cause :** dépendance à des services cloud ou infogérés  
- **Impact :** indisponibilité, perte de données, non‑conformité contractuelle  
- **Probabilité :** Moyenne  
- **Criticité :** Moyenne  

---

## 3. Risques liés à l’Intelligence Artificielle

### 🤖 3.1 Risque de dérive du modèle (model drift)
- **Cause :** évolution des comportements fraudeurs, données obsolètes  
- **Impact :** baisse de performance, fraude non détectée  
- **Probabilité :** Moyenne  
- **Criticité :** Moyenne  

### ⚖️ 3.2 Risque de biais algorithmique
- **Cause :** données d’entraînement biaisées, absence de revue métier  
- **Impact :** décisions injustes, non‑conformité réglementaire  
- **Probabilité :** Moyenne  
- **Criticité :** Moyenne  

### 📉 3.3 Risque de sur‑dépendance au modèle IA
- **Cause :** absence de double validation humaine, automatisation excessive  
- **Impact :** erreurs non détectées, décisions incorrectes  
- **Probabilité :** Moyenne  
- **Criticité :** Élevée  

### 🔍 3.4 Risque de manque de traçabilité et d’explicabilité
- **Cause :** documentation insuffisante, absence de versioning des modèles  
- **Impact :** impossibilité d’expliquer une décision automatisée (ACPR, RGPD)  
- **Probabilité :** Moyenne  
- **Criticité :** Élevée  

### 🔐 3.5 Risque de compromission du modèle IA
- **Cause :** accès non contrôlé au modèle, attaques adversariales  
- **Impact :** manipulation des prédictions, fraude  
- **Probabilité :** Faible à Moyenne  
- **Criticité :** Moyenne  

---

## 4. Synthèse des risques Cyber & IA

| Domaine | Risque | Probabilité | Impact | Criticité |
|--------|--------|-------------|--------|-----------|
| Cyber | Accès non autorisé | Moyenne | Élevé | Élevée |
| Cyber | Ransomware | Élevée | Élevé | Élevée |
| Cyber | Défaillance des contrôles | Moyenne | Élevé | Élevée |
| Cyber | Prestataires externes | Moyenne | Moyen | Moyenne |
| IA | Dérive du modèle | Moyenne | Moyen | Moyenne |
| IA | Biais algorithmique | Moyenne | Moyen | Moyenne |
| IA | Sur‑dépendance | Moyenne | Élevé | Élevée |
| IA | Manque de traçabilité | Moyenne | Élevé | Élevée |
| IA | Compromission du modèle | Faible/Moyenne | Moyen | Moyenne |

---

## 5. Conclusion

Les risques cyber et IA constituent des enjeux majeurs pour le système sinistres.  
Ils nécessitent :

- une gouvernance renforcée  
- des contrôles techniques réguliers  
- une supervision humaine des modèles IA  
- une documentation complète et à jour  
- une surveillance continue des accès et des vulnérabilités  

Ces risques guideront la construction du **plan de travail** et des **tests d’audit**.


