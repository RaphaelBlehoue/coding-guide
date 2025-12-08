# CONVENTION D’ANALYSE — CONSTRUCTION DU CONTEXTE MÉTIER

## Transformer un recueil de besoins client en contexte métier exploitable

---

## 1. Objectif du guide

Ce document définit **la convention officielle d’analyse** utilisée dans ce repository pour transformer un recueil de besoins client (idée, expression libre, document métier, entretien, etc.) en un **contexte métier structuré, traçable et exploitable** sur l’ensemble du cycle de vie applicatif :

**Idée → Analyse → UX → User Stories → Développement → Tests → CI/CD → Release → Production**

Il constitue :
- un **référentiel méthodologique** pour les humains,
- un **guide d’entraînement et d’exécution** pour les assistants IA,
- une **base de vérité métier** indépendante de toute solution technique.

---

## 2. Définition formelle du contexte métier

### 2.1 Définition

Un **contexte métier** est la représentation **structurée, explicite et justifiée** :

- des **objectifs métier** poursuivis,
- des **problèmes réels à résoudre**,
- des **utilisateurs et rôles impliqués**,
- des **processus métier existants et cibles**,
- des **règles, contraintes et hypothèses**,

qui expliquent **pourquoi l’application existe**, **pour qui**, et **dans quelles conditions réelles**.

> Le contexte métier répond à la question fondamentale :
> **« Pourquoi cette application existe-t-elle, pour qui, et sous quelles contraintes métier ? »**

---

## 3. Principe fondamental : du besoin exprimé au besoin métier

### 3.1 Limites du recueil de besoins brut

Un recueil de besoins client contient souvent :
- des solutions déguisées en besoins (« il faut un bouton », « on veut un dashboard »),
- des attentes contradictoires,
- des besoins implicites ou mal formulés.

👉 Ce matériau est **nécessaire mais insuffisant**.
Il ne constitue **pas encore** un contexte métier exploitable.

---

### 3.2 Paradigme d’analyse utilisé

La convention repose sur le paradigme de **l’Analyse des Exigences Métier (Business Requirements Analysis)**.

La première étape est l’**élicitation des besoins**, dont l’objectif est :

> **Comprendre le problème avant de définir la solution.**

---

## 4. Étape 1 — Élicitation structurée des besoins

### 4.1 Définition

L’**élicitation des besoins** est un processus systématique visant à :
- identifier,
- comprendre,
- clarifier

les besoins réels des parties prenantes, **au-delà de leurs formulations initiales**.

---

### 4.2 Techniques d’élicitation reconnues

Les techniques suivantes sont considérées comme valides et recommandées :

- entretiens semi-directifs avec les parties prenantes,
- observation des pratiques réelles (shadowing, immersion terrain),
- ateliers collaboratifs (workshops),
- analyse de documents existants,
- questionnaires ciblés,
- prototypage exploratoire.

---

### 4.3 Livrable attendu

Un **corpus brut de besoins**, sans interprétation ni priorisation, contenant :
- citations directes,
- faits observables,
- demandes exprimées telles quelles.

---

## 5. Étape 2 — Structuration analytique des besoins

### 5.1 Objectif

Transformer un corpus hétérogène en **informations métier structurées**, indépendantes de toute solution technique.

---

### 5.2 Axes de structuration obligatoires

Les besoins doivent être classés selon les axes suivants :

#### A. Objectifs métier
- Pourquoi ce projet existe-t-il ?
- Quels résultats mesurables sont attendus ?

#### B. Utilisateurs et rôles
- Qui utilise le système ?
- Dans quel cadre organisationnel ou professionnel ?

#### C. Processus métier
- Comment le travail est-il réalisé aujourd’hui (AS-IS) ?
- Où se situent les frictions, pertes ou risques ?

#### D. Règles métier
- Quelles règles sont non négociables ?
- Quelles validations, calculs ou contraintes s’appliquent ?

#### E. Contraintes
- réglementaires,
- techniques,
- organisationnelles,
- budgétaires.

---

### 5.3 Livrable attendu

Un **document de besoins structurés**, encore **indépendant de toute décision de conception ou technique**.

---

## 6. Étape 3 — Formalisation du contexte métier

### 6.1 Structure obligatoire du document « Contexte métier »

Le document `context_metier.md` doit respecter la structure suivante :

#### 1. Vision et objectifs métier
- Problème principal à résoudre
- Valeur attendue
- Indicateurs de succès (KPI)

#### 2. Périmètre métier
- Ce qui est inclus
- Ce qui est explicitement exclu

#### 3. Acteurs et utilisateurs
- rôles,
- responsabilités,
- interactions.

#### 4. Processus métier clés
- processus actuels (AS-IS),
- processus cibles (TO-BE).

#### 5. Règles métier
- règles de gestion,
- règles de validation,
- dépendances métier.

#### 6. Contraintes et hypothèses
- contraintes externes,
- hypothèses retenues et leur justification.

---

### 6.2 Rôle central du contexte métier

Le contexte métier devient :
- la **référence unique de compréhension métier**,
- le **socle de cohérence** pour UX, User Stories, tests et releases,
- un **artefact vivant**, maintenu à jour tout au long du projet.

---

## 7. Alignement avec le cycle de vie applicatif

### Idée / Analyse
Valide que l’idée répond à un **problème réel et justifié**.

### UX
Alimente :
- personas,
- parcours utilisateurs,
- scénarios d’usage.

### User Stories
Chaque User Story doit être traçable vers :
- un objectif métier,
- un processus métier,
- une règle métier.

### Développement
Les priorités techniques sont guidées par la **valeur métier**, pas par la complexité.

### Tests
Les critères d’acceptation sont dérivés directement des règles métier.

### CI/CD – Release – Production
Les releases sont évaluées selon leur **impact métier mesurable**.

---

## 8. Bonnes pratiques essentielles

- Séparer strictement **besoins métier** et **solutions techniques**.
- Maintenir le contexte métier à jour.
- Valider systématiquement avec des experts métier.
- Utiliser un vocabulaire métier stable et partagé.

---

## 9. Références (sources vérifiables)

- Sommerville, I. *Software Engineering*, 10e éd., Pearson, 2016.
- IEEE. *Guide to the Software Engineering Body of Knowledge (SWEBOK)*, v3.0, 2014.
- ISO/IEC/IEEE 29148:2018 — *Requirements Engineering*.
- Pulsion Technology, *Requirements Analysis for Software Development*, 2023.
- Software Development UK, *Best Practices for Capturing Business Requirements*, 2022.
- Wikipedia, « Requirements elicitation » (mise à jour continue).

---

## 10. Finalité pour un assistant IA

Un assistant IA appliquant cette convention doit être capable de :

- distinguer besoin exprimé et besoin métier,
- produire un contexte métier structuré, justifié et traçable,
- relier chaque artefact projet à une finalité métier explicite,
- refuser toute implémentation sans contexte métier valide.
