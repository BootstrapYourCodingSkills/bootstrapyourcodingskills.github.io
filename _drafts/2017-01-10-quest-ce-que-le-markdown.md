---
layout: post
title:  "Qu'est-ce que le Markdown"
date:   2016-11-30 13:13:14 +0100
image: cloud.jpg
comments: true
video: false
---

Si je vous disais qu'il existe un format de fichier qui soit lisible sur n'importe quel système d'exploitation, gratuit, complet et (presque) universel ?

Je parle du Markdown.

* * *

Vous créer des fichiers Word pour tous vos documents ? Vous passez plus de temps sur le style que sur le contenu ?

Vous n'avez pas Word parce que c'est cher, gourmand en ressource ou que tout le monde ne peut pas lire le format ? Alors vous faites des documents en texte brute ou en RTF ?

Markdown est une syntaxe, un format de fichier qui permet de créer des fichiers complet d'une manière relativement simple. On peut formatter le texte (titre, gras, italique...), ajouter des images ou des liens hypertext. Le tout avec un format léger, lisible, facilement exportable vers PDF ou une page HTML.


# Avantages/Inconvénients du Markdown

## Avantages

- Format universel : N'importe quel éditeur de texte peut lire un fichier Markdown. Il existe également des éditeurs Markdown pour afficher un rendu final sur toutes les plateformes (Windows, Mac, Android, iOS...). La syntaxe est la même ou presque;
- Complet : Titre, gras, italique, image, lien hypertext... On peut faire beaucoup de chose simplement.
- Meilleur choix entre du texte brut et Word
- Léger : Il est extrément léger ce qui facilite le partage
- Génération simplifié vers du HTML ou du PDF

## Inconvénients

- Apprentissage du langage: Markdown est un langage qui demande de faire un effort au démarrage pour le comprendre.
- Outil : Il vous faut télécharger un éditeur Markdown sur votre plateforme pour afficher le rendu final du document.
- Limite: Le style du texte est limité : pas de couleur, pas de gestion d'interligne... On peut seulement changer ces paramètres à l'export en fonction de l'outil qu'on utilise.

# Cas d'utilisation

1. Documentation

  L'une des raisons pour lequel Markdown est beaucoup utilisé est la création de documentation, technique ou non. Cela permet d'avoir un format simple, presque autant que du texte brut et de pouvoir le mettre en forme très facilement. On peut générer un site web à partir des fichiers markdown pour permettre à tout le monde d'y accéder.

2. Ecriture
 
  L'un des avantages de Markdown est qu'on est concentré sur ce qu'on écrit. On n'est plus perturbé par une barre d'outil, des dizaines de boutons. Tout se fait au clavier et on reste concentré sur notre tâche. De plus on ne se soucie plus du style du document, on ne peut pas le changer.


3. Instructions
   
   A l'instar de [Github](https://github.com/){:target="_blank"} beaucoup de site utilise Markdown comme base pour créer des fichiers de documentation ou d'instruction (README, INSTALL) qui per 


4. Site statique

   Un site statique est un site dont le contenu ne change pas en fonction de l'utilisateur. C'est à dire qu'il n'y a pas de gestion d'utilisateur, pas d'administration, pas de base de données... Un site extrêmement simple et rapide.

   Ce blog est un site statique et cet article (ainsi que tous les autres) a été généré à partir d'un fichier Markdown.
   
   Beaucoup de sites statiques utilisent le Markdown pour générer les pages web.


# Exemple

Voici un exemple d'un fichier Markdown:


---
Le fichier brute:

---

```markdown
# Mon titre

## Mon titre 2

Ceci est le corps de texte.

Quelques exemples de format du texte: *gras*, _italique_.

Une image:
![Image bateau]({{ site.url }}/content/images/client-server.svg)
```
---
Le rendu:

----

# Mon titre

## Mon titre 2

Ceci est le corps de texte.

Quelques exemples de format du texte: *gras*, _italique_.

Une image:
![Image bateau]({{ site.url }}/content/images/client-server.svg)


---

## Extensions

Il existe plusieurs (trop) extension de fichier pour le Markdown:

- .md
- .markdown
- .mdown
- .mkd

Personnellement j'utilise `.md` parce que je sais qu'il est compris sur toutes les plateformes.


# Conclusion

Markdown est un langage à balise qui demande un effort d'apprentissage au début mais devient très vite simple à utiliser. A savoir que cette connaissance n'est pas nécessaire pour lire un fichier, seulement pour l'écrire. Il existe des outils pour afficher le rendu final d'un fichier markdown. On peut aussi l'exporter en PDF ou en page web très facilement.

Une fois le langage compris, vous ne passerez pas des heures à styliser votre document. Vous vous focaliserez sur le contenu. Et c'est pour ça que tout le monde l'adore. On se rend très vite compte qu'il est beaucoup plus simple et rapide d'écrire quand on n'a pas des dizaines de boutons à notre disposition, quand l'outil nous propose seulement une page noir (ou blanche) pour pouvoir écrire, quand se fait au clavier et que les doigts ne touchent plus la souris.


