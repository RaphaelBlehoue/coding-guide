# CONTEXTE MÉTIER — Système d’Information de Gestion Agricole

## 1. Vision et objectifs métier

### Problématique

Le chef d’entreprise gère plusieurs cultures agricoles à distance (aubergine Djamba F1, tomate Cobra, piment, poivron, etc.) sur différents sites en Côte d’Ivoire.
Il souhaite disposer d’un système d’information lui permettant de piloter son exploitation **comme s’il était physiquement sur place**.

### Objectifs métier

- Assurer un **suivi régulier** (quotidien ou tous les 2–3 jours) des cultures.
- Comparer systématiquement le **pipeline attendu** (référence agronomique) avec le **stade observé sur le terrain**.
- Détecter automatiquement les **écarts, anomalies, maladies ou stress**.
- Proposer des **actions recommandées** basées sur des **protocoles de traitement formalisés**.
- Fournir une **vision économique consolidée** (rendements, intrants, main-d’œuvre, coûts).
- Faciliter la **prise de décision à distance**, basée sur des données fiables, structurées et à jour.

_Source : Cahier des charges – Système d’Information de gestion agricole (v3)._

---

## 2. Périmètre métier

### Inclus dans le périmètre

- **Suivi des cultures** par culture et par site.
- Gestion d’un **pipeline standard par culture** (phases, semaines/jours, stades attendus).
- Tableau **« Matching pipeline vs Observé »** incluant :
  - Stade attendu vs stade observé
  - Indicateurs de croissance
  - Interventions réalisées
  - Anomalies/ravageurs
  - Statut de matching (Conforme / Retard / Avance)
  - Action recommandée
- Gestion des **protocoles de traitement** par culture et par étape (phase, semaine).
- Suivi des **interventions agricoles**.
- Suivi des **récoltes, rendements et qualité**.
- Suivi de la **main-d’œuvre** (effectifs, heures, observations).
- **Alertes automatiques** et recommandations.
- **Reporting** quotidien, hebdomadaire et mensuel.
- **Évolutivité** : ajout de nouvelles cultures, pipelines et indicateurs.

### Hors périmètre explicite

Aucun élément hors périmètre n’est explicitement défini dans les documents fournis.

---

## 3. Acteurs métier

### Acteurs principaux

- **Chef d’entreprise (sponsor métier)**

  - Consulte le tableau de bord global.
  - Analyse les rapports et indicateurs.
  - Prend les décisions stratégiques et opérationnelles.

- **Responsables terrain**
  - Saisissent les observations terrain (stades, anomalies, interventions).
  - Enregistrent les récoltes et la main-d’œuvre.
  - Consultent et appliquent les protocoles de traitement.

### Acteurs secondaires

- **Ouvriers agricoles**
  - Utilisateurs indirects via la saisie ou l’exécution des tâches terrain.
  - Rôles et droits non formalisés à ce stade.

---

## 4. Processus métier

### Processus cible (TO-BE)

1. **Saisie terrain régulière**

   - Fréquence : quotidienne ou tous les 2–3 jours.
   - Données : stades observés, indicateurs de croissance, anomalies, interventions.

2. **Analyse automatique**

   - Comparaison pipeline attendu vs observé.
   - Calcul du statut de matching.
   - Détection d’écarts et d’anomalies.

3. **Recommandations et alertes**

   - Génération d’alertes en cas de problème.
   - Proposition d’actions issues des protocoles de traitement.

4. **Suivi économique**

   - Consolidation des rendements, intrants et coûts.
   - Analyse de la performance par culture et par site.

5. **Reporting**
   - Rapports automatiques quotidiens / 2–3 jours.
   - Rapports hebdomadaires et mensuels d’évolution et de comparaison aux prévisions.

---

## 5. Règles métier

- Chaque culture dispose d’un **pipeline de référence**.
- Toute observation terrain doit être **comparée** au pipeline attendu.
- Le système doit produire un **statut de matching** standardisé.
- Toute anomalie ou écart significatif déclenche une **alerte**.
- Les **recommandations** sont toujours issues des **protocoles de traitement** associés.
- Les protocoles sont structurés par **culture → phase → semaine/âge de la plante**.
- Les données doivent être **compréhensibles sur le terrain** et **exploitables à distance**.

---

## 6. Contraintes métier

- Utilisation terrain via **application mobile Android**.
- Consultation et pilotage via **interface web** (PC ou mobile).
- Interface simple, robuste et adaptée aux conditions terrain.
- Respect des exigences de **sécurité et de bonnes pratiques agricoles**
  (normes non détaillées dans les documents fournis).

---

## 7. Finalité métier

Mettre à disposition un système d’information permettant :

- Un **pilotage agricole à distance en temps réel**.
- Une **prise de décision basée sur des données factuelles**.
- Une **amélioration durable de la productivité et des rendements**.
- Une exploitation structurée, traçable et évolutive.
