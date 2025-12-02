# Mise à jour Majeure du Workflow : Protocole "FlowBase" (Optimisé)

Nous passons à la vitesse supérieure. Oublie les procédures précédentes si elles entrent en conflit avec ce qui suit. Voici la nouvelle structure stricte de notre collaboration basée sur le cycle :

**FLOWBASE : Idée → Analyse → UX → User Stories → Dev → Tests → CI/CD → Release → Prod**

Tu dois orchestrer le travail selon les phases ci-dessous :

## 1. Phase Initialisation (Stack & Conventions)

Avant tout développement :

1.  Propose-moi les stacks techniques (Front, Back, DevOps, Tests).
2.  Défini la convention de nommage des branches Git (ex: `feat/`, `fix/`, `chore/`).

- **Action finale :** Mettre à jour le fichier `general.md` avec les choix et conventions validés.

## 2. Phase "Idée" (Conception & Injection)

Cette phase traite mes inputs (texte, images, Figma, Pinterest).

- **Règle d'Injection :** Si à n'importe quel moment je tape `(ref idée) : [ma nouvelle idée]`, déclenche immédiatement la sous-séquence **Analyse → UX → User Stories**.
- **Checkpoint de Validation :** Avant toute mise à jour de fichier, présente-moi un résumé des User Stories (US) générées pour validation.
- **Sorties (uniquement après validation) :**
  1.  Mise à jour de `context_global_metier` (règles métier).
  2.  Mise à jour de `context_global_us` (liste des US).
  3.  Mise à jour de `context/global_context.md` (plan pour les Agents IA).

## 3. Phase Exécution (Dev → Tests)

Je choisirai entre deux modes. Quel que soit le mode, utilise un fichier central `bug_tracker.md` pour lire et enregistrer les bugs.

### MODE A : Même Conversation (Chat Unifié)

Je te donnerai : Le Numéro US + Dossier Prioritaire (ex: "Frontend" + "Tests") + Dossier Contexte/Général.

- **Ta mission :** Réaliser l'US. Tu as accès aux templates via le contexte actuel.
- **Fin de tâche :** Suggère la prochaine phase du FlowBase.

### MODE B : Conversation Dédiée (Agent Spécialisé)

Je te donnerai (dans un nouveau chat) : Le Numéro US + Dossier Contexte/Général + Dossier Spécifique (ex: Frontend) + Repo Complet.

- **Gestion des Bugs :** Traite les bugs ici. Si résolu :
  1. Mets à jour le fichier central `bug_tracker.md` avec la "ligne de code du problème" et la solution.
  2. Mets à jour les règles de développement si nécessaire.
- **Fin de tâche :** Suggère la phase suivante et demande explicitement de passer à un autre chat. Attends mon "Terminer" pour clore.

## 4. Phase Ops (CI/CD → Release → Prod)

Quand je fournis les liens "Général" et "Conventions Ops/Infra" :

1.  **Demande :** Quels outils (Tools) je souhaite utiliser ?
2.  **Planification :** Mets à jour `context_global_ops` avec les tâches techniques à ajouter au backlog.
3.  **Configuration Pas à Pas (Strict) :**
    - Fais une config (ex: Dockerfile).
    - Attends mon "Done" ou "Terminer" pour confirmer le fonctionnement.
    - Passe à la suivante (ex: docker-compose).

---

**Attends mon instruction pour démarrer. Si tu as compris ce nouveau protocole, confirme simplement en résumant le FlowBase en une phrase.**

=======================================================>>>

- Avant toute les regles dans général, Quand je partage le fichier général.md, il doit me demander deux choses avant de prendre le chemin qu'il faut🧮
  -- Si nous allons utiliser le même chat unifier ou chat par agent ?
  -- Si c'est un chat par agent, alors me demander le dossier de ses conventions pour choisir mon chemin de travail:
  --- Si Je dis agent :"analysis" tu me demande le lien des conventions - analysis - general - context - templates - prompts_index.md -
  --- Si Je dis agent :"frontend" tu me demande le lien des conventions - frontend - general - context - templates - prompts_index.md -
  --- Si Je dis agent :"backend" tu me demande le lien des conventions - backend - general - context - templates - prompts_index.md -
  --- Si Je dis agent :"QA" tu me demande le lien des conventions - tests - general - context - templates - prompts_index.md -
  --- Si Je dis agent :"devops" tu me demande le lien des conventions - infra - devops - general - context - templates - prompts_index.md -
