---
layout: course-fr
title: Mise en page
number: 2.1
---

Si on prend l'exemple d'un logiciel de traitement de textes comme *Word* ou *libre Office Writer*, la mise en page s'appuie sur des titres et des paragraphes essentiellement.
Voyons donc de nouvelles balises qui définissent ces sections de document:
- `<p>` definit un paragraphe
- `<h1>`,  `<h2>`, ... definissent differents niveaux de titre.

On pourra vérfier que revenir à la ligne dans un fichier html n'impliquera pas de revenir à la ligne dans le navigateur.
Par exemple :
```
<body>
  Hello
  World
  !
</body>
```
s'affichera comme ceci :
>Hello world !

Si à présent on écrit un document en utilisant les balises `<p>` et `<h>`, on obtient une mise en page satisfaisante:

```html
<body>
  <h1>Hello world!</h1>
  <h2>I'm a subtitle !</h2>
  <p>this is the first line</p>
  <p>this is the second line</p>
</body>
```

et voici le résultat:

# Hello world!
## I'm a subtitle !
this is the first line  
this is the second line
