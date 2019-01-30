# Node JS


## Comprendre les module exports et autres requires

- [Understanding module exports](https://www.sitepoint.com/understanding-module-exports-exports-node-js/)
- [NodeJS require cannot find custom module](https://stackoverflow.com/questions/16652620/node-js-require-cannot-find-custom-module)

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
