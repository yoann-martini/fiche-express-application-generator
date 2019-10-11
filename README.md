# fiche-express-application-generator
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

Un exemple qui génère un Express app nommé myapp : $ express --view=ejs myapp
L'app va être créée dans un dossier nommé myapp dans le dossier de travail courant et le view engine va être paramétré sur ejs

Installer les dépendances :
$ cd myapp
$ npm install

Lancer l'app sur MacOS
$ DEBUG=myapp:* npm start

Lancer l'app sur Windows
> set DEBUG=myapp:* & npm start

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
