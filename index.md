---
title: Squid, pour gérer la documentation du Fablab
---

# Bienvenue sur la page du projet Squid

Squid est un projet pour augmenter et normaliser le contenu numérique de la [Fabrique du Loch](http://www.lafabriqueduloch.org/).

Il s'agit d'utiliser GitHub pour
- pérenniser l'ensemble de la documentation des projets du fablab,
- gérer l'information destinée au public (une simple url serait alors communiquée)
- ainsi que les pages dites statiques du site web de la Fabrique.


En créant des fichiers .md, il est possible de créer des pages web alimentant un site partagé par les membres d'un groupe.

Les fichiers .md sont des fichiers texte que l'on peut écrire simplement.
Une fois publié, le fichier est présenté sous forme de page web.
Comme cette propre page!

## La syntaxe Markdown
En utilisant une syntaxe simple, il est possible de composer du texte structuré avec quelques conventions simples
pour créer des mises en gras, en italique, des titres, des listes, inclure des liens, des images, des tableaux, etc.


### Quelques exemples de mise en pages

# Titre 1
## Titre 2
### Titre 3

Texte en **Gras** ou _Italique_ ou `Code`

- Liste
- Non ordonnée

1. Liste
2. Numérotée

```markdown
Voici un bloc de code.
(Certains éditeurs comme Atom, vous permettent de créer un bloc de code en tapant uniquement "code" sur une seule ligne.
Le bloc sera automatiquement créé).
```


Ces styles sont obtenus très simplement par quelques caractères spéciaux:

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

Il est aussi possible de créer des tableaux et bien d'autres éléments.
Plus d'info (en anglais) sur le [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

Quelques [astuces](tipstricks.md) pour mettre en page en utilisant Markdown

## Github pages
Les pages de ce projet sont gérées par Github Pages.

Un dépôt Github a été créé: [Projet Squid](http://github.com/arnaudswail/squid/)

Les fichiers .md sont stockés dans le dépôt et peuvent être éditer par plusieurs méthodes:
- Directement sur le site Github.com
- En récupérant les fichiers du dépôt sur son ordinateur; On modifie les fichiers localement
puis on utilise Git (Github Desktop par exemple) pour télécharger les modification sur Github.com pour être prises en compte.

Github utilise Jekyll un moteur de génération de pages HTML à partir des fichiers .md.
Parfois, une fois mis à jour sur le site, il faut attendre quelques minutes pour voir le fichier HTML modifié.

## Quelques exemples
Allons plus loin avec quelques exemples de fichiers Markdown:
- Une page du site web, [C'est quoi un Fablab?](https://arnaudswail.github.io/squid/fabloch)
- Un document de l'association, [L'ordre du jour du prochain CA](CA_du_11_janvier_2019.md)

- [La Fabrique du Loch](https://arnaudswail.github.io/squid/association)
- [Le règlement intérieur](https://arnaudswail.github.io/squid/reglement)
- [Nos services](https://arnaudswail.github.io/squid/services)
- [Des liens utiles](liens)
