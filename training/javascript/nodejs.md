# Node JS

[Permettre l'utilisation des imports en NodeJS](https://timonweb.com/posts/how-to-enable-es6-imports-in-nodejs/)


## Comprendre les module exports et autres requires

- [Understanding module exports](https://www.sitepoint.com/understanding-module-exports-exports-node-js/)
- [NodeJS require cannot find custom module](https://stackoverflow.com/questions/16652620/node-js-require-cannot-find-custom-module)

[Writing neat asynchronous Node JS code with Promises](https://medium.com/dev-bits/writing-neat-asynchronous-node-js-code-with-promises-32ed3a4fd098)

## Comment lire un fichier ligne par ligne

NodeJS propose la méthode fs.readfile pour lire les données d'un fichier.
Mais quand le fichier est trop volumineux, cette fonction ne peut gérer l'espace mémoire requis pour
stocker tout le contenu du fichier.
Il est alors nécessaire de lire le fichier ligne par ligne par exemple.

```
var lineReader = require('readline').createInterface({
  input: require('fs').createReadStream('file.in')
});

lineReader.on('line', function (line) {
  console.log('Line from file:', line);
});
```

- [Read a file line by line](https://stackoverflow.com/questions/6156501/read-a-file-one-line-at-a-time-in-node-js)

Dans certains cas (obscurs), la lecture de fichiers ne se fait pas.
Le problème peut être contourné en utilisant le module **byline** qui semble plus robuste.
[node-byline](https://github.com/jahewson/node-byline)

- [Convertir un buffer en chaîne de caractères](https://hackernoon.com/https-medium-com-amanhimself-converting-a-buffer-to-json-and-utf8-strings-in-nodejs-2150b1e3de57)
- [Ecrire dans un fichier en nodejs](https://stackoverflow.com/questions/2496710/writing-files-in-node-js)


## Sqlite3
[Query](http://www.sqlitetutorial.net/sqlite-nodejs/query/)
[How to read a sqlite3 database using node js synchronously](https://stackoverflow.com/questions/15575914/how-to-read-a-sqlite3-database-using-node-js-synchronously)

[Controlling the Execution Flow of Statements](http://www.sqlitetutorial.net/sqlite-nodejs/statements-control-flow/)
