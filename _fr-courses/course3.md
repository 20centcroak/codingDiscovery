---
layout: course-fr
title: Ajouter des styles
number: 3
---

Bien, maintenant nous savons créer une page web et ajouter des liens. Mais franchement le résultat est très moche.
Si on regarde le résultat du cours "Créer des liens", on voit que les liens sont tous sur la même ligne même si dans notre code on est passé à la ligne. De plus le texte est noir, les liens sont soulignés et bleus comme dans l'internet des années 1990 et le fond est blanc.

Il est donc temps de présenter un autre langage informatique, complémentaire du html : les css (cascade sthyle sheets ou feuilles de style en cascade)

Css ets un fichier séparé du code html qui va indiquer le style à appliquer aux différents éléments de la page (balises, classes, id).
Ma&is pourquoi utiliser un fichier séparé. Pour de nombreuses raisons mais si on ne devait en citer que 2, les voici:
- définir des styles indépendamment de la page permet de réutiliser ces styles pour toutes les autres pages du site web. Cela permet donc d'obtenir une jolie homogénéité sur le design du site, ainsi que de gagner beaucoup de temps.
- lorqu'un site web nécessite d'être rafraichi avec un look plus moderne ou si on veut que l'utilisateur puisse choisir le thème à appliquer au site, il suffit de définir un nouveau jeu de fichiers css à appliquer et tout le contenu est re-stylé.

Cependant css ne serait rien sans quelques nouvelles balises :
- `<p>` definit un paragraphe
- `<h1>`,  `<h2>`, ... definissent differents niveaux de titre.

Nous pouvons dès lors ajouter des styles à notre page :
```
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>add style!</title>
    <link rel="stylesheet" href="css/styles.css">
  </head>
  <body>
    <h1>We add styles!</h1>
    <p>Here is a list of links:<p>
    <p><a href="https://github.com/20centcroak/childrencourses">visit children courses</a></p>
    <p><a href="sample1.html">see sample1</a></p>
    <p><a href="https://github.com/20centcroak/childrencourses" target="_blank">visit children courses in a separate tag</a></p>
  </body>
</html>
```

et voici le contenu du fichier styles.css :
```
body {
  background-color: DarkTurquoise ;
  font-family: Georgia, serif;
}
h1{
  color: Blue;
}
p {
  color: Teal;
  padding-left: 20px;
}
a{
  color: MidnightBlue;
  text-decoration: none;
}
a:hover {
  color: DarkOrange;
}
```

css and tags should be seen like russian dolls. if `<a>` is inside a `<p>` tag whit itself is inside a `<body>` tag, then all styles defined in the body section of css file apply to p and a while not overwriten. In our example, background-color is not overwriten, then it applies to all elements inside `<body>`. Text color is defined in the p section but it overwriten in the a section, then text color in all <a> sections of the html document is MidnightBlue while text color in p sections is Teal.

Note that we used the syntax `a:hover` that applies to all <a> tag when mouse pointer is over this element. It results in a color change when the mouse points on a link.

When no style is defined like in our previous tries, then the browser styles elements with a standard HTML1.0 ugly design.
