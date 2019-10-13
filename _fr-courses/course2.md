---
layout: course-fr
title: Créer des liens
number: 2
---

La fonctionnalité la plus intéressante du langage html, et qui l'a popularisé, est la possibilité d'ajouter des liens vers d'autres sites ou d'autres sections du même site. C'est cela qui crée la *toile* (web en anglais).

 Par exemple, si vous voulez qu'un visiteur de votre site web puisse cliquer pour ouvrir la page *Qwant*, il suffit d'ajouter un lien vers cette page. Ce lien s'appelle *url*. On ajoute ce lien grâce à la balise `<a>` comme ceci :
 ```
 <a href="https://www.qwant.com/">Qwant</a>
 ```

Si vous souhaitez diriger votre visiteur vers une autre page du site, vous pouvez utiliser un lien *relatif* (il ne comporte pas le début de l'url *http://www. ...*)
```
<a href="exemple.html">voir l'exemple</a>
```

Il est également possible d'ouvrir le lien dans un nouvel onglet de navigation pour que le visiteur ne quitte pas votre site définitivement. Il faut alors utiliser le mot clef *target* dans la balise *<a>*:
```
<a href="https://www.qwant.com/" target="_blank">Qwant</a>
```
