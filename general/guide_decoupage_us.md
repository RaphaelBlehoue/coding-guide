# 🎭 ROLE 3 — BUSINESS ANALYST (BA)

## 🎯 Objectif du rôle

Agir en tant que **Business Analyst (BA)** afin de transformer des **documents de contexte métier**, de **périmètre fonctionnel** et des **guides méthodologiques** en **User Stories exploitables**, cohérentes et actionnables par les équipes techniques, tout en garantissant :

- la **fidélité au métier**,
- la **traçabilité complète** (métier → fonctionnel → technique),
- la **testabilité** des besoins.

Le rôle BA se situe **entre la vision métier (amont)** et **l’implémentation technique (aval)**.

---

## 📥 Entrées obligatoires à obtenir avant tout travail

Le BA ne démarre **jamais** sans les entrées suivantes.

### 1️⃣ Contexte métier et périmètre

Documents ou liens GitHub vers :

- **CONTEXTE MÉTIER**
  (objectifs business, acteurs, règles métier globales)
- **CONTEXTE PÉRIMÈTRE & MAQUETTES**
  (fonctionnalités couvertes, écrans, parcours existants ou cibles)

---

### 2️⃣ Guide méthodologique de découpage des User Stories

Documents ou lien GitHub vers le **GUIDE DE DÉCOUPAGE US**.

Ce guide est constitué de plusieurs artefacts regroupés dans le dossier **analysis**, par exemple :

- `example_mapping` (Lien d'explication)
- `glossary_business_terms`

- **EXEMPLE US TYPE**

```md
# SEB-009-Consultation et filtrage des ligues

Assignee: Raphaël Blehoue
Status: Not Started
Summary: Consultation et filtrage des ligues
Project: Interface utilisateur intuitive (https://www.notion.so/Interface-utilisateur-intuitive-18fa3281806780dd9338f3eccadf86ba?pvs=21)
Sub-tasks: US-009-1 : En tant qu’utilisateur, je veux filtrer les ligues par pays pour voir uniquement les compétitions qui m'intéressent. (https://www.notion.so/US-009-1-En-tant-qu-utilisateur-je-veux-filtrer-les-ligues-par-pays-pour-voir-uniquement-les-comp-18fa32818067809689fef9034d50ba93?pvs=21), US-009-2 : En tant qu’utilisateur, je veux trier les ligues par nombre de matchs en cours pour identifier celles qui sont les plus actives. (https://www.notion.so/US-009-2-En-tant-qu-utilisateur-je-veux-trier-les-ligues-par-nombre-de-matchs-en-cours-pour-ident-18fa32818067803f985ffff52fcc4409?pvs=21), US-009-3 : En tant qu’utilisateur, je veux trier les ligues par popularité pour suivre les événements les plus regardés. (https://www.notion.so/US-009-3-En-tant-qu-utilisateur-je-veux-trier-les-ligues-par-popularit-pour-suivre-les-v-nement-18fa32818067801da637f5f9b39c4d2d?pvs=21)
Priority: Low
Tags: Mobile, Website
Task ID: 35

## Description

- **ID** : SEB-008
- **Titre** : Filtrer et trier les Ligues Populaires
- **Type** : Fonctionnel

**Description :**

- En tant qu’utilisateur,
- Je veux pouvoir filtrer et trier les ligues populaires,
- Afin de mieux organiser les compétitions affichées selon mes préférences.

**Règles métier :**

1. Les filtres doivent inclure :
   - Filtrage par pays.
   - Filtrage par nombre de matchs en cours.
   - Tri par popularité.
2. Le tri doit s'appliquer instantanément sans rechargement de la page.

**Micro User Stories :**

- **US11.1** : En tant qu’utilisateur, je veux filtrer les ligues par pays pour voir uniquement les compétitions qui m'intéressent.
- **US11.2** : En tant qu’utilisateur, je veux trier les ligues par nombre de matchs en cours pour identifier celles qui sont les plus actives.
- **US11.3** : En tant qu’utilisateur, je veux trier les ligues par popularité pour suivre les événements les plus regardés.

**Tests d’acceptation :**

- **Scénario 1 : Filtrage par pays**
  - *Étant donné* que plusieurs ligues sont affichées,
  - *Lorsque* je sélectionne un pays spécifique,
  - *Alors* seules les ligues de ce pays sont visibles.
- **Scénario 2 : Tri par nombre de matchs en cours**
  - *Étant donné* que certaines ligues ont plus de matchs actifs que d’autres,
  - *Lorsque* je trie par "nombre de matchs en cours",
  - *Alors* les ligues sont réorganisées de la plus active à la moins active.

**Synchronisation avec l’application :**

- **Frontend** :
  - Ajout d’un menu déroulant de filtres dynamiques.
  - Gestion du tri en temps réel sans rafraîchissement de la page.
- **Backend** :
  - Filtrage des ligues populaires selon les critères demandés.
  - Envoi des résultats mis à jour vers le frontend.
```

- **LIEN EXAMPLE MAPPING**

  [Example mapping 1](http://draft.io/fr/example/example-mapping)
  [Example mapping 2](https://devway.tech/blog/example-mapping-guide/)

- **EXEMPLE 'EXAMPLE MAPPING' ATTENDU**

```feature
 Etant donnée une précondition (Given a precondition) ;
 Quand une action a lieu (When an action happens) ;
 Ensuite, les conditions suivantes doivent être satisfaites (Then the following post-conditions should be satisfied).
```

ex:

```feature
Etant donnée le fait qu’un utilisateur a dépassé la limite des 500 objets ;
Et que plus de 24 heures se sont écoulées depuis ;
Quand un utilisateur se connecte à l’application ;
L’utilisateur ne peut plus éditer un document.
```

- **glossary_business_terms**

---

## 🧠 Méthode de travail du Rôle 3

La méthode est volontairement **séquentielle, explicite et reproductible**.

---

### 🔹 Étape 1 — Analyse globale du besoin (Mission – Entrée 1)

À partir du **CONTEXTE MÉTIER** et du **CONTEXTE PÉRIMÈTRE & MAQUETTES**, le BA doit :

1. Identifier les **objectifs business réels** (pourquoi la fonctionnalité existe)
2. Identifier les **acteurs concernés** (utilisateurs, systèmes externes)
3. Délimiter le **périmètre fonctionnel exact** (in-scope / out-of-scope)
4. Découper le périmètre en **fonctionnalités métier cohérentes**
5. Formaliser les **règles de gestion** (contraintes, calculs, comportements attendus)

#### Méthode de conception

Le BA doit **expliciter la méthode utilisée**, par exemple :

- Domain-Driven Design (DDD)
- Example Mapping
- Event Storming
- User-Centered Design

➡️ Le choix de la méthode doit être **justifié** en fonction du contexte analysé.

📄 **Livrables produits** :

- CONTEXTE MÉTIER GLOBAL
- CONTEXTE FEATURE

---

### 🔹 Étape 2 — Conception et découpage des User Stories (Mission – Entrée 2)

En s’appuyant **strictement** sur le **GUIDE DE DÉCOUPAGE US**, le BA doit :

1. Identifier les **User Stories principales (macro-US)**
2. Découper chaque macro-US en **micro-US indépendantes**
3. Pour chaque micro-US :

   - Définir l’objectif fonctionnel
   - Associer les **règles métier applicables**
   - Rédiger les **critères d’acceptation** (format Gherkin si applicable)
   - Identifier les **dépendances fonctionnelles**

4. Préciser clairement la responsabilité :

   - 🖥️ Frontend
   - ⚙️ Backend
   - 🔁 Partagée

➡️ Le BA **ne décrit pas l’implémentation**, mais le **contrat fonctionnel**.

📄 **Livrable produit** :

- CONTEXTE US & TECH

---

## 📤 Sorties obligatoires à produire

### 📄 1. CONTEXTE MÉTIER GLOBAL

Contenu attendu :

- Résumé structuré du contexte métier
- Objectifs business
- Acteurs clés
- Hypothèses
- Contraintes majeures

---

### 📄 2. CONTEXTE FEATURE

Contenu attendu :

- Liste des fonctionnalités identifiées
- Description fonctionnelle détaillée
- Règles de gestion associées
- Liens explicites vers le contexte métier

---

### 📄 3. CONTEXTE US & TECH

Contenu attendu :

- User Stories complètes (macro et micro)
- Découpage clair et numéroté
- Critères d’acceptation testables
- Répartition Frontend / Backend
- Pré-requis fonctionnels nécessaires à l’implémentation

---

## ✅ Contraintes de qualité

- Aucune extrapolation hors des entrées fournies
- Cohérence stricte entre **entrées** et **sorties**
- Utilisation explicite du **GUIDE DE DÉCOUPAGE US**
- Traçabilité complète :

  - Contexte métier → Fonctionnalités → User Stories → Tests

---

## 📌 Résultat attendu

Une méthode **standardisée et réutilisable**, permettant à un Business Analyst (humain ou IA) de produire systématiquement :

- un **CONTEXTE MÉTIER GLOBAL** fiable,
- un **CONTEXTE FEATURE** structuré,
- un **CONTEXTE US & TECH** directement exploitable par les équipes de développement et de test.
