# Fiche express application generator

## express-application-generator
Explications rapides sur l'utilisation d'express generator :

On utilise l'outil de génération d'application, express-generator pour créer rapidement
un squelette d'application.
 
Installer le module :
avec une version moderne de node (à partir de Node.js 8.2.0) : $ npx express-generator

Pour les versions antérieures:

$ npm install -g express-generator 

$ express

Pour les options :

$ express -h

Un exemple qui génère un Express app nommé myapp :

$ express --view=ejs myapp


L'app va être créée dans un dossier nommé myapp dans le dossier de travail courant et le view engine va être paramétré sur ejs

Installer les dépendances :

$ cd myapp

$ npm install

Lancer l'app sur MacOS

$ DEBUG=myapp:* npm start

Lancer l'app sur Windows

`> set DEBUG=myapp:* & npm start`

Ensuite accèdez a l'app via votre navigateur : http://localhost:3000/ 

L'app générée à la structure suivante :

app.js
bin
    www
package.json
public
    images
    javascripts
    stylesheets
        style.css
routes
    index.js
    users.js
views
    error.ejs
    index.ejs
    layout.ejs

7 dossiers, 9 fichiers

La structure de l'app créée par le générateur n'est est qu'une possible parmi d'autres. Soyez libres d'utiliser cette structure ou de la modifier pour mieux s'adapter à vos besoins.

## express-mvc-generator
Générateur d'application Model View Controller

installation :

`$ npm install express-mvc-generator -g`

pour les options :

$ express -h

Un exemple qui génère un Express app nommé myapp dans le dossier de travail courant :

$ express myapp

Installer les dépendances :

$ cd myapp && npm install

lancer l'app :

$ DEBUG=myapp:* node app or nodemon app

Structure de fichiers :

`$express myapp

* myapp
  * app
    * controllers
      * home.js
    * models
      * home.js
    * views
      * 404.ejs
      * error.ejs
      * index.ejs
      * login.ejs
      * signup.ejs
      
  * config
    * auth.js
    * constants.js
    * database.js
    * passport.js
    * routes.js
     
  * lib
    * email.js
    
  * node_modules
  
  * public.js
    * css
      * style.css
    * js
      * script.js
    * img
      * img.jpg
    * uploads
      * img.jpg
      
  * app.js
    
  * package.json`
    
Les réglages importants :
1. Ouvrir config/database.js, configurer votre mongo db
2. ouvrir config/constants.js, configurer vos constantes (SMTP ...)
3. Si vous voulez utiliser SMTP, dé-commentez les lignes de 95 à 98 du fichier passport.js

Lancez le générateur :

$ node app or nodemon app

Les urls de la démo :

`Signup : http://localhost:8042/signup`

`Login : http://localhost:8042/login`

Vous pouvez configurer le générateur avec les lignes de commandes visibles suite à la commande du help

fonctionnalités : 

Bonne structure de fichiers MVC style Express.
Exemples de Controller et modèles (Mongoose) intégrés , réglages de Passport et Settings
Les modules npm les plus utilisés et important sont pré installés , avec des exemples d'utilisation

Des exemples express mvc simples et compréhensibles inclus
Y sont inclus des  modules npm comme : pm2 ,async, body-parse, sessions, flash, cookie, dateformat, mongoose, nodemailer , nodemon, passport

Supporte ces View engines:

Jade

Handlebars

Swig

EJS

Marko

Nunjucks

Supported CSS pre-processors

SASS (both node-sass and ruby sass)

LESS

Stylus

-------------------------------------------
Supporte ces Databases (avec MVC structure):

MongoDB

MySQL

PostgreSQL

RethinkDB

SQLite


Aide et assistance : rajaram.tavalam@gmail.com






