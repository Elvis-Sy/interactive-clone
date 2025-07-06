# Clonage de id-interactive.fr

## Description

Ce projet est une reproduction du site **id-interactive.fr** utilisant React, TailwindCSS et d'autres outils.  
L'objectif est de recréer l'expérience utilisateur et le design, avec une navigation fluide et des animations modernes au scroll.

## Installation

```bash
git clone https://github.com/Elvis-Sy/interactive-clone.git
npm install
npm run dev

```

## Mode de travail

### Description

Chaque développeur travaille sur **sa propre branche**, puis **merge dans la branche principale distante** (`dev`) **via une Pull Request (PR)**.
Pour garantir un développement organisé et éviter les conflits, chaque nouvelle page est développée dans une **branche dédiée**.

#### Étapes :

1. **Créer une nouvelle branche** pour la page (exemple : `ma-page/fonctionnalite`).
2. **Développer tes fonctionnalités** dans cette branche sans impacter la branche principale (`main`).
3. Une fois la page terminée et testée, **merger** ta branche dans la branche principale.
4. Revenir à la branche principale, **mettre à jour** ta copie distante (push).
5. Répéter ce procédé pour chaque nouvelle fonctionnalité/page.

Ce workflow permet de travailler simultanément sur plusieurs fonctionnalités sans perturber la version stable.

---

### Commandes Git principales

#### 1. Créer une branche et s’y positionner

```bash
git checkout -b ma-page/fonctionnalite
```
#### 2. Travailler, commiter tes changements

```bash
git add .
git commit -m "Ajout de la page Ma Page"
```

#### 3. Revenir à la branche principale

```bash
git checkout dev
```
#### 4. Pousser ta branche sur le dépôt distant (dev)

```bash
git push origin ma-page/fonctionnalite
```

#### 5. Supprimer la branche ma-page/fonctionnalite

```bash
git branch -d ma-page/fonctionnalite
```

---

## Contenus

- [`INFORMATIONS.md`](./INFORMATIONS.md) : Tout ce qu'il y a à savoir sur les informations du projet
- [`COLORS.md`](./COLORS.md) : Les principales couleurs utilisées dans le site

---

⚠️ Veuillez ne pas travailler directement sur `main`.

✅ Branche principale de développement : `dev`

Merci de créer vos branches à partir de `dev`.

