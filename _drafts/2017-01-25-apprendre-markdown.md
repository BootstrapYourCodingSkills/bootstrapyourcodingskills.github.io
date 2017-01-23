---
layout: post
title:  "Apprendre le Markdown"
date:   2017-01-25 13:13:14 +0100
image: writing2.jpg
comments: true
video: false
---

Si vous chercher à comprendre un peu mieux ce qu'est le Markdown, je vous conseille de lire [cet article]({% post_url 2017-01-17-quest-ce-que-le-markdown %}){:target="_blank"}. Cet article présente la syntaxe du Markdown.

* * *

# Syntaxe Markdown

## Texte

<div class="title-custo">
  <p>Rendu</p>
</div>
***


Ceci est un paragraphe.

Il n'y a pas de retour à la ligne dans un paragraphe. Tout se fait dans le même contenu. Pour mettre un espace entre 2 phrases il faut faire 2 paragraphes. C'est à dire laisser une ligne vide entre 2 morceaux de texte.

L'espace entre chaque paragraphe est fixe et il n'est possible de le changer.

<div class="title-custo">
  <p>Texte brut</p>
</div>
***

    Ceci est un paragraphe.

    Il n'y a pas de retour à la ligne dans un paragraphe. Tout se fait dans le même contenu. Pour mettre un espace entre 2 phrases il faut faire 2 paragraphes. C'est à dire laisser une ligne vide entre 2 morceaux de texte.

    L'espace entre chaque paragraphe est fixe et il n'est possible de le changer

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

On peut utiliser le `_` ou `*` pour formatter du texte. Les 2 signes sont équivalents

/!\ Certains éditeurs ne les gèrent pas de la même façon et certains signes ne sont pas utilisables.


## Titres

Le Markdown a 6 niveaux de titres. Le style des titres dépend de l'éditeur/l'interpreteur de Markdown utilisé.

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
      3. ...

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
          3. ...

## Liens et images

<div class="title-custo">
  <p>Rendu</p>
</div>
***


[Lien vers google](http://google.fr)

[Lien vers google via référence][google]

[google]:http://google.fr

![image](http://markdown-here.com/img/icon256.png)


<div class="title-custo">
  <p>Texte brut</p>
</div>
***

    [Lien vers google](http://google.fr)

    [Lien vers google via référence][google]

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

ou aligné pour être plus lisible dans le texte brut mais un peu plus contraignant :

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

    
Ou aligné pour être plus lisible dans le texte brut mais un peu plus contraignant :

    Colonne 1   | Colonne 2   | Colonne 3
    ---         | ---         | ---
    Cellule 1-1 | Cellule 2-1 | Cellule 3-1
    1           | 2           | 3


# Quote et code

<div class="title-custo">
  <p>Rendu</p>
</div>
***


> Ceci est un blockquote

`Ajout d'un bloc de code brut sur une seule ligne`

```
Ajout de code brut sur une plusieurs lignes. On peut utiliser cette syntaxe pour plusieurs chose mais la plus répendue est l'ajout d'un bloc de code.
```

<div class="title-custo">
  <p>Texte brut</p>
</div>
***

    > Ceci est un blockquote

    `Ajout d'un bloc de code brut sur une seule ligne`

    ```
    Ajout de code brut sur une plusieurs lignes. On peut utiliser cette syntaxe pour plusieurs chose mais la plus répandue est l'ajout d'un bloc de code.
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

Il est possible du HTML si le but de l'article est de le transformer en page web. Certains outils sont également capable d'afficher du HTML.

<div class="title-custo">
  <p>Rendu</p>
</div>


<p>Ceci est un <strong>paragraphe</strong></p>

<div class="title-custo">
  <p>Texte brut</p>
</div>
***

    <p>Ceci est un <strong>paragraphe</strong></p>    
