---
layout: post
title:  "Comment fonctionne un site internet ?"
date:   2016-11-30 13:13:14 +0100
image: cloud.jpg
comments: true
video: false
---

Avant de commencer à créer son site, il est important de comprendre comment ça fonctionne. Ne vous inquiétez pas c'est assez simple. Je vous explique tout ça:

* * *

En informatique on évoque souvent les termes client/serveur. Pour un site internet, le terme client désigne le navigateur et tout ce qui est exécuté dessus. Quand au serveur, il reçoit des requêtes du client et y répond. 

Voici un exemple:

![Client serveur]({{ site.url }}/content/images/client-server.svg)

Partons d'un exemple, vous souhaitez vous identifier sur un site internet via l'habituel email/mot de passe.

- Vous saisissez une URL dans votre navigateur web. Cela va envoyer une requête au serveur web. Celui-ci va traiter la requête et renvoyer la réponse au client, c’est-à-dire le navigateur, sous forme de code HTML.
- (1) Le navigateur (client) interprète le HTML et affiche donc la page avec les 2 champs de saisie de texte plus un bouton pour se connecter.
- Quand vous cliquez sur le bouton, le client va envoyer une autre requête au serveur en lui transmettant votre email/mot de passe.
- (2) Le serveur reçoit ces informations et vérifie que le mot de passe correspond bien à l'adresse email.
- Le serveur peut par exemple vérifier que ces informations existent dans une base de données. La base de données est une façon très efficace d'enregistrer des données, comme par exemple les utilisateurs d'un site.
- Il peut également appeler 1 ou plusieurs autres serveurs pour utiliser d'autres services, par exemple envoyer un email, créer un post Facebook ou autre...
- Une fois que le couple email/mot de passe a été retrouvé dans la bases de données, le serveur renvoit une réponse au client, en disant, "OK laisse le rentrer" et va alors vous rediriger vers la page de votre compte. On revient à l'étape 1.

---

Concrètement comment ça fonctionne. Reprenons notre exemple, pas à pas.

1. **Client** - HTML
   
    On utilise le HTML (aka HyperText Markup Language) pour structurer la page. Voici un exemple le plus simple possible d'un formulaire de connexion.
    
    Quand on clique sur `Connexion`, on va envoyer une requête au serveur. Dans notre test ci-dessous, il n'y a pas de serveur, donc il ne se passera rien.
 
   ![Exemple]({{ site.url }}/content/images/fonctionnement-site-1.png)
    
   [Visualiser](http://htmlpreview.github.io/?https://github.com/BootstrapYourCodingSkills/first-website/blob/master/index.html)   
   [Code source](https://github.com/BootstrapYourCodingSkills/first-website)
   
   Pour créer la même page chez vous, c'est très simple. Créer un fichier texte sur votre ordinateur et renommer le en `index.html`. Ouvrez ce fichier dans un éditeur de texte (bloc note, TextEdit...). Ensuite recopiez le code source (cf lien "Code source" ci-dessus et cliquez sur le lien `index.html`). Collez le contenu (le texte qui commence par `<html>` et termine par `</html>`) dans votre fichier. Une fois le copié/collé effectué, ouvrez ce fichier dans votre navigateur. Et voila, votre 1ère page web !
   
1. **Client** - HTML + CSS

   On peut aussi ajouter du CSS (aka Cascading Style Sheets) pour rajouter un peu de couleur et mettre en forme toute la page. Le CSS est un ensemble de règles qu'on va appliquer sur le HTML pour le modifier. Dans l'exemple ci-dessous, le HTML est très légéremment modifié mais on a surtout rajouté un fichier `style.css` qui va se charger d'appliquer les règles de style.


   ![Exemple]({{ site.url }}/content/images/fonctionnement-site-2.png)
   
   [Visualiser](http://htmlpreview.github.io/?https://github.com/BootstrapYourCodingSkills/second-website/blob/master/index.html)   
   [Code source](https://github.com/BootstrapYourCodingSkills/second-website)

   
1. **Client** - HTML + CSS + Javascript

   En plus de ces 2 technologies on emploie également du Javascript. Il s'agit d'un langage qu'on utilise pour modifier en temps réel la page. Ici on s'en sert pour vérifier que les champs texte ne sont pas vides avant l'envoi au serveur.
   
   [Visualiser](http://htmlpreview.github.io/?https://github.com/BootstrapYourCodingSkills/third-website/blob/master/index.html)  
   [Code source](https://github.com/BootstrapYourCodingSkills/third-website)


1. **Serveur web**

   Un serveur web est un programme qui va attendre une requête d'un client et qui va se charger de la traiter et de renvoyer une réponse. On se base sur l'URL pour savoir qui et comment on va gérer la page.  
   Il existe beaucoup de langages "serveur" qu'on peut utiliser pour cette tâche. Le plus connu / utilisé est probablement le PHP mais on retrouve aussi Java, Ruby, Python, Javascript (qui est aussi un langage client) et beaucoup d'autres...

Si vous souhaitez vous exercer, il existe de nombreux tutorials sur Internet comme [OpenClassrooms](https://openclassrooms.com/) qui propose des cours sur de nombreux sujets lié au développement informatique.
