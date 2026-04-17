# 📸 MonAlbumPhoto

## 📖 Description

MonAlbumPhoto est une application web axée sur le backend permettant de gérer et organiser des collections de photos personnelles et de groupe.

Le projet vise à offrir un système structuré permettant aux utilisateurs de :

* téléverser et organiser leurs photos
* créer des albums
* identifier des personnes (privées ou liées à un groupe)
* associer des photos à des lieux
* gérer des groupes partagés avec différents niveaux de permissions

Le projet est actuellement en développement actif et met l’accent sur la mise en place d’une base backend solide avec des technologies modernes.

---

## 🛠️ Technologies utilisées

### Backend

* Node.js
* TypeScript
* Prisma ORM
* PostgreSQL

### Outils

* Git (gestion de version)
* HeidiSQL (visualisation de la base de données)
* Prisma Client (accès aux données)

---

## ⚙️ Installation

### 1. Cloner le dépôt

```bash
git clone https://github.com/ton-username/MonAlbumPhoto.git
cd MonAlbumPhoto
```

### 2. Installer les dépendances

```bash
npm install
```

### 3. Configurer les variables d’environnement

Créer un fichier `.env` à la racine du projet :

```env
DATABASE_URL=postgresql://postgres:motdepasse@localhost:5432/MonAlbumPhoto?schema=public
```

---

### 4. Initialiser la base de données

Appliquer le schéma Prisma :

```bash
npx prisma db push
```

Générer le client Prisma :

```bash
npx prisma generate
```

---

## 🧱 Structure de la base de données

Le projet comprend les entités principales suivantes :

* **User** — utilisateurs de l’application
* **Photo** — photos et leurs métadonnées
* **Album** — collections de photos
* **Location** — lieux associés aux photos
* **PrivatePerson** — personnes identifiées par un utilisateur
* **Group** — groupes partagés entre utilisateurs
* **GroupMembership** — rôles des utilisateurs dans un groupe
* **GroupPerson** — personnes associées à un groupe

Relations principales :

* Une photo peut appartenir à plusieurs albums
* Une photo peut contenir plusieurs personnes identifiées
* Un album peut être lié à un groupe
* Un utilisateur peut appartenir à plusieurs groupes avec différents rôles (VIEW, EDIT, ADMIN)

---

## 🚧 État du projet

✅ Schéma de base de données conçu et fonctionnel
✅ Prisma configuré
✅ Connexion à PostgreSQL établie
🚧 Développement des API en cours
🚧 Frontend non implémenté

---

## 🚀 Feuille de route

* [ ] Créer les API REST (Users, Albums, Photos)
* [ ] Implémenter le téléversement de photos
* [ ] Ajouter l’authentification et la gestion des permissions
* [ ] Implémenter les groupes et les rôles
* [ ] Développer une interface frontend
* [ ] Déployer l’application

---

## 📌 Remarques

Ce projet a pour objectif de :

* renforcer les compétences en backend
* maîtriser Prisma et la conception de bases de données
* construire une application complète étape par étape

---

## 👤 Auteur

Guillaume Bélanger-Méthot

---

## 📄 Licence

Projet réalisé à des fins d’apprentissage et de portfolio.
