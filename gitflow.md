# Documentation Git Flow

## Introduction
Le **Git Flow** est une stratégie de gestion des branches basée sur Git, introduite par Vincent Driessen. Elle aide à organiser le développement des fonctionnalités, la préparation des versions et la gestion des correctifs tout en maintenant une branche principale propre et stable.

## Table des matières
1. [Branches principales](#branches-principales)
   - [master](#master)
   - [develop](#develop)
2. [Branches de support](#branches-de-support)
   - [feature](#feature)
   - [release](#release)
   - [hotfix](#hotfix)

---

## Branches principales

### `master`
La branche `master` contient toujours le code en production. Chaque commit sur cette branche doit correspondre à une version stable du projet.

### `develop`
La branche `develop` est la branche par défaut pour les développements en cours. Elle contient le dernier code stable avec toutes les nouvelles fonctionnalités intégrées.

---

## Branches de support

### `feature`
Les branches `feature` sont créées à partir de la branche `develop`. Elles servent à développer des fonctionnalités spécifiques. Une fois terminées, elles sont fusionnées dans `develop`.

- **Initialisation** :
  ```bash
  git flow init

- **Ajout de branche** :
  ```bash
  git flow feature start homepage

- **Push simplifier** :
  ```bash
  git flow feature publish homepage

- **Pull Simplifier** :
  ```bash
  git flow feature pull origin homepage

  OR

  git pull origin feature/homepage

### `release`
La branche `release` permet de rassembler un ensemble de modification en une seule intégration a la branche `master`. Réduisant les incident a un minimum.

- **merge with the develop branch** :
  ```bash
    git flow release start v0.0.1
    -- Commit change --*
    git flow release finish v0.0.1

- **To see a graph of the commit** :
  ```bash
    git log --oneline --graph --color -all --decorate 

### `hotfix`
Les branches `hotfix` sont utilisées pour corriger rapidement des bugs critiques sur la branche `master`. Elles permettent d'apporter des corrections urgentes sans perturber le flux de développement principal.

- **Créer une branche hotfix**
   ```bash
  git flow hotfix start title
  -- ajout des modif -- 
  git flow hotfix finish title