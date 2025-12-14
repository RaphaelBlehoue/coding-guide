```markdown
# 📄 CONTEXTE PÉRIMÈTRE & MAQUETTES

**Rôle : Product Owner (PO) & UX/UI**
**Produit : Système d’Information de Gestion Agricole**

---

## 1. Cadre et clarification

- Les maquettes fournies ne décrivent **pas** le métier.
- Elles sont utilisées **exclusivement comme inspiration UX/UI** :
  - organisation des écrans,
  - structuration de l’information,
  - types de parcours utilisateurs,
  - patterns visuels (dashboard, cartes, listes, filtres).
- **Aucune fonctionnalité bancaire ou financière n’est retenue.**
- Le métier cible est **strictement agricole**.

Source métier unique :

- `context_metier.md` (GitHub – fourni par le sponsor)

---

## 2. Objectif produit

Construire une application permettant aux agriculteurs de :

- centraliser les données de leur exploitation,
- suivre parcelles, cultures et interventions,
- accéder à des services agricoles,
- faciliter la prise de décision à partir de données terrain (climat, marché, santé des cultures).

---

## 3. Périmètre fonctionnel (Scope)

### 3.1 Accueil / Dashboard agricole

**Objectif :** vision synthétique et pilotage rapide.

Fonctionnalités :

- vue globale de l’exploitation,
- indicateurs clés :
  - météo locale,
  - alertes (climat, maladies),
  - tâches/interventions en cours,
- accès rapide aux modules principaux.

UX :

- dashboard en cartes,
- hiérarchisation visuelle des informations.

---

### 3.2 Gestion des parcelles & cultures

Fonctionnalités :

- liste des parcelles,
- détail d’une parcelle :
  - culture en cours,
  - stade de croissance,
  - historique des interventions,
- suivi des rendements.

UX :

- navigation par cartes,
- filtres (culture, statut, période).

---

### 3.3 Climat & environnement

Fonctionnalités :

- données météo localisées,
- alertes climatiques,
- visualisation de l’impact climatique sur les cultures.

UX :

- graphiques simples,
- codes couleur et pictogrammes.

---

### 3.4 Santé des cultures / solutions maladies

Fonctionnalités :

- déclaration ou détection de maladies,
- recommandations de traitements,
- historique sanitaire par parcelle.

UX :

- parcours guidé,
- fiches explicatives claires.

---

### 3.5 Services agricoles

Fonctionnalités :

- location de matériel agricole,
- embauche de main-d’œuvre,
- prestations externes.

UX :

- logique catalogue,
- recherche et filtres,
- fiches services détaillées.

---

### 3.6 Marché agricole

Fonctionnalités :

- consultation des prix du marché,
- achat / vente de produits agricoles.

UX :

- vues comparatives,
- tendances visuelles (graphes simples).

---

### 3.7 Profil & paramètres

Fonctionnalités :

- informations de l’exploitant,
- paramètres de l’exploitation,
- historique des actions.

UX :

- navigation simple,
- accès secondaire.

---

## 4. Architecture de navigation (proposition)

Navigation principale :

- Accueil
- Parcelles
- Climat
- Santé des cultures
- Services
- Marché
- Profil

Principe :

- navigation claire,
- profondeur limitée,
- accès rapide aux fonctionnalités clés.

---

## 5. Principes UX/UI retenus

Inspirations issues des maquettes (sans reprise fonctionnelle) :

- design orienté **dashboard**,
- usage de cartes et blocs modulaires,
- visualisation de données simple et lisible,
- priorité à l’ergonomie terrain (agriculteurs).

Aucune décision graphique définitive (branding, couleurs) n’est figée.

---

## 6. Hors périmètre (à ce stade)

- fonctionnalités bancaires ou financières,
- comptabilité avancée,
- automatisation IoT non explicitement décrite dans le contexte métier,
- IA prédictive avancée (hors recommandations simples).

---

## 7. Pré-requis pour la suite

Avant passage au rôle **Business Analyst (BA)** :

- validation du périmètre fonctionnel,
- priorisation des modules (MVP),
- confirmation de la cible utilisateur principale,
- validation du support (web, mobile, hybride).

---

## 8. Statut du livrable

- 📄 CONTEXTE PÉRIMÈTRE & MAQUETTES
- Aligné strictement avec le besoin métier agricole
- Maquettes utilisées uniquement comme inspiration UX/UI
```

====Une Proposition de maquette (wireframe basse-fidélité) - (peut être améloiré)

# 📐 MAQUETTE FONCTIONNELLE — Application de Gestion Agricole

**Rôle : PO / UX-UI**
**Niveau : Wireframe basse fidélité (structure & parcours)**
**Base : CONTEXTE MÉTIER – Système d’Information de Gestion Agricole**

---

## 1. Principes généraux de la maquette

- **Mobile first**
- Usage terrain (lisibilité, actions rapides)
- Architecture simple, peu profonde
- Composants récurrents :
  - cartes,
  - listes,
  - filtres,
  - indicateurs visuels simples.
- Aucun choix de branding, couleurs ou identité graphique figé

---

## 2. Navigation globale

### Navigation principale (barre basse)

- Accueil
- Parcelles
- Climat
- Santé
- Services

### Navigation secondaire

- Marché
- Profil / Paramètres

---

## 3. Écran — Accueil / Dashboard

### Objectif

Vue synthétique de l’exploitation et accès rapide aux actions clés.

### Structure

**Header**

- Nom exploitant
- Localisation
- Icône alertes

**Bloc “Aujourd’hui”**

- Carte météo locale (température, pluie, risque)
- Carte alertes (maladies, climat, urgences)
- Carte tâches en cours (max. 3)

**Bloc KPI**

- Nombre de parcelles / surface totale
- Interventions à venir
- Dernier rendement connu / tendance simple

**Raccourcis actions**

- Ajouter une intervention
- Déclarer un problème sanitaire
- Consulter le marché
- Rechercher un service

---

## 4. Écran — Parcelles (liste)

### Objectif

Vision globale des parcelles et accès au détail.

### Structure

**Header**

- Titre “Parcelles”
- Recherche (nom / culture)

**Filtres**

- Culture
- Statut (OK / À surveiller / Alerte)
- Période
- Surface

**Liste en cartes**
Chaque carte contient :

- Nom de la parcelle
- Surface
- Culture en cours
- Stade de croissance
- État général
- Dernière intervention

**CTA flottant**

- Ajouter une intervention

---

## 5. Écran — Détail d’une parcelle

### Objectif

Suivi précis et historique d’une parcelle.

### En-tête

- Nom parcelle
- Surface
- Culture + stade
- Indicateur d’état

### Onglets

#### 5.1 Résumé

- Météo spécifique
- Alertes actives
- Prochaine action recommandée

#### 5.2 Interventions

- Liste chronologique des interventions
- Bouton “Ajouter intervention”

#### 5.3 Rendements

- Graphe simple par saison
- Dernier rendement enregistré

#### 5.4 Historique

- Événements notables (incidents, changements)

---

## 6. Écran — Climat

### Objectif

Anticipation et compréhension de l’impact climatique.

### Structure

**Sélecteur période**

- Aujourd’hui / 7 jours / 14 jours

**Blocs**

- Prévisions météo
- Alertes climatiques
- Impact sur les parcelles concernées

---

## 7. Écran — Santé des cultures

### Objectif

Détection, suivi et accompagnement sanitaire.

### Accueil module

- Bouton “Déclarer un symptôme”
- Bouton “Consulter l’historique”

### Parcours guidé (déclaration)

1. Choix de la parcelle
2. Choix culture et stade
3. Sélection des symptômes (liste / pictogrammes)
4. Validation

### Résultat

- Causes possibles
- Recommandations
- Actions de suivi

---

## 8. Écran — Services agricoles

### Objectif

Accès aux services externes agricoles.

### Structure

**Recherche + filtres**

- Type de service
- Localisation
- Disponibilité

**Catalogue**

- Cartes services (titre, description courte, zone)

**Fiche service**

- Détail
- Conditions
- Bouton de contact / demande

---

## 9. Écran — Marché agricole

### Objectif

Aide à la décision économique (consultation).

### Structure

- Sélection produit
- Zone géographique

**Blocs**

- Prix actuel
- Évolution (graphique simple)
- Comparaison des marchés

---

## 10. Écran — Profil & Paramètres

### Objectif

Gestion du compte et de l’exploitation.

### Contenus

- Informations exploitant
- Paramètres exploitation
- Préférences
- Historique des actions

---

## 11. Hors périmètre explicite

- Paiement intégré
- Banque / finance
- Comptabilité
- Automatisation IoT non définie
- IA prédictive avancée

---

## 12. Statut du livrable

- ✅ Conforme au contexte métier agricole
- ✅ Maquette fonctionnelle, non graphique
- ✅ Exploitable pour :
  - User Stories (BA),
  - priorisation MVP,
  - conception UI détaillée ultérieure
