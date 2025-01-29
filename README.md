# TrackDown by trhacknon

![TrackDown](https://static-trkn.replit.app/trkn.svg) <!-- (Ajoutez votre logo ici si possible) -->

## 🚀 Introduction

**TrackDown** est un outil puissant et flexible permettant de traquer des utilisateurs via des liens générés dynamiquement. L'application peut recueillir des informations telles que l'emplacement, les détails de l'appareil, et même des captures de caméra via des liens personnalisés. 

### Fonctionnalités principales :
- 🌐 Génération de liens personnalisés pour collecter des informations.
- 📍 Suivi de la localisation en temps réel.
- 🎥 Captures de caméra.
- ☁️ Deux types de pages : 
  - Cloudflare (page sous attaque).
  - WebView (affiche un site dans un iframe).

## 📋 Prérequis

Avant de commencer, assurez-vous d'avoir les éléments suivants :
- Node.js et npm installés.
- Un bot Telegram et son **token**.
- Un compte sur Replit, Glitch, ou Render pour héberger l'outil.

## ⚙️ Installation et configuration

### Étape 1 : Clonez le projet
Clonez ce dépôt Git sur votre machine locale :

```bash
git clone https://github.com/tucommenceapousser/TrackDownV2.git
cd TrackDownV2
```

### Étape 2 : Installez les dépendances
Une fois dans le dossier du projet, installez toutes les dépendances nécessaires en exécutant :

```bash
npm install
```

### Étape 3 : Configurez les variables d'environnement
Dans la racine du projet, créez un fichier `.env` avec les variables suivantes :

```env
SERVER_URL=http://votre-url-de-deploiement
bot=VOTRE_TOKEN_TELEGRAM
```

- **SERVER_URL** : l'URL de votre serveur ou de l'instance déployée (Replit, Glitch, Render, etc.).
- **bot** : le token de votre bot Telegram (obtenez-le via [BotFather](https://t.me/BotFather)).

### Étape 4 : Lancer le serveur
Une fois configuré, lancez le serveur avec :

```bash
node index.js
```

Le serveur sera accessible par défaut sur le port `5000`.

## 📲 Déploiement en ligne

Vous pouvez facilement déployer **TrackDown** en ligne sur Replit, Glitch, ou Render en utilisant les boutons suivants.

### Replit

[![Déployer sur Replit](https://replit.com/badge/github/tucommenceapousser/TrackDownV2)](https://replit.com/github/tucommenceapousser/TrackDownV2)

### Glitch


[![deploy on Glitch](https://cdn.glitch.com/2703baf2-b643-4da7-ab91-7ee2a2d00b5b%2Fremix-button.svg)](https://glitch.com/edit/#!/import/github/tucommenceapousser/TrackDownV2)

### OnRender

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/tucommenceapousser/TrackDownV2)

## 🔧 Personnalisation

Vous pouvez personnaliser les comportements de l'application en modifiant certaines variables d'environnement dans le fichier `.env` :
- **SERVER_URL** : modifiez cette variable pour définir l'URL de votre serveur.
- **bot** : ajoutez le token de votre bot Telegram pour gérer les interactions.

## 🤖 Utilisation du bot Telegram

1. Lancez le bot en envoyant `/start`.
2. Utilisez `/create` pour générer de nouveaux liens de traçage.
3. Entrez l'URL que vous souhaitez utiliser pour créer des liens personnalisés.
4. Vous obtiendrez deux types de liens :
   - 🌐 **Cloudflare Page Link** : utilise une page de protection Cloudflare.
   - 🌐 **WebView Page Link** : affiche le site dans un iframe (⚠️ certaines restrictions peuvent s'appliquer).

### Commandes importantes :
- `/start` : pour démarrer l'interaction avec le bot.
- `/create` : pour générer un nouveau lien.
- `/help` : obtenir de l'aide sur l'utilisation du bot.

## THX TO Th30neAnd0nly for the good base
**https://github.com/Th30neAnd0nly/TrackDown**

## 📄 Licence

Ce projet est sous licence [MIT](LICENSE).
