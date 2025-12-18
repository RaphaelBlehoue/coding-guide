# 📄 CONTEXTE MÉTIER GLOBAL

---

## 1. Vision et intention stratégique

Le produit vise à répondre à un besoin critique du monde agricole :  
👉 **reprendre le contrôle opérationnel, agronomique et économique des exploitations**, dans un contexte de complexité croissante (climat, coûts, volatilité des marchés, pression réglementaire).

L’application se positionne comme un **outil d’aide à la décision métier**, permettant à l’exploitant de piloter son exploitation **à distance**, de manière **factuelle, continue et traçable**, en s’appuyant sur des données structurées et comparables dans le temps.

---

## 2. Problématique métier identifiée

Les exploitants agricoles font face à plusieurs difficultés structurelles :

- Suivi terrain **irrégulier ou non standardisé**
- Décisions souvent basées sur :
  - l’expérience empirique
  - des observations partielles
  - des données dispersées
- Difficulté à :
  - comparer l’état réel des cultures à un référentiel agronomique fiable
  - détecter précocement les anomalies (stress, maladies, retards)
  - mesurer l’impact économique des décisions techniques
- Dépendance à la présence physique sur le terrain
- Faible capacité de **pilotage à distance**

**Source** : CONTEXTE MÉTIER.

---

## 3. Objectifs métier principaux

### 3.1 Objectifs fonctionnels

- Mettre en place un **suivi régulier et standardisé** des cultures
- Comparer automatiquement :
  - le **pipeline agronomique attendu**
  - avec le **stade observé réel**
- Détecter de manière systématique :
  - écarts de développement
  - anomalies
  - maladies
  - stress abiotiques
- Proposer des **actions recommandées** basées sur :
  - des protocoles de traitement formalisés
  - des règles métier explicites
- Centraliser les données techniques et économiques
- Fournir une **vision consolidée et synthétique** via dashboard et alertes

**Source** : CONTEXTE MÉTIER + priorisation MVP utilisateur.

---

### 3.2 Objectifs décisionnels

- Aider l’exploitant à :
  - anticiper les risques
  - prioriser les interventions
  - arbitrer entre coût, rendement et risque
- Permettre une **prise de décision à distance**, fondée sur :
  - données climatiques réelles
  - données terrain actualisées
  - indicateurs économiques

---

## 4. Périmètre métier du MVP

### 4.1 Fonctionnalités incluses

Le MVP couvre **l’intégralité de la chaîne de valeur décisionnelle** :

- Suivi des cultures (observations terrain)
- Pipeline agronomique de référence
- Comparaison attendu / observé
- Détection d’écarts et anomalies
- Recommandations basées sur protocoles
- Vision économique consolidée :
  - rendements
  - intrants
  - main-d’œuvre
  - coûts
- Dashboard global
- Système d’alertes
- Données climatiques via API réelle
- Données marché (API ou simulation)

**Source** : CONTEXTE PÉRIMÈTRE & MAQUETTES + décision MVP utilisateur.

---

### 4.2 Hors périmètre explicite

Sont exclus du MVP :

- Optimisation prédictive long terme non validée
- Automatisation complète des interventions terrain
- Fonctions sociales ou communautaires
- Modules réglementaires avancés non spécifiés

*(Aucune extrapolation au-delà des documents fournis.)*

---

## 5. Acteurs métier (personas)

### 5.1 Exploitant agricole

- Responsable du suivi des cultures
- Décideur final des actions à mener
- Utilisateur principal du dashboard et des alertes

### 5.2 Système applicatif

- Compare automatiquement données observées et référentielles
- Déclenche alertes et recommandations
- Agrège données techniques, climatiques et économiques

**Source** : CONTEXTE MÉTIER.

---

## 6. Données clés manipulées

- Données de parcelles
- Données d’observation terrain
- Pipelines agronomiques
- Protocoles de traitement
- Données climatiques (API externe réelle)
- Données de marché (API ou simulées)
- Données économiques (coûts, intrants, main-d’œuvre)

---

## 7. Dépendances et contraintes

### 7.1 Dépendances externes

| Domaine | Statut MVP | Justification |
|------|-----------|--------------|
| Climat | API réelle obligatoire | Données critiques pour analyse agronomique |
| Marché | API ou simulation | Donnée informative, non bloquante |

---

### 7.2 Contraintes métier

- Données fiables et traçables
- Comparaisons reproductibles dans le temps
- Lisibilité et synthèse des informations
- Utilisation possible à distance

---

## 8. Indicateurs de valeur métier

- Capacité à détecter précocement les anomalies
- Réduction du temps de décision
- Amélioration du pilotage économique
- Centralisation des informations critiques
- Meilleure anticipation des risques climatiques et sanitaires

---

## 9. Positionnement global

Le produit n’est **ni un simple outil de saisie**, ni un tableau de données brutes.  
Il se positionne comme un **assistant de pilotage agricole**, structurant l’information et guidant la décision, sans se substituer à l’expertise humaine.

---