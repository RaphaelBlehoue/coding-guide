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
