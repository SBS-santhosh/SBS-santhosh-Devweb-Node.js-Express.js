
# SBS-santhosh-Devweb-Node.js-Express.js

Application CRUD de gestion de clients avec Node.js et Express.js

## Description

Application web permettant de gérer une liste de clients (id, nom, prénom) avec les opérations CRUD :
- **C**reate (Créer)
- **R**ead (Lire)
- **U**pdate (Modifier)
- **D**elete (Supprimer)

## Prérequis

- Node.js (version 18 ou supérieure)
- npm (généralement installé avec Node.js)

## Installation

1. Clonez le repository
```bash
git clone https://github.com/votre-username/SBS-santhosh-Devweb-Node.js-Express.js.git
cd SBS-santhosh-Devweb-Node.js-Express.js
```

2. Installez les dépendances
```bash
npm install
```

3. Installez les modules supplémentaires
```bash
npm install method-override ejs
```

## Lancement de l'application

```bash
npm start
```

L'application sera accessible sur : `http://localhost:3000`

## Utilisation

### Routes disponibles

- `GET /clients` - Liste tous les clients
- `GET /clients/new` - Formulaire de création d'un client
- `POST /clients` - Créer un nouveau client
- `GET /clients/:id` - Afficher un client spécifique
- `GET /clients/:id/edit` - Formulaire de modification d'un client
- `PUT /clients/:id` - Mettre à jour un client
- `DELETE /clients/:id` - Supprimer un client

## Structure du projet

```
├── app.js                 # Fichier principal
├── package.json           # Dépendances du projet
├── routes/
│   └── clients.js         # Routes et logique des clients
└── views/
    └── clients/           # Vues EJS
        ├── clients.ejs    # Liste des clients
        ├── new.ejs        # Création d'un client
        ├── show.ejs       # Affichage d'un client
        └── edit.ejs       # Modification d'un client
```

## Technologies utilisées

- **Node.js** - Environnement d'exécution JavaScript
- **Express.js** - Framework web
- **EJS** - Moteur de templates
- **method-override** - Support des méthodes HTTP PUT et DELETE

## Notes

⚠️ Cette application n'utilise pas de base de données. Les données sont stockées en mémoire et seront perdues au redémarrage du serveur.

## Auteur

Santhosh - BTS SIO
```

## Points importants à ajouter dans votre `.gitignore` :

Créez un fichier `.gitignore` à la racine de votre projet :

```
# Dépendances
node_modules/

# Logs
npm-debug.log*
*.log

# Fichiers système
.DS_Store
Thumbs.db

# IDE
.vscode/
.idea/
```
