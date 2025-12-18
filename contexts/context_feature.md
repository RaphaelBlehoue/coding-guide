# 📄 CONTEXTE FEATURE  

---

## 1. Objectif du document

Ce document décrit **l’ensemble des features fonctionnelles** du produit, structurées en deux niveaux :

1. **Features MVP** : indispensables pour délivrer la valeur métier initiale
2. **Features futures (post-MVP)** : extensions naturelles, non critiques au lancement

👉 La distinction est **volontairement explicite** afin de :
- sécuriser le périmètre MVP
- faciliter la priorisation produit
- éviter toute dérive fonctionnelle

**Sources exclusives** :  
- CONTEXTE MÉTIER  
- CONTEXTE PÉRIMÈTRE & MAQUETTES  
- Décisions MVP utilisateur  

---

# 🟢 PARTIE 1 — FEATURES MVP

---

## FEATURE MVP-01 — Gestion des exploitations & parcelles

### Objectif métier  
Structurer l’exploitation agricole comme socle de toutes les analyses.

### Description  
Permettre de définir :
- une exploitation
- ses parcelles
- les cultures associées

### Règles de gestion
- Une exploitation possède plusieurs parcelles
- Une parcelle est associée à une culture active
- Toute donnée métier est rattachée à une parcelle

---

## FEATURE MVP-02 — Suivi terrain des cultures

### Objectif métier  
Mettre en place un **suivi régulier, standardisé et traçable** des cultures.

### Description  
Saisie d’observations terrain :
- stade phénologique
- état visuel
- indicateurs agronomiques observables

### Règles de gestion
- Un suivi est horodaté
- Un suivi est lié à une parcelle
- La fréquence cible est quotidienne ou tous les 2–3 jours

---

## FEATURE MVP-03 — Pipeline agronomique de référence

### Objectif métier  
Disposer d’un **référentiel attendu** pour chaque culture.

### Description  
Définition des stades théoriques d’évolution d’une culture.

### Règles de gestion
- Un pipeline est spécifique à une culture
- Les stades sont ordonnés dans le temps
- Chaque stade possède des indicateurs attendus

---

## FEATURE MVP-04 — Comparaison attendu / observé

### Objectif métier  
Automatiser l’analyse agronomique de base.

### Description  
Comparaison systématique entre :
- données observées terrain
- pipeline agronomique de référence

### Règles de gestion
- La comparaison est déclenchée après chaque suivi
- Les écarts sont mesurés sur des critères définis

---

## FEATURE MVP-05 — Détection d’écarts, anomalies et stress

### Objectif métier  
Identifier précocement les situations à risque.

### Description  
Qualification automatique des situations :
- conforme
- écart mineur
- écart critique

### Règles de gestion
- Les seuils sont définis par règles métier
- Une anomalie peut être multi-facteurs (climat + stade)

---

## FEATURE MVP-06 — Protocoles & recommandations d’actions

### Objectif métier  
Transformer l’analyse en **aide à l’action concrète**.

### Description  
Proposition de recommandations :
- traitements
- actions correctives
- surveillance renforcée

### Règles de gestion
- Une recommandation est liée à un type d’anomalie
- Les recommandations s’appuient sur des protocoles formalisés
- Une recommandation peut être informative ou actionnable

---

## FEATURE MVP-07 — Données climatiques (API réelle)

### Objectif métier  
Contextualiser les observations et décisions.

### Description  
Intégration de données météo :
- températures
- précipitations
- événements extrêmes

### Règles de gestion
- Données issues d’une API externe réelle
- Données associées à une localisation/parcelle
- Données historisées

---

## FEATURE MVP-08 — Dashboard global de pilotage

### Objectif métier  
Offrir une **vision synthétique et actionnable** de l’exploitation.

### Description  
Vue consolidée :
- état des parcelles
- anomalies en cours
- indicateurs clés

### Règles de gestion
- Données temps quasi réel
- Hiérarchisation visuelle des priorités

---

## FEATURE MVP-09 — Système d’alertes

### Objectif métier  
Ne pas dépendre d’une consultation manuelle.

### Description  
Génération d’alertes :
- anomalies critiques
- seuils dépassés
- événements climatiques

### Règles de gestion
- Une alerte est liée à un événement détecté
- Les alertes sont consultables à distance

---

## FEATURE MVP-10 — Vision économique consolidée

### Objectif métier  
Relier décisions techniques et performance économique.

### Description  
Suivi :
- intrants
- main-d’œuvre
- coûts
- rendements estimés

### Règles de gestion
- Données économiques rattachées aux parcelles
- Calculs consolidés à l’échelle exploitation

---

## FEATURE MVP-11 — Données marché (API ou simulation)

### Objectif métier  
Informer la prise de décision économique.

### Description  
Affichage de tendances de prix agricoles.

### Règles de gestion
- Données issues d’API ou simulées
- Données non bloquantes pour les autres features

---

# 🔵 PARTIE 2 — FEATURES POST-MVP (ÉVOLUTIONS)

---

## FEATURE FUT-01 — Historisation avancée & analyses temporelles

- Comparaison inter-annuelle
- Analyse de performance par culture
- Tendances long terme

---

## FEATURE FUT-02 — Prédiction & scénarios agronomiques

- Simulation d’impact climatique
- Projection de rendement
- Aide à la planification long terme

---

## FEATURE FUT-03 — Automatisation des plans d’action

- Génération automatique de plans d’intervention
- Planification des tâches terrain

---

## FEATURE FUT-04 — Intégration capteurs & IoT

- Capteurs sol / météo
- Données temps réel terrain
- Réduction des saisies manuelles

---

## FEATURE FUT-05 — Gestion réglementaire & traçabilité avancée

- Conformité réglementaire
- Historique des traitements
- Dossiers d’audit

---

## FEATURE FUT-06 — Collaboration & multi-utilisateurs

- Partage avec conseillers agronomes
- Accès multi-rôles
- Commentaires et validations

---

## FEATURE FUT-07 — Optimisation économique avancée

- Arbitrage coût / rendement
- Optimisation des intrants
- Analyse de rentabilité fine

---

## FEATURE FUT-08 — Intégrations externes étendues

- ERP agricoles
- Outils comptables
- Plateformes de négoce

---

## 3. Synthèse de structuration

- **MVP** : pilotage agronomique + décisionnel + économique
- **Post-MVP** : automatisation, prédiction, collaboration et optimisation avancée

---