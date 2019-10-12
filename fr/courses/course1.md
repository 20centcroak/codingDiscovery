---
layout: course-fr
title: Ma première page html
number: 1
next: course2
---

html est un langage informatique. Il est composé de *balises* comme `<html>` et de texte.
Une fois ce *code* écrit, ce langage est compris et affiché par les navigateurs internet.

Essaie ce code très simple. Crée un fichier *index.html* et copie et colle les quelques lignes ci-dessous :
```html
<html>
  Hello world
</html>
```

Ouvre ensuite ce fichier dans ton navigateur internet et tu verras ton message s'afficher !
Comme tu peux le voir, les *balises* ne sont pas affichées, elles sont uniquement utilisées par le navigateur internet pour comprendre comment afficher le texte. Les balises vont généralement par paires et sont ouvertes et fermées comme ceci : `<html></html>`

Même si cet exemple simple fonctionne, c'est grâce au fait que les navigateurs internet sont très permissifs, ils réussissent à afficher des pages même lorsqu'elles présentes des petites erreurs de code, ce qui ne sera pas vrai pour d'autres langages informatiques. Cependant si on veut éviter les mauvaises surprises, nous devons ajouter plus de détails dans notre code pour décrire plus précisément le contenu à afficher.

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
- nous introduisons la paire de balises `<head>`. A l'intérieur, nous pouvons ajouter des informations au sujet de notre page html. Par exemple, on peut ajouter un titre qui sera affiché par le navigateur internet dans l'onglet de navigation comme on le voit sur l'image suivante :

![page with title]({{ page.githubRepo}}/assets/images/htmlpart1Title.png)

- endin la partie à afficher se trouve à l'intérieur des balises `<body>`.

Tout cette soupe doit être recommencée pour chaque page que l'on crée... Une méthode plus simple est d'utiliser un modèle tel que [html5 boilerplate](https://html5boilerplate.com). Une autre méthode (ouune méthode complémentaire) consiste à utiliser un IDE, c'est à dire un logiciel dédié à l'écriture de code informatique. Par exemple [Atom](https://atom.io/) ou [Visual Studio Code](https://code.visualstudio.com) font gagner beaucoup de temps lorsqu'on crée un site web.

Nous verrons d'autres moyens permettant de se concentrer sur le contenu que nous voulons afficher et pas sur la soupe répétitive que nous venons de voir.
