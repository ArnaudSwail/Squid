# Electron

Electron permet de développer des applications desktop à partir d'une application NodeJS.

Chaque page de l'application desktop est donc une page html faisant appel à du code javascript.

Des librairies propres à NodeJS permettent d'interagir avec le système d'exploitation de la machine,
notamment la gestion de fichiers.

[Debugging Electron application](https://www.sitepoint.com/debugging-electron-application/)

Sur Github, openlayers-electron montre une intégration d'une page
utilisant Openlayers dans une application Electron.
Note: Dans cet exemple, OpenLayers n'est pas accessible depuis le script index.js de l'application.


## Tips and Tricks

[La doc complète](https://electronjs.org/docs/all)

### couldn't set selectedTextBackgroundColor from default ()
Parfois, la console peut afficher le message suivant:
```
Electron Helper[1944:91412] Couldn't set selectedTextBackgroundColor from default ()
```
[Couldn't set selectedTextBackgroundColor from default()](https://github.com/electron/electron/issues/4420)
En placant le code suivant dans le HTML, le message n'apparait plus.
```
<style> ::selection { background: white; /* WebKit/Blink Browsers */ } </style>
```

### Sqlite3
Il faut construire ce module natif avec les configurations de base d'Electron.

```
$ npm install electron-rebuild
$ ./node_modules/.bin/electron-rebuild -w sqlite3 -p

```

[How to build an Electron app](https://blog.alexdevero.com/electron-app-pt1/)

[Electron app can't find sqlite3 module](https://stackoverflow.com/questions/38716594/electron-app-cant-find-sqlite3-module)
[How to use Sqlite3 in electron](https://stackoverflow.com/questions/32504307/how-to-use-sqlite3-module-with-electron)

[How does `db.serialize` work in `node-sqlite3`](https://stackoverflow.com/questions/41949724/how-does-db-serialize-work-in-node-sqlite3)
[Promise with sqlite3](https://stackoverflow.com/questions/40691884/nodejs-sqlite-why-each-statement-return-no-results)


#### Prepared Statements
```
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database('data.db');

db.serialize(function() {

  var stmt = db.prepare("INSERT INTO users VALUES (?,?)");
  for (var i = 0; i < 10; i++) {
      stmt.run("user " + i, "email " + i);
  }
  stmt.finalize();

  stmt = db.prepare("SELECT * FROM users WHERE id=?");
  stmt.each(userId, function(err, row) {
      console.log(row.name, row.email);
  }, function(err, count) {
      stmt.finalize();
  });
});
```

https://electronjs.org/docs/tutorial/application-distribution
