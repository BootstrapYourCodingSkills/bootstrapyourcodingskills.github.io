---
layout: post
title:  "Qu'est-ce que le Markdown ?"
date:   2017-01-17 13:13:14 +0100
image: markdown.png
comments: true
video: false
---

Vous créez des fichiers Word pour tous vos documents ? Vous passez plus de temps sur le style que sur le contenu ? Vous n'avez pas Word parce que c'est cher, gourmands en ressource ou que tout le monde ne peut pas lire le format ? Alors vous faites des documents en texte brut ou en RTF ?

Si je vous disais qu'il existe un format de fichier qui soit lisible sur n'importe quel système d'exploitation, gratuit et complet.

Vous l'aurez compris, je parle du Markdown.

* * *

Markdown est une syntaxe, un format de fichier qui permet de créer des fichiers complets d'une manière relativement simple. On peut formater le texte (titre, gras, italique...), ajouter des images ou des liens hypertexte. Le tout avec un format léger, lisible et facilement exportable vers du PDF ou une page HTML.

# Encore au début 

Markdown est une technologie assez jeune, il n'existe pas d'outils qui acceptent toutes les syntaxes possibles. La communauté utilise de plus en plus le terme Markdown pour tout ce qui concerne le `text-to-HTML`, ce qui complique les choses pour avoir un outil standard et des spécifications précises.

On étudiera ici seulement la syntaxe "original" du Markdown, celle qui est utilitée sur ce site web.


# Avantages/Inconvénients du Markdown

## Avantages

- **Format universel** N'importe quel éditeur de texte peut lire un fichier Markdown. C'est du texte avec une syntaxe particulière. Il existe également des éditeurs Markdown pour afficher le rendu final. On en trouve sur toutes les plateformes (Windows, Mac, Android, iOS...). La syntaxe est la même ou presque, on voit ça dans les inconvénients.
- **Formattage du texte** Titre, gras, italique, image, lien hypertexte... On peut faire beaucoup de choses simplement.
- **Léger** Il est extrément léger ce qui facilite le partage.
- **Exportable** On peut facilement générer du HTML ou du PDF à partir d'un fichier Markdown.
- **Web** C'est une syntaxe très utilisée pour créer des pages web :
   - Plus sécurisé, après tout ce n'est que du texte.
   - Séparer la partie visuelle du contenu. Markdown étant le contenu.
   - Facile et agréable à utiliser.


## Inconvénients

- **Apprentissage du langage** Markdown est une syntaxe qui demande un petit effort d'apprentissage.
- **Outil** Pour afficher un rendu "final" d'un fichier Markdown, il vous faut télécharger un éditeur Markdown.
- **Limite** Le style du texte est limité : pas de couleur, pas de gestion d'interligne... On peut seulement changer ces paramètres à l'export (PDF ou HTML par exemple) en fonction de l'outil qu'on utilise.
- **Format universel** En fait ce n'est pas si universel. Chaque éditeur / outil utilisant le Markdown acceptera ou non certaines syntaxes... C'est un problème de jeunesse qui devrait être réglé dans les nouvelles versions de ces outils.

# Cas d'utilisation

1. Documentations / Instructions

    A l'instar de [Github](https://github.com/){:target="_blank"}  beaucoup de sites utilisent Markdown comme base pour créer des fichiers de documentation ou d'instruction (README, INSTALL...).
   
   L'une des raisons pour lequel Markdown est beaucoup utilisé est la création de documentation, technique ou non. Cela permet d'avoir un format simple, presque autant que du texte brut et de pouvoir le mettre en forme très facilement.

1. Ecriture
 
   Markdown nous permet d'être concentré sur ce qu'on écrit sans être perturbé par une barre d'outil ou des dizaines de boutons. Tout se fait au clavier. De plus on ne se soucie plus du style du document, on ne peut pas le changer. Cela facilite grandement la tâche de création de contenu, on reste concentré sur l'écriture.

1. Web

   Le Markdown est aussi utilisé pour créer le contenu des sites Internet et de séparer la partie visuelle (HTML/CSS) du texte brut.
   
   Il existe aussi des sites "statiques" dont le contenu ne change pas en fonction de l'utilisateur. C'est à dire qu'il n'y a pas de gestion d'utilisateur, pas d'administration, pas de base de données... Un site extrêmement simple et rapide. Le coeur de ces sites statiques reposent sur des fichiers comme le Markdown qui composent l'ensemble des pages web.

   Ce blog est un site statique et cet article (ainsi que tous les autres) a été généré à partir d'un fichier Markdown.
   
   Beaucoup de sites statiques utilisent le Markdown pour générer les pages web.


# Exemple

Voici un exemple d'un fichier Markdown:

---

####Le fichier brut

---

    # Mon titre

    ### Mon titre 2

    Ceci est le corps de texte.

    Quelques exemples de format du texte: **gras**, _italique_.

    Une image:
    ![Image]({{ site.url }}/content/images/flat-images.jpg)

---

####Le rendu
---

# Mon titre

### Mon titre 2

Ceci est le corps de texte.

Quelques exemples de format du texte: **gras**, _italique_.

Une image:
![Image]({{ site.url }}/content/images/flat-image.jpg)


---

## Extensions

Il existe plusieurs (trop) extensions de fichiers pour le Markdown:

- .md
- .markdown
- .mdown
- .mkd
- ...

Personnellement j'utilise `.md` parce que je sais qu'il est compris sur toutes les plateformes.


# Conclusion

Markdown est un langage à balise qui demande un effort d'apprentissage au début mais devient très vite simple à utiliser. A savoir que cette connaissance n'est pas nécessaire pour lire un fichier, seulement pour l'écrire. Il existe des outils pour afficher le rendu final d'un fichier Markdown. On peut aussi l'exporter en PDF ou en page web très facilement.

Une fois la syntaxe comprise, vous ne passerez pas des heures à styliser votre document. Vous vous focaliserez sur le contenu et c'est pour ça qu'il est très populaire. On se rend très vite compte qu'il est beaucoup plus simple et rapide d'écrire quand on n'a pas des dizaines de boutons à notre disposition, quand l'outil nous propose seulement une page noir  (ou blanche) pour pouvoir écrire, quand tout se fait au clavier et que les doigts ne touchent plus la souris.

Il est aussi très simple à utiliser dans un site web ou dans un système d'information. La syntaxe est simple et il est très facile de faire ce qu'on en veut via un programme.

J'écrirai un autre post pour apprendre à l'utiliser.