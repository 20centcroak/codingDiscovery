---
layout: course-fr
title: Ma première page html
number: 1
---

html est un langage informatique. Il est composé de *balises* comme `<html>` et de texte.
Une fois ce *code* écrit, ce langage est compris et affiché par les navigateurs internet.

Essaie ce code très simple. Crée un fichier *index.html* et copie / colle les quelques lignes ci-dessous :
```html
<html>
  Hello world
</html>
```

Ouvre ensuite ce fichier dans ton navigateur internet et tu verras ton message s'afficher !
Comme tu peux le voir, les *balises* ne sont pas affichées, elles sont uniquement utilisées par le navigateur internet pour comprendre comment afficher le texte. Les balises vont généralement par paires et sont ouvertes et fermées comme ceci : `<html></html>`

{% octicon info fill:"blue" %} html n'est pas un langage de programmation car même si l'on peut, ntoamment grâce aux liens, interagir avec l'utilisateur, on ne peut pas exécuter des séquences complexes sans l'aide d'autres langages qu'on découvrira par la suite.

Il existe d'autres types de langages informatiques utilisant des balises. On les appelle les [langages de balisages](https://fr.wikipedia.org/wiki/Langage_de_balisage). L'un des plus connus est le format XML, on l'utilise sans le savoir quand on utilise un logiciel de [traitement de texte](https://fr.wikipedia.org/wiki/Traitement_de_texte) comme Word ou [Libre office](https://fr.libreoffice.org/). Les titres, paragraphes, images, ... sont identifiés grâce aux balises. Ces balises ne sont pas visibles dans le logiciel qui, comme le navigateur internet pour le langage html, interprète ces balises et affiche le résultat.

Les langages de balisage demandent à ouvrir et fermer les balises et à fournir de nombreux détails pour leur interprétation. On a donc également conçu des langages plus simples et moins puissants, plus proches du langage humain. C'est le cas des langages *json* ou *markdown* qui sont très utilisés. [json](https://jsoneditoronline.org/) est principalement utilisé pour échanger des données (par exemple entre 2 programmes informatiques). En voici un exemple:
```json
{  
    "élèves":
    {  
        "nom":      "Dupont",   
        "prénom":   "Marcel",   
        "age":      12  
    },
    {  
        "nom":      "Durant",   
        "prénom":   "Gertrude",   
        "age":      14  
    }
}  
```

Le langage [markdown](https://stackedit.io/) permet quant à lui de mettre en forme du texte. Il est très utilisé dans les wiki ou les blogs pour écrire rapidement un texte avec de la mise en page. En voici un exemple:
```markdown
# titre
## sous-titres
[lien](https://20centcroak.github.io/codingDiscovery)
```
et voici, une fois interprété ce qu'il devient :
> # titre
>## sous-titres
>[lien](https://20centcroak.github.io/codingDiscovery)
