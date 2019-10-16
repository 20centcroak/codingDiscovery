---
layout: course-fr
title: Ajouter des styles
number: 3
---

Bien, maintenant nous savons créer une page web et ajouter des liens. Mais franchement le résultat est très moche.
Si on regarde le résultat du cours "Créer des liens", on voit que le texte est noir, les liens sont soulignés et bleus comme dans l'internet des années 1990 et le fond est blanc.

Il est donc temps de présenter un autre langage informatique, complémentaire du html : les css (cascade sthyle sheets ou feuilles de style en cascade)

Css est un fichier séparé du code html qui va indiquer le style à appliquer aux différents éléments de la page (balises, classes, id).
Mais pourquoi utiliser un fichier séparé. Pour de nombreuses raisons sur lesquelles on reviendra mais si on ne devait en citer que 3, les voici:
- définir des styles indépendamment de la page permet de réutiliser ces styles pour toutes les autres pages du site web. Cela permet donc d'obtenir une jolie homogénéité sur le design du site, ainsi que de gagner beaucoup de temps.
- lorqu'un site web nécessite d'être rafraichi avec un look plus moderne ou si on veut que l'utilisateur puisse choisir le thème à appliquer au site, il suffit de définir un nouveau jeu de fichiers css à appliquer et tout le contenu est re-stylé.
- en séparant le style et la mise en forme, on peut faire travailler 2 personnes spécialistes dans leur domaine de manière indépendante. L'une travailler sur le fichier html est décrivant la structure de la page et le second travaille sur l'aspect graphique : le choix des couleurs, la [police](https://fr.wikipedia.org/wiki/Police_d%27%C3%A9criture) de caractère et sa taille, ...

Nous pouvons ajouter des styles à notre page en définissant le fichier à utiliser entre les balises `<head>` :
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

Les balise doivent être vues comme des poupées russes. Si on définit un lien avec la balise `<a>` qui est contenu dans un paragraphe défini avec la balise `<p>`, lui-même contenu dans la balise `<body>`, alors tous les styles définis dans le fichier css pour la balise `<body>` vont s'appliquer à la balise `<p>` puis à la balise `<a>` tant qu'ils ne sont pas redéfinis dans ces balises.
Dans l'exemple ci-dessus, la couleur du fond `background-color` est définie pour la balise `<body>` et n'est pas redéfinie dans les autres balises, elle va donc s'appliquer pour toutes les balises contenues dans `<body>`. La couleur du texte `color` est définie pour la balise <p> et s'applique donc pour cette balise, mais elle ne s'apliquera pas aux liens, même s'ils sont contenus dans la balise `<p>` car une autre couleur est définie pour la balise `<a>`.

{% octicon info fill:"blue" %}
on a utilisé une syntaxe un peu spéciale  `a:hover`. On pourrait traduire *hover* par *survol*. Ce style s'applique aux balises `<a>` lorsque le pointeur de la souris survolle le lien. Dans notre cas, la couleur du lien change quand on passe la souris sur un lien.

{% octicon info fill:"blue" %} Lorsqu'aucun style n'est défini, alors le navigateur applique des styles par défaut.

{% octicon info fill:"blue" %} la balise `<link>` permet d'indiquer la feuille de style à utiliser. On utilise, comme pour les liens le mot clef `href` pour fournir le nom et l'emplacement du fichier. `css/styles.css` signifie : à partir de l'emplacement de la page affichée, tu vas dans le dossier *css* et tu charges le fichier *styles.css*. C'est ce qu'on appelle un chemin *relatif*: il est relatif à l'emplacement du fichier qui y fait réfrérence. On aurait pu également écrire `/css/styles.css`. Cela signifie : à partir du répertoire principal du site web, tu vas dans le dossier *css* et tu charges le fichier *styles.css*. C'est ce qu'on appelle un chemin *absolu*: quelque soit l'emplacement du fichier en cours, on va chercher la feuille de styles toujours au même endroit.
