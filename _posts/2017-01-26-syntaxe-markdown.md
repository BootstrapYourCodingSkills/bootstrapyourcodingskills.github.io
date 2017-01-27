---
layout: post
title:  "La syntaxe Markdown"
date:   2017-01-26 13:13:14 +0100
image: writing2.jpg
comments: true
video: false
---

Si vous cherchez à comprendre un peu mieux ce qu'est le Markdown, je vous conseille de lire [cet article]({% post_url 2017-01-17-quest-ce-que-le-markdown %}){:target="_blank"}.

Cet article présente la syntaxe pour lire et écrire un fichier Markdown.

* * *

# Syntaxe Markdown

## Texte

<div class="title-custo">
  <p>Rendu</p>
</div>

***

Ceci est un paragraphe.

Il n'y a pas de retour à la ligne dans un paragraphe. Tout se fait dans le même contenu. Pour mettre un espace entre 2 phrases il faut faire 2 paragraphes. C'est à dire laisser une ligne vide.

L'espace entre chaque paragraphe est fixe et il n'est pas possible de le changer.

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    Ceci est un paragraphe.

    Il n'y a pas de retour à la ligne dans un paragraphe. Tout se fait dans le même contenu. Pour mettre un espace entre 2 phrases il faut faire 2 paragraphes. C'est à dire laisser une ligne vide.

    L'espace entre chaque paragraphe est fixe et il n'est pas possible de le changer

## Formattage du texte

<div class="title-custo">
  <p>Rendu</p>
</div>

***

**gras**

*italique*

***italique et gras***

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    **gras**

    *italique*

    ***italique et gras***

On peut utiliser le `_` ou `*` pour formater du texte. Les 2 signes sont équivalents.

![warning]({{ site.url }}/assets/images/warning.png) Markdown étant encore assez jeune, certains éditeurs peuvent ne pas bien interpréter l’un ou l’autre caractère.

## Titres

Le Markdown a 6 niveaux de titres. Le style des titres dépend de l'éditeur de Markdown utilisé.

<div class="title-custo">
  <p>Rendu</p>
</div>

***

# Titre 1

## Titre 2

### Titre 3

#### Titre 4

##### Titre 5

###### Titre 6

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    # Titre 1
    ## Titre 2
    ### Titre 3
    #### Titre 4
    ##### Titre 5
    ###### Titre 6

## Commentaires

<div class="title-custo">
  <p>Rendu</p>
</div>

***

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    <!--- Ceci est un commentaire -->

## Liste

<div class="title-custo">
  <p>Rendu</p>
</div>

***


1. Item ordonné 1
2. Item ordonné 2
   - sous item 1
   + sous item 2
   * sous item 3
      1. sous sous items 1
      2. sous sous items 2
      3. Pour ajouter plusieurs paragraphes dans un item, il faut commencer chaque nouveau paragraphe par autant d’espaces que le début de l'item. Cela permet de garder la numérotation de la liste pour la suite.
         Ceci est un autre paragraphe qui est décalé par plusieurs espaces pour poursuivre la liste ordonnée.
       
      4. sous sous item 4

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    1. Item ordonné 1
    2. Item ordonné 2
       - sous item 1
       + sous item 2
       * sous item 3
          1. sous sous items 1
          2. sous sous items 2
          3. Pour ajouter plusieurs paragraphes dans un item, il faut commencer chaque nouveau paragraphe par autant d’espaces que le début de l'item. Cela permet de garder la numérotation de la liste pour la suite.
          Ceci est un autre paragraphe qui est décalé par plusieurs espaces pour poursuivre la liste ordonnée.
          4. sous sous item 4

## Liens et images

<div class="title-custo">
  <p>Rendu</p>
</div>

***


[Lien vers google](http://google.fr)

[Lien vers google via une référence][google]

[google]:http://google.fr

![image](http://markdown-here.com/img/icon256.png)


<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    [Lien vers google](http://google.fr)

    [Lien vers google via une référence][google]

    [google]:http://google.fr

    ![image](http://markdown-here.com/img/icon256.png)


## Tableaux

<div class="title-custo">
  <p>Rendu</p>
</div>

***


Colonne 1 | Colonne 2 | Colonne 3
--- | --- | ---
Cellule 1-1 | Cellule 2-1 | Cellule 3-1
1 | 2 | 3

Il est possible d'aligner les caractères `|` et  `- ` pour être plus lisible dans l'édition mais un peu plus contraignant :

Colonne 1   | Colonne 2   | Colonne 3
---         | ---         | ---
Cellule 1-1 | Cellule 2-1 | Cellule 3-1
1           | 2           | 3

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    Colonne 1 | Colonne 2 | Colonne 3
    --- | --- | ---
    Cellule 1-1 | Cellule 2-1 | Cellule 3-1
    1 | 2 | 3
    
Il est possible d'aligner les caractères `|` et  `- ` pour être plus lisible dans l'édition mais un peu plus contraignant :

    Colonne 1   | Colonne 2   | Colonne 3
    ---         | ---         | ---
    Cellule 1-1 | Cellule 2-1 | Cellule 3-1
    1           | 2           | 3


# Quote et code

<div class="title-custo">
  <p>Rendu</p>
</div>

***

Il est possible de mettre en avant du texte pour le démarquer visuellement du texte standard. On utilise souvent cette syntaxe pour du code informatique ou des citations (bloc de citation ou blockquote en anglais).

> Ceci est un blockquote

`Ajout d'un bloc de code brut sur une seule ligne`

    Une autre façon de créer un bloc de code est d'ajouter 4 espaces avant.

```
On peut également ajouter du code brut sur plusieurs lignes et/ou plusieurs paragraphes via 3 ` en début et en fin de bloc. Il est recommandé de les mettre sur les ligne au-dessous et en-dessous du bloc.
```

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    > Ceci est un blockquote

    `Ajout d'un bloc de code brut sur une seule ligne`

    Une autre façon de créer un bloc de code est d'ajouter 4 espaces avant.

    ```
    On peut également ajouter du code brut sur plusieurs lignes et/ou plusieurs paragraphes via 3 ` en début et en fin de bloc. Il est recommandé de les mettre sur les ligne au-dessous et en-dessous du bloc.
    ```

## Règle horizontale

<div class="title-custo">
  <p>Rendu</p>
</div>

***

---

***

___

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    ---

    ***

    ___


## HTML

Il est possible d'ajouter du HTML si le but de l'article est de le transformer en page web. De plus, certains éditeurs sont également capable d'afficher du HTML.

<div class="title-custo">
  <p>Rendu</p>
</div>

***

<p>Ceci est un <strong>paragraphe</strong></p>

<div class="title-custo">
  <p>Texte brut</p>
</div>

***

    <p>Ceci est un <strong>paragraphe</strong></p>    
