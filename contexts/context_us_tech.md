# 📄 CONTEXTE US & TECH — Micro-US techniques  
## Lot 1 — 5 US (conforme US Type)

---

## EPIC MVP-05 — Détection d’écarts, anomalies et stress  
### FEATURE — Analyse des écarts agronomiques

- **US-11 — Détecter automatiquement une anomalie agronomique**

  **Description :**  
  En tant que système,  
  Je veux analyser les écarts entre l’observé et le pipeline attendu,  
  Afin d’identifier automatiquement les anomalies ou situations à risque.

  **Micro User Stories :**
  - **US-11-FE — Afficher le statut d’anomalie sur l’interface parcelle**  
    En tant qu’exploitant, je veux visualiser clairement si une anomalie est détectée afin d’identifier rapidement les parcelles à risque.
  - **US-11-BE — Analyser les écarts et détecter une anomalie**  
    En tant que système, je veux appliquer les règles de seuil afin de détecter automatiquement une anomalie agronomique.

---

## EPIC MVP-05 — Détection d’écarts, anomalies et stress  
### FEATURE — Qualification des anomalies

- **US-12 — Identifier le type d’anomalie détectée**

  **Description :**  
  En tant que système,  
  Je veux qualifier le type d’anomalie détectée,  
  Afin d’adapter les recommandations agronomiques.

  **Micro User Stories :**
  - **US-12-FE — Afficher le type d’anomalie détectée**  
    En tant qu’exploitant, je veux connaître la nature de l’anomalie afin de comprendre la situation terrain.
  - **US-12-BE — Qualifier l’anomalie selon des règles métier**  
    En tant que système, je veux classifier l’anomalie (stress, maladie, retard, excès) selon les données disponibles.

---

## EPIC MVP-06 — Protocoles & recommandations  
### FEATURE — Génération de recommandations

- **US-14 — Identifier le protocole applicable à une anomalie**

  **Description :**  
  En tant que système,  
  Je veux identifier le protocole agronomique adapté à une anomalie,  
  Afin de proposer une réponse cohérente et formalisée.

  **Micro User Stories :**
  - **US-14-FE — Afficher le protocole associé à une anomalie**  
    En tant qu’exploitant, je veux consulter le protocole recommandé afin de comprendre les actions proposées.
  - **US-14-BE — Sélectionner le protocole applicable**  
    En tant que système, je veux associer une anomalie à un protocole selon les règles métier définies.

---

## EPIC MVP-06 — Protocoles & recommandations  
### FEATURE — Aide à la décision

- **US-15 — Générer une recommandation d’action**

  **Description :**  
  En tant que système,  
  Je veux générer une recommandation d’action,  
  Afin d’aider l’exploitant à corriger la situation détectée.

  **Micro User Stories :**
  - **US-15-FE — Présenter une recommandation d’action claire**  
    En tant qu’exploitant, je veux visualiser les actions recommandées afin de décider rapidement.
  - **US-15-BE — Générer une recommandation basée sur un protocole**  
    En tant que système, je veux transformer un protocole en recommandation exploitable.

---

## EPIC MVP-07 — Données climatiques  
### FEATURE — Intégration météo

- **US-17 — Récupérer les données climatiques via une API externe**

  **Description :**  
  En tant que système,  
  Je veux récupérer des données climatiques fiables via une API,  
  Afin de contextualiser l’analyse agronomique.

  **Micro User Stories :**
  - **US-17-FE — Afficher les données climatiques associées à une parcelle**  
    En tant qu’exploitant, je veux consulter les données météo afin de comprendre leur impact sur mes cultures.
  - **US-17-BE — Consommer une API météo et stocker les données**  
    En tant que système, je veux interroger une API externe et persister les données climatiques.

---