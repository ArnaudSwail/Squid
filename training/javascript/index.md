# javascript

Un classique, le remplacement d'une chaine de caractères
- [string.replace all occurrences](https://stackoverflow.com/questions/21162097/node-js-string-replace-doesnt-work)

L'objet javascript, un tableau, un dictionnaire
- [How to create dictionary](https://stackoverflow.com/questions/7196212/how-to-create-dictionary-and-add-key-value-pairs-dynamically)
- [How to do associative array hashing](https://stackoverflow.com/questions/1208222/how-to-do-associative-array-hashing-in-javascript)

Mesurer le temps
- [How to measure time](https://stackoverflow.com/questions/313893/how-to-measure-time-taken-by-a-function-to-execute)

## Graphes

### algorithmes de référence
- [Javascript algorithms](https://github.com/trekhleb/javascript-algorithms)

### npath, fast path finding
[Path finding library](https://www.reddit.com/r/javascript/comments/71k0nr/i_made_a_very_fast_path_finding_library_what_do/)

- [ngraph.graph](https://github.com/anvaka/ngraph.graph)
- [ngraph.path](https://github.com/anvaka/ngraph.path)


### node-dijkstra

Installation
```
npm install node-dijkstra
```

Utilisation
```
const Graph = require('node-dijkstra')

const route = new Graph()

route.addNode('A', { B:1 })
route.addNode('B', { A:1, C:2, D: 4 })
route.addNode('C', { B:2, D:1 })
route.addNode('D', { C:1, B:4 })

route.path('A', 'D')
```
