# GENERAL — Conventions Globales FlowBase

---

## REF-GN-050

**Titre :** Convention de Nommage des Branches Git
**Contenu :**
Les branches Git doivent suivre la structure FlowBase, et inclure systématiquement l’ID de la User Story (US) ou du Bug.

### Branches principales

- `main` → Production
- `dev` → Pré-production / intégration
- `uat` → Environnement de recette
- `ops` → Infrastructure / CI-CD (optionnel)

### Branches de travail (obligatoires)

- `feat/USxxx-nom-court`
- `fix/BUGxxx-description`
- `test/USxxx-suite-de-tests`
- `refactor/composant`
- `docs/sujet`
- `chore/maintenance`
- `ops/task`

**Exemples :**

- `feat/US034-auth-login-form`
- `fix/BUG112-null-reference-login`
- `test/US021-auth-playwright-tests`

**Référence :** GitFlow Extended 2025 + FlowBase Branch Rule
**Compatibilité :** REF-GN-000, REF-GN-001
**Niveau :** Essentiel

---

## REF-GN-051

**Titre :** Stack Technique Validée (Front, Back, Tests, DevOps)
**Contenu :**
La stack suivante est **la stack officielle FlowBase**. Tous les agents IA doivent l’utiliser par défaut.

---

### 🟦 **Default-Frontend**

- React 19
- TypeScript 5
- Vite 6
- Zustand (state simple)
- Jotai ou Redux Toolkit (state complexe)
- React Query (données asynchrones)
- UI : TailwindCSS + RadixUI
- Tests : Vitest + Testing Library
- E2E : Playwright

**Référence :** React 19 Docs (2025), Vite 6 Docs

---

### 🟥 **Default-Backend**

- .NET 8 ou .NET 9
- Architecture : Clean Architecture (Domain / Application / Infra / API)
- Minimal API
- EF Core 9
- MediatR
- FluentValidation
- AutoMapper
- PostgreSQL (DB par défaut)

**Référence :** Microsoft Learn .NET 9 (2025), Jason Taylor Clean Architecture

---

### 🟪 **Default-Tests**

- Frontend : Vitest, Playwright, MSW
- Backend : xUnit, SpecFlow, FluentAssertions
- BDD : Cucumber / Gherkin
- API : Postman ou Newman
- Mocking : Moq / FakeItEasy

**Référence :** Testing Library 2024–2025, Cucumber Docs

---

### 🟧 **Default-DevOps**

- Docker 25.x
- Docker Compose
- Kubernetes 1.31
- Helm 3.x
- OpenShift 4.x
- GitHub Actions ou Azure DevOps (selon projet)
- Versioning : git-cliff
- Monitoring : Grafana / Prometheus (optionnel)

**Référence :** CNCF 2025 Recommended Stack

---

## REF-GN-052

**Titre :** Standards de Documentation FlowBase
**Contenu :**
Tous les fichiers doivent respecter les standards suivants :

1. Toujours inclure un identifiant REF-XXX.
2. Toujours citer les sources officielles (docs React, Microsoft, Cucumber, etc.).
3. Toujours structurer les fichiers en :
   - Titre
   - Référence REF
   - Contenu
   - Compatibilité
   - Niveau (Essentiel / Recommandé / Optionnel)

---

## REF-GN-053

**Titre :** Conventions de Travail FlowBase
**Contenu :**

1. Toute nouvelle idée débute par la syntaxe :
   `(ref idée) : [ma nouvelle idée]`
   → déclenche immédiatement **Analyse → UX → User Stories**

2. Aucun code ne peut être généré avant validation explicite d’une User Story.

3. Toute communication entre agents IA doit :

   - mentionner la phase FlowBase
   - fournir les REF utilisées
   - pointer vers les fichiers contextuels mis à jour

4. Les fichiers contextuels sont sacrés :
   - `global_context.md`
   - `context_global_metier.md`
   - `context_global_us.md`
   - `context_global_ops.md`
   - `bug_tracker.md`

---

**Fin du fichier.**
