---
layout: post
title:  "Qu'est-ce que le Markdown"
date:   2016-11-30 13:13:14 +0100
image: cloud.jpg
comments: true
video: false
---

Si je vous disais qu'il existe un format de fichier qui soit lisible sur n'importe quel système d'exploitation, gratuit, complet et universel ?

Je parle bien du Markdown.

* * *

Vous créer des fichiers Word pour tous vos documents ? Vous passez plus de temps sur le style que sur le contenu ?

Vous n'avez pas Word parce que c'est cher, gourmand en ressource du PC ou que tout le monde ne peut pas lire le format ? Alors vous faites des documents texte brute ou du RTF ?

Arrêtez tout ! Il existe maintenant une solution pour vos problème.

Markdown est un langage à balise qui permet de créer des fichiers complet puisqu'on peut formatter le texte (titre, gras, italique...), ajouter des images ou des liens hypertext. Le tout avec un format léger, facilement exportable vers PDF ou page HTML et disposant d'outil pour l'utiliser sur toutes les plateformes.


# Avantages/Inconvénients du Markdown

## Avantages

- Format universel: Il existe des outils sur toutes les plateformes (Windows, Mac, Android, iOS...) pour lire ou écrire du Markdown. La syntaxe est exactement la même.
- Complet : Titre, gras, italique, image, lien hypertext... On peut faire beaucoup de chose simplement.
- Meilleur choix entre du texte brut et Word
- Léger : Il est extrément léger ce qui facilite le partage
- Génération HTML ou PDF


## Inconvénients

- Apprentissage du langage: Markdown est un langage ce qui demande de faire un petit effort pour comprendre le langage
- Outil: Il vous faut télécharger le bon outil sur votre plateforme pour afficher le rendu final du document
- Limite: Le style du texte est limité : pas de couleur, l'espace entre les lignes est toujours le même...

# Cas d'utilisation

1. Documentation

  L'une des raisons pour lequel Markdown est beaucoup utilisé est la création de documentation, technique ou non. Cela permet d'avoir un format simple, presque autant que du texte brut et de pouvoir le mettre en forme très facilement.

2. Ecriture
 
  De plus en plus de personnes utilisent le Markdown pour écrire parce qu'on peut rajouter des titres et du formattage (gras, italique...) mais sans ce soucier de la présentation finale comme sur un document Word.  

3. Instructions
   
   A l'instar de [Github](https://github.com/){:target="_blank"} beaucoup de site utilise Markdown comme base pour créer des fichiers de documentation ou d'instruction (README, INSTALL) qui per 


4. Site statique

   Un site statique est un site dont le contenu ne change pas en fonction de l'utilisateur. C'est à dire qu'il n'y a pas de gestion d'utilisateur, pas d'administration, pas de base de données... Un site extrêmement simple et rapide.
   
   Beaucoup de sites statiques utilisent le Markdown pour générer les pages web.


# Exemple

Voici un exemple d'un fichier Markdown:

Le fichier brute:
```markdown
# Mon titre

## Mon titre 2

Ceci est le corps de texte.

Quelques exemples de format du texte: *gras*, _italique_.

Une image:
![Image bateau]({{ site.url }}/content/images/client-server.svg)
```

Le rendu:


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

Markdown est un langage à balise qui demande un effort d'apprentissage au début mais devient très vite simple à utiliser. A savoir que cette connaissance n'est pas nécessaire pour lire un fichier, seulement pour l'écrire. 

Il existe des outils pour afficher le rendu final d'un fichier markdown. On peut aussi l'exporter en PDF ou en page web très facilement.

Vous ne le savez peut-être pas mais ce blog est un site statique et cet article (ainsi que tous les autres) a été généré à partir d'un fichier Markdown.
