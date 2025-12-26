# 01 – Cartographie des risques IT dans le secteur assurantiel

## 1. Introduction

La cartographie des risques IT permet d’identifier, d’évaluer et de prioriser les risques susceptibles d’impacter le système de gestion des sinistres et les modèles IA associés.  
Elle constitue la base du plan de travail de la mission d’audit.

---

## 2. Méthodologie utilisée

La démarche repose sur :

- Interviews des parties prenantes (IT, Sécurité, Data, Métier, Conformité)  
- Analyse documentaire (politiques IT, procédures, schémas d’architecture, rapports internes)  
- Diagnostic initial (points forts / points de vigilance)  
- Analyse des risques sectoriels (assurance, cyber, IA)  
- Référentiels : ISO 27001, ITGC, RGPD, COSO, EIOPA  

Chaque risque est évalué selon :

- **Probabilité** (Faible / Moyenne / Élevée)  
- **Impact** (Faible / Moyen / Élevé)  
- **Criticité** = combinaison probabilité × impact  

---

## 3. Risques IT majeurs identifiés

### 🔹 3.1 Risque de disponibilité des systèmes critiques
- **Cause :** incidents techniques, pannes, dépendance à des prestataires, absence de PRA testé  
- **Impact :** impossibilité de traiter les sinistres, perte de service client  
- **Probabilité :** Moyenne  
- **Criticité :** Élevée  

### 🔹 3.2 Risque d’intégrité des données sinistres
- **Cause :** erreurs de saisie, absence de contrôles automatiques, incohérences inter‑systèmes  
- **Impact :** décisions erronées, fraude non détectée, reporting faussé  
- **Probabilité :** Moyenne  
- **Criticité :** Élevée  

### 🔹 3.3 Risque de confidentialité des données personnelles
- **Cause :** habilitations trop larges, accès non révoqués, logs incomplets  
- **Impact :** violation RGPD, sanctions ACPR, perte de confiance  
- **Probabilité :** Moyenne  
- **Criticité :** Élevée  

### 🔹 3.4 Risque cyber (intrusion, ransomware)
- **Cause :** vulnérabilités non corrigées, absence de tests réguliers, phishing  
- **Impact :** paralysie des systèmes, fuite de données, chantage  
- **Probabilité :** Élevée  
- **Criticité :** Élevée  

---

## 4. Risques liés à l’IA et à la détection de fraude

### 🤖 4.1 Risque de dérive du modèle IA
- **Cause :** absence de recalibrage, données d’entraînement obsolètes  
- **Impact :** baisse de performance, fraude non détectée  
- **Criticité :** Moyenne  

### 🤖 4.2 Risque de biais algorithmique
- **Cause :** données historiques biaisées, absence de revue métier  
- **Impact :** décisions injustes, non‑conformité réglementaire  
- **Criticité :** Moyenne  

### 🤖 4.3 Risque de manque de traçabilité
- **Cause :** documentation insuffisante, absence de versioning des modèles  
- **Impact :** impossibilité d’expliquer une décision automatisée  
- **Criticité :** Élevée  

### 🤖 4.4 Risque de sécurité des modèles IA
- **Cause :** accès non contrôlé aux modèles, attaques adversariales  
- **Impact :** manipulation des prédictions, fraude  
- **Criticité :** Moyenne  

---

## 5. Risques opérationnels liés au processus sinistres

### 📝 5.1 Risque d’erreur dans le traitement des sinistres
- **Cause :** absence de double validation, surcharge des équipes  
- **Impact :** indemnisation incorrecte, litiges  
- **Criticité :** Moyenne  

### 📝 5.2 Risque de fraude interne ou externe
- **Cause :** contrôles insuffisants, absence de revue des accès sensibles  
- **Impact :** pertes financières, réputation  
- **Criticité :** Élevée  

---

## 6. Synthèse visuelle de la cartographie des risques

| Domaine | Risque | Probabilité | Impact | Criticité |
|--------|--------|-------------|--------|-----------|
| IT | Disponibilité | Moyenne | Élevé | Élevée |
| IT | Intégrité des données | Moyenne | Élevé | Élevée |
| IT | Confidentialité | Moyenne | Élevé | Élevée |
| Cyber | Ransomware | Élevée | Élevé | Élevée |
| IA | Dérive du modèle | Moyenne | Moyen | Moyenne |
| IA | Biais | Moyenne | Moyen | Moyenne |
| IA | Traçabilité | Moyenne | Élevé | Élevée |
| Opérationnel | Erreur sinistres | Moyenne | Moyen | Moyenne |
| Opérationnel | Fraude | Moyenne | Élevé | Élevée |

---

## 7. Conclusion

La cartographie met en évidence :

- Une forte exposition aux risques **cyber**, **données** et **confidentialité**  
- Une dépendance croissante aux **modèles IA**, nécessitant une gouvernance renforcée  
- Des risques opérationnels significatifs liés au traitement des sinistres  

Ces éléments serviront de base au **plan de travail de la mission**, qui détaillera les tests à mener pour chaque risque prioritaire.


