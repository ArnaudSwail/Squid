---
title: Squid, pour gérer la documentation du Fablab
---

## Bienvenue sur la page du projet Squid

Squid est un projet pour augmenter et normaliser le contenu numérique de la [Fabrique du Loch](http://www.lafabriqueduloch.org/).

Il s'agit d'utiliser GitHub pour pérenniser l'ensemble de la documentation des projets du fablab,
gérer l'information destinée au public (une simple url serait alors communiquée)
ainsi que les pages dites statiques du site web de la Fabrique.

En créant des fichiers .md, il est possible de créer des pages web alimentant un site partagé par les membres d'un groupe.

Les fichiers .md sont des fichiers texte que l'on peut écrire simplement.
Une fois publié, le fichier est présenté sous forme de page web.
Comme cette propre page!

### Markdown
En utilisant une syntaxe simple, il est possible de composer du texte structuré avec quelques conventions simples
pour créer des mises en gras, en italique

Texte en **Gras** ou _Italique_ ou `Code`

# Titre 1
## Titre 2
### Titre 3

- Liste
- Non ordonnée

1. Liste
2. Numérotée

```markdown
Pour créer un bloc de code.
(Certains éditeurs comme Atom, vous permettent de créer un bloc de code en tapant uniquement "code" sur une seule ligne.
Le bloc sera automatiquement créé).
```

Et ces styles sont obtenus très simplement par quelques caractères spéciaux:

```
Texte en **Gras** ou _Italique_ ou `Code`

# Titre 1
## Titre 2
### Titre 3

- Liste
- Non ordonnée

1. Liste
2. Numérotée

[Lien](url)

![Image](src)

```

Il est possible de créer des tableaux et bien d'autres éléments.
Plus d'info (en anglais) sur le [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

Pour jouer sur la taille d'une image:
```
![test image size](/assets/images/juju-NB.jpg){:class="img-responsive"}
![test image size](/assets/images/juju-NB.jpg){:height="50%" width="50%"}
![test image size](/assets/images/juju-NB.jpg){:height="700px" width="400px"}
```

Allons plus loin avec quelques exemples de fichiers Markdown:
- Une page du site web, [La Fabrique du Loch](https://arnaudswail.github.io/squid/fabloch)
- Un document de l'association, [L'ordre du jour du prochain CA](CA_du_11_janvier_2019.md)
