# Global Context — Méta-instructions pour tous les agents IA

---

## REF-GN-000

**Titre :** Contexte global et règles de travail des agents IA
**Contenu :**
Ce fichier définit les règles permanentes que tous les agents IA doivent respecter, quel que soit leur domaine ou le dossier dans lequel ils opèrent.
Il constitue la **mémoire centrale** du cadre méthodologique Bleyob.

Tous les agents doivent lire et appliquer ce fichier avant d'exécuter la moindre tâche.

---

# 🧬 1. Flow méthodologique global (obligatoire)

Tous les agents IA doivent appliquer systématiquement le flow méthodologique suivant lorsque l’utilisateur présente une idée, une fonctionnalité, une User Story ou une demande d’implémentation :

**Idée → Analyse → UX → User Stories → Dev → Tests → CI/CD → Release → Prod**

Ce flow est détaillé dans **REF-GN-011** du fichier `general/bleyob_overview.md`.

---

# 🧠 2. Rappel automatique des références

## REF-GN-001

**Titre :** Rappel automatique des références (mémoire IA permanente)
**Contenu :**
Tous les agents IA doivent :

1. **Charger et mémoriser l’ensemble des références REF-XXX-YYY** présentes dans le dépôt.
2. **Utiliser ces références automatiquement** comme guides de raisonnement :
   - Flow de travail (REF-GN-011)
   - Règles User Stories (REF-GN-015, REF-GN-016)
   - Example Mapping (REF-AN-020)
   - Gherkin (REF-AN-030)
   - Clean Architecture .NET (REF-BK-001)
   - Standards React/TS (REF-FR-XXX)
   - Tests & QA (REF-TS-XXX)
   - CI/CD (REF-DV-001)
3. Appliquer les références **par défaut**, sauf si l’utilisateur en fournit d’autres explicitement.
4. Prioriser **les références globales REF-GN-\*** au-dessus des références spécifiques.

### Comportement attendu

Si l’utilisateur dit :

> « Voici une idée »
> alors l’agent doit automatiquement déclencher :

- l’étape Analyse,
- la création d’Epics, Macro-US, Micro-US,
- Example Mapping,
- Préparation Gherkin,
  sans que l’utilisateur ait besoin de le préciser.

### Exception

Si l’utilisateur dit :

> « Applique REF-BK-005 pour cette tâche »
> alors l’agent applique **uniquement** les références explicitement données.

**Référence :** Méthodologie Bleyob — IA Behavioral Rules (2025)
**Compatibilité :** toutes les références du dépôt
**Niveau :** Essentiel

---

# 🧱 3. Structure globale du dépôt

Tous les agents doivent connaître et respecter la structure globale du dépôt :

- `idea/` (optionnel)
- `analysis/` → Épuration fonctionnelle, Example Mapping, Gherkin
- `general/` → Normes globales, guidelines transverses
- `frontend/` → Méthodologies React / TS
- `backend/` → .NET / Clean Architecture
- `tests/` → Standards BDD / TDD
- `devops/` → Docker, Kubernetes, CI/CD
- `quality/` → SonarQube, règles de qualité
- `infra/` → Sécurité, bonnes pratiques
- `templates/` → PR templates, commit conventions
- `context/` → mémoire centrale (ce fichier)
- `prompts_index.md` → index des prompts par référence

---

# 🧩 4. Responsabilités par dossier

## `analysis/`

- Épics
- Macro-US
- Micro-US
- Example Mapping
- Règles métier
- Gherkin initial
- Glossaire métier

## `frontend/`

- React
- TypeScript
- UI
- State Management
- Tests front

## `backend/`

- Domain
- Application
- Infrastructure
- API
- .NET
- Architecture Patterns

## `tests/`

- Unitaires
- Intégration
- E2E
- BDD / Gherkin
- Playwright / SpecFlow

## `devops/`

- Docker
- Kubernetes
- Helm
- OpenShift
- CI/CD Pipelines
- Versioning git-cliff

---

# 🎯 5. Règles de fonctionnement pour les agents IA

### L’agent doit TOUJOURS :

- Appliquer le flow Bleyob complet
- Identifier automatiquement l’étape en cours
- Respecter les conventions REF
- Produire un travail modulaire, traçable, sourcé
- Aligner son raisonnement avec Clean Architecture
- S’appuyer sur les fichiers du dossier où il est assigné

### L’agent ne doit JAMAIS :

- Sauter d’étape dans le flow
- Écrire du code sans User Story complète
- Générer une US sans critères d’acceptation
- Produire des tests sans mapping fonctionnel
- Ignorer les références globales REF-GN-000 et REF-GN-001
- Inventer des informations non vérifiables

---

# 🔁 6. Interaction multi-agents

Lorsqu’un agent spécialisé doit coopérer avec un autre (ex. backend → tests), il doit :

1. Se référer à REF-GN-000 (mémoire globale).
2. Identifier les références du domaine cible.
3. Transmettre les données dans un format structuré :
   - ID US
   - DTO
   - Contrats
   - Acceptance Criteria
   - Mapping Gherkin
4. Assurer la cohérence de bout en bout du flow.

---

# 🎉 7. Références essentielles à connaître

- REF-GN-000 → Contexte global
- REF-GN-001 → Rappel automatique des références
- REF-GN-011 → Flow méthodologique Bleyob
- REF-GN-015 → Structure User Story
- REF-GN-016 → US enrichies
- REF-AN-010 → Analyse Macro-US / Micro-US
- REF-AN-020 → Example Mapping
- REF-AN-030 → Gherkin Guidelines
- REF-BK-001 → Clean Architecture .NET
- REF-FR-001 → Conventions React / TypeScript
- REF-DV-001 → CI/CD pipelines
- REF-TS-010 → Stratégie de tests

---

# 🧩 8. Résumé

Ce fichier constitue la **mémoire principale** de tous les agents IA travaillant dans le dépôt.
Il définit :

- les règles globales,
- le flow obligatoire,
- la façon d’utiliser les références,
- les responsabilités par dossier,
- les comportements autorisés/interdits.

Aucun agent IA ne doit commencer une tâche sans charger **REF-GN-000**.
