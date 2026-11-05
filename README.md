# 📦 Adopt Your Pokemon - Projet Central

Bienvenue dans le dépôt central du projet **Adopt Your Pokemon**, une application web "full-stack" interactive permettant aux utilisateurs d'adopter, de collectionner et d'interagir avec des Pokémon virtuels. 

Ce dépôt agit comme un conteneur principal. Il utilise les sous-modules Git (`.gitmodules`) pour lier et versionner conjointement les environnements Frontend et Backend.

## 🏗️ Architecture du Projet

Le projet est divisé en deux sous-modules distincts, séparant clairement l'interface utilisateur de la logique d'affaires et de l'API :

*   **[Frontend](https://github.com/Milleboy2007/Adopt_My_Pokemon_FrontEnd.git)** : Interface utilisateur moderne développée avec React 19, Vite et React Router v7.
*   **[Backend](https://github.com/Milleboy2007/Adopt_My_Pokemon_Backend.git)** : API RESTful robuste développée avec NestJS v11, TypeORM et SQLite.

## 🚀 Installation et Initialisation

Lors du clonage de ce dépôt central, il est impératif d'initialiser les sous-modules pour récupérer le code du Frontend et du Backend.

```bash
# 1. Cloner le dépôt central avec ses sous-modules
git clone --recursive <URL_DU_DEPOT_CENTRAL>

# Si le dépôt est déjà cloné mais que les dossiers frontend/backend sont vides :
git submodule update --init --recursive
```

## 🛠️ Démarrage Rapide

Pour lancer le projet complet en environnement de développement, vous devrez démarrer les deux serveurs dans des terminaux séparés.

**Terminal 1 : Backend**
```bash
cd backend
npm install
npm run seed
npm run start:dev
```

**Terminal 2 : Frontend**
```bash
cd frontend
npm install
npm run dev
```

L'application web sera accessible à l'adresse `http://localhost:5173` et communiquera de façon transparente avec l'API sur `http://localhost:3000`.