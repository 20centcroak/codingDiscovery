---
layout: course-fr
title: Modèle html
number: 1.1
---

Même si l'exemple très simple de la première leçon fonctionne, c'est grâce au fait que les navigateurs internet sont très permissifs, ils réussissent à afficher des pages même lorsqu'elles présentes des petites erreurs de code, ce qui ne sera pas vrai pour d'autres langages informatiques. Cependant si on veut éviter les mauvaises surprises, nous devons ajouter plus de détails dans notre code pour décrire plus précisément le contenu à afficher.

Voici un second exemple:
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>My first html page</title>
  </head>
  <body>
    Hello world!
  </body>
</html>
```

C'est un fichier html mieux formé. Il donnera exactement le même résultat et nous voyons d'autres balises :
- `<!DOCTYPE html>`:  définit la version du langage html utilisé. Ici, nous utilisons la version HTML5
- dans la balise `<html>`, nous définissons la langue : `lang="en"`. *en* signifie "english", *fr* sera utilisé pour une page en français. Nous définissons également la direction du texte `dir="ltr"`. Si on doit lire de droite à gauche, nous indiquerons "rtl": . *ltr* signifie de gauche à droite (left to right).
- nous introduisons la paire de balises `<head>`. A l'intérieur, nous pouvons ajouter des informations au sujet de notre page html. Par exemple, on peut ajouter un titre qui sera affiché par le navigateur internet dans l'onglet de navigation.

- enfin la partie à afficher se trouve à l'intérieur des balises `<body>`.

{% octicon info fill:"blue" %} Tout cette soupe doit être recommencée pour chaque page que l'on crée... Une méthode plus simple est d'utiliser un modèle tel que [html5 boilerplate](https://html5boilerplate.com). Une autre méthode (ou une méthode complémentaire) consiste à utiliser un [IDE](https://fr.wikipedia.org/wiki/Environnement_de_d%C3%A9veloppement), c'est à dire un logiciel dédié à l'écriture de code informatique. Par exemple [Atom](https://atom.io/) ou [Visual Studio Code](https://code.visualstudio.com) font gagner beaucoup de temps lorsqu'on crée un site web. Visual Studio Code est aujourd'hui largement utilisé pour les développements logiciel web en entreprise.

Nous verrons d'autres moyens permettant de se concentrer sur le contenu que nous voulons afficher et pas sur la soupe répétitive que nous venons de voir.
