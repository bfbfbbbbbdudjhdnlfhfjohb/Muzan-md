<p align="center"><h1>muzan-md 🚀</h1><br> </p>

![banner](muzan-md.jpg)

muzan-md est un bot multi-devices conçu pour enrichir vos conversations WhatsApp avec des fonctionnalités utiles et amusantes. Qu'il s'agisse de gérer des fichiers, d'interagir avec des stickers ou de faciliter la gestion de groupe, muzan-md est là pour vous aider ! 🎉💬

## Fonctionnalités Principales ✨

- **Téléchargement de Fichiers :** muzan-md peut télécharger des fichiers audio et vidéo à partir de liens que vous lui envoyez, pour que vous puissiez les partager facilement avec vos contacts. 🎶📹

- **Exportation de Stickers :** Vous pouvez exporter des stickers de Telegram et les utiliser dans vos conversations WhatsApp en les envoyant simplement à muzan-md. 😄✨

- **Gestion de Groupe :** muzan-md offre des fonctionnalités de gestion de groupe, comme l'ajout ou la suppression de membres, la configuration de règles et d'autres paramètres. 👥📋

- **Text to Image :** Les meilleurs logos ont été sélectionnés pour votre confort. 🖼️🎨

## Fonctionnalités Ludiques 🎉

- **Blagues et Devinettes :** muzan-md est équipé d'une collection de blagues et de devinettes pour égayer vos conversations. 😂🤔

- **Citations Inspirantes :** Recevez des citations inspirantes pour vous motiver au quotidien. 💪🌟

## Obtenir muzan-md 🛠️

1. Cliquez sur **[Fork](https://github.com/Digitalgeek-hack/Muzan-md/fork)** afin de copier le repo sur votre compte GitHub. N'oubliez pas d'ajouter une étoile 🌟 pour encourager les développeurs !

2. Obtenez une session du bot :  
   - [Session-1](https://zkscan.onrender.com)  
   - [Session-2](https://zokouscan-din3.onrender.com)

## Déploiement 🚀

- **Déploiement sur Heroku** :
  1. Si vous ne disposez pas de compte **Heroku**, cliquez [**ici**](https://id.heroku.com/login) pour en créer un.
  2. Cliquez [**ici**](https://github.com/Digitalgeek-hack/Muzan-md) pour déployer le bot sur **Heroku**.

- **Déploiement sur Koyeb** :
  1. Si vous n'avez pas de compte **Koyeb**, cliquez [**ici**](https://dashboard.koyeb.com/signup) pour en créer un.
  2. Cliquez sur le bouton ci-dessous pour déployer sur Koyeb :<br>
     [![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=muzan-md&type=docker&image=docker.io%2Fluffy077%2Fmuzanmd%3Alatest&env%5BPREFIXE%5D=.&env%5BLECTURE_AUTO_STATUS%5D=oui&env%5BTELECHARGER_AUTO_STATUS%5D=oui&env%5BNOM_BOT%5D=Zokou-MD&env%5BLIENS_MENU%5D=https%3A%2F%2Fwallpapercave.com%2Fuwp%2Fuwp3943464.jpeg&env%5BPM_PERMIT%5D=non&env%5BMODE_PUBLIC%5D=oui&env%5BETAT%5D=1&env%5BSESSION_ID%5D=mettez+votre+session&env%5BNOM_OWNER%5D=Muzan%2B%2B&env%5BNUMERO_OWNER%5D=22891733300&env%5BWARN_COUNT%5D=3&env%5BSTARTING_BOT_MESSAGE%5D=oui&env%5BANTI_VUE_UNIQUE%5D=oui&env%5BPM_CHATBOT%5D=non&env%5BHEROKU%5D=non&env%5BDATABASE_URL%5D=mettez+une+database&env%5BANTI_COMMAND_SPAM%5D=non&ports=8000%3Bhttp%3B%2F)

- **Déploiement sur Render** :
  1. Si vous n'avez pas de compte **Render**, cliquez [**ici**](https://dashboard.render.com) pour vous inscrire.
  2. Créez un nouveau sweb service.  
  3. Choisissez **Public Git Repository**.  
  4. Dans le champ , entrez `https://gitlab.com/bankai421341/senbonzakura.git`.
  5. Cliquez sur **Connect**.  
  6. Sélectionnez le **Free Plan** si vous ne voulez pas payer.  
  7. Dans la section **environemment variable**, cliquez sur **Add from .env** et copiez le contenu suivant :

     ```env
     PREFIXE=.
     LECTURE_AUTO_STATUS=oui
     TELECHARGER_AUTO_STATUS=oui
     NOM_BOT=muzan-md
     LIENS_MENU=https://files.catbox.moe/66u0k3.jpeg
     PM_PERMIT=non
     MODE_PUBLIC=oui
     ETAT=1
     SESSION_ID=muza
     NOM_OWNER=jarix
     NUMERO_OWNER=muzantech
     WARN_COUNT=3
     STARTING_BOT_MESSAGE=oui
     ANTI_VUE_UNIQUE=oui
     PM_CHATBOT=non
     ANTI_COMMAND_SPAM=non
     ```

  8. Cliquez sur **Add env** pour enregistrer, puis modifiez selon vos besoins. N'oubliez pas d'entrer votre session ID.  
  9. Cliquez sur **Deploy service** et profitez-en !


 - **Déploiement GitHub**

  1. **Forkez le dépôt**.
  2. Modifiez le fichier `exemple_de_set.env` en `set.env` et ajoutez-y votre **session_ID**.
  3. Créez un nouveau fichier `.github/workflows/deploy.yml` et mettez-y ce contenu :

```yml
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  schedule:
    - cron: '0 */4 * * *'

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: |
        npm install -g pm2
        npm install

    - name: Start application with timeout
      run: |
        timeout 14520s npm run muzan

```


## Contributions 🤝

Les contributions à muzan sont les bienvenues ! Si vous avez des idées pour de nouvelles fonctionnalités, des améliorations ou des corrections de bogues, n'hésitez pas à ouvrir une issue ou à soumettre une demande de pull. 🙌

### Remerciements :
- **Fatao**, qui a ajouté des commandes (Fancy, GPT, Dall-e, APK)  
- **CrazyPrice**, qui a hébergé un second site web pour les session_id  

## Licence 📜

Le Bot WhatsApp muzan est publié sous la [Licence MIT](https://opensource.org/licenses/MIT).

Profitez des fonctionnalités variées du Bot WhatsApp muzan pour améliorer vos conversations et rendre votre expérience WhatsApp plus intéressante ! 🎊💬

## Développeurs :
- [**muzantech**](https://github.com/Digitalgeek-hack/Muzan-md/)
- [**jarixpro᚜**](https://github.com/Digitalgeek-hack/Muzan-md)
