
## Systeme
SSD
El Capitan

## Developer
Chrome
Firefox

Atom
Github Desktop

### Python
python3

### NodeJS
[NodeJS](https://nodejs.org/en/)

npm est installé avec NodeJS

#### Projet NodeJS en ES6
Pour utiliser ES6 comme syntaxe javascript (notamment import)

```
npm install babel-cli
npm install babel-preset-es2015
```

#### Servir des pages web avec un serveur NodeJS

[Using Node as a simple web server](https://stackoverflow.com/questions/6084360/using-node-js-as-a-simple-web-server)

Installer les modules nécessaires
```
npm install connect serve-static
```

Créer un fichier *server.js*
```
var connect = require('connect');
var serveStatic = require('serve-static');
connect().use(serveStatic(__dirname)).listen(8080, function(){
    console.log('Server running on 8080...');
});
```

Lancer le serveur web
```
$ node server.js
```

##### Utiliser ES6 sur un serveur NodeJS

Installation des modules babel
```
npm install --save-dev babel-cli babel-preset-es2015 rimraf

```
rimraf est un module permettant de supprimer un répertoire et tous les fichiers contenus.

```
{
  "presets": ["es2015"]
}
```

### OpenLayers 5 avec NodeJS
https://github.com/openlayers/ol-webpack

##### Import des modules nodes dans une page web
Une page web peut utiliser certains scripts javascripts installés avec npm.

En NodeJS, pour utiliser un module, on utilise la méthode require('unelibrairie.js').
Pour utiliser la même méthode pour les pages web incluses dans un serveur node,
on utilise la librairie Browserify.

[Browserify](http://browserify.org/)



### Electron

Pour une première application avec Electron
```
$ git clone https://github.com/electron/electron-quick-start
$ cd electron-quick-start
$ npm install
$ npm start
```



### Bash
Voir [Traitment de fichiers CSV pour création d'une base de données](/pesticides/index.md)
