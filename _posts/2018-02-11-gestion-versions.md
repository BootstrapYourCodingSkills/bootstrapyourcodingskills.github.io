---
layout: post
title:  "Gestion de versions"
date:   2018-02-11 21:17:00 +0100
image: git.png
comments: true
video: false
---

L'une des choses les plus importantes dans le développement informatique est la gestion de versions. Cela permet, entre autres, de sauvegarder son travail, de travailler en équipe et de pouvoir revenir dans le temps... et ce n'est pas tout.

* * *

La gestion de versions est un des seuls moyens pour travailler de façon sereine et en collaboration avec d'autres développeurs.

Par exemple, cela permet de revenir en arrière lorsqu'un bug est difficile à identifier et de trouver à partir de quel moment il est apparu. C'est également l'une des façon les plus efficientes pour sauvegarder son travail.

### Alors comment ça marche ?

Le principe est simple : on va regrouper les changements par un ensemble cohérent. Exemple : la même fonctionnalité, la correction d'un même bug... cet ensemble devient ce qu'on appelle une révision (ou une version).

Un changement peut être l'ajout, la suppression ou la modification d'un fichier.

On créé une révision en se basant sur la précédente, ce qui permet de créer un chemin clair des différents changements.

Sur le schéma ci-dessous, qui se lit de gauche à droite, on peut voir que `C1` est la première révision du projet. `C2` se base dessus pour apporter ses modifications et on poursuit ainsi de suite avec les suivantes.

![Révision]({{ site.url }}/content/images/commits.png)

/!\ A savoir qu'il n'y a pas de limite aux nombres de révisions qui peuvent suivre.

De cette façon on parvient à créer un historique de toutes les modifications en conservant leurs ordres d'arrivées. Il y a toujours une seule révision précédente. Grâce à ce système on peut revenir sur une ancienne révision pour avoir un état précédant ou vérifier d'où vient un bug qu'on vient de détecter.

Peu importe le langage, les outils de développement, le système d'exploitation, il est nécessaire d'avoir ce genre de logiciel.

### Dépôt

Les fichiers **versionnés** sont mis à disposition sur un **dépôt**, c'est à dire un espace géré par un logiciel de gestion de versions et souvent hébergé sur un serveur externe.

L'intérêt d'externaliser ce dépôt, que ce soit sur un serveur d'entreprise ou sur Internet (aka "le cloud")  réside dans deux choses :

- que tous les collaborateurs puissent y avoir accès
- que les données soit hébergées ailleurs que sur le seul poste du développeur.

Pour pouvoir effectuer des modifications, il faut au préalable télécharger ce dépôt qui contient l'ensemble des fichiers **versionnés**.

Par défaut, quand on récupère un dépôt, on se base sur la dernière révision créée.

### Branche

Pour faciliter le travail sur plusieurs fonctionnalités à la fois et le travail en équipe, il est possible de créer ce qu'on appelle une branche.

Une branche permet de créer un autre chemin et d'y ajouter des révisions qui n'influence pas le chemin principal.

On peut voir sur le schéma ci-dessous qu'on a deux chemins, le principal (en bleu) et un autre qu'on a appellé "*feature1*". On peut également se rendre compte que le chemin principal est une branche. qu'on nomme "master" par convention.

![Branche]({{ site.url }}/content/images/branch.png)

Pour créer une autre branche, on part d'une révision de départ. Ici on vient de la deuxième révision de la branche **master**.

De la même façon que pour la branche principale, on y ajoute des révisions, une à la fois.

Quand la fonctionnalité est terminée et validée, on peut **merger** (ou *fusionner* en français) cette branche dans la branche principale. Cette fusion va apporter toutes les révisions de la branche de développement dans la branche principale.

Cette façon de faire permet à deux personnes de travailler en parallèle sans être dérangé par le développement de l'autre ou d'éviter d'apporter des changements non testé sur la branche de livraison du produit.

C'est pour cette raison qu'on parle souvent d'arbre de révision ou d'arborescence. Chaque branche contient des noeuds (ou révision) qui viennent d'un tronc commun.

L'objectif pour les équipes est de rendre cet arbre le plus lisible possible et de veuiller à ce que tout le monde respecte le workflow des autres développeurs.

### Conflit

Qui dit gestion de versions, dit gestion de conflits.

Prenons un exemple simple, Arthur travaille sur la nouvelle page d'accueil du site internet et Hervé sur le nouveau formulaire de contact sur le même dépot. Chacun va donc travailler dans une branche pour ne pas gêner l'autre.

Pas de chance, les deux vont modifier le fichier `style.css` qui contient les styles du site internet.

Arthur va terminer son travail le premier et merger sa branche dans **master**. Quand Hervé va vouloir merger sa propre branche, il va avoir un conflit dans le fichier `style.css`.

La plupart des outils arrive à détecter -  de façon plutôt intelligente - les différences entres les deux versions d'un fichier. Hervé devra donc prendre garde à récupérer les modifications de son collègue et d'y ajouter les siennes.

Bien sûr dans la vraie vie, il peut y avoir des conflits sur plusieurs fichiers et/ou plusieurs fois dans le même fichier. C'est là, la plus grande difficulté de ce système mais ce comportement facilite grandement 

### Systèmes centralisés et décentralisés

Il existe deux grandes catégories d'outils de gestion de version.

#### Systèmes centralisés

Les premiers sont ceux qu'on appelle **centralisés**, c'est à dire qu'un seul dépôt est la référence et contient tout l'historique et les changements du projet. C'est celui-ci qui sera hébergé sur un serveur dédié à ce besoin.

C'est le cas par exemple avec des logiciels comme [CVS](https://www.nongnu.org/cvs/) ou [SVN](https://subversion.apache.org/).

#### Systèmes décentralisés

Dans l'autre cas, chaque dépôt contient l'ensemble des modifications du projet, tous les développeurs auront donc une copie complète de toutes les modifications. Un dépôt peut donc être désynchronisé par rapport à un autre mais cela permet de ne pas être dépendant d'une seule machine.

Les logiciels [Mercurial](https://www.mercurial-scm.org/) et [Git](https://git-scm.com/) sont dans cette catégorie.

### Git

Il existe bien sûr d'autres outils que je ne mentionne pas mais je voulais mettre en avant [Git](https://git-scm.com/) qui est le logiciel le plus populaire pour la gestion de versions.

Il existe énormément de services qui sont basés dessus dont le plus connus : [Github](https://github.com/) qui regroupe des milliers de bibliothèque open-source, d'exemple de code ou divers outils... On peut également citer [Bitbucket](https://bitbucket.org/product) ou [GitLab](https://about.gitlab.com/) qui permettent d'héberger ses dépôts Git et offrent d'autres services plus poussés à partir du code source.

Git est probablement le logiciel le plus complet malgré le fait qu'il soit complexe à appréhender et demande un effort particulier à prendre en main.

### Conclusion

Vous l'avez peut-être compris mais il est obligatoire d'utiliser ce genre d'outils pour créer et développer sereinement son site web, son application ou tout autre projet  informatique.

Il est indispensable de l'utiliser quand on développe à plusieurs mais aussi nécessaire quand on est développe seul grâce aux différentes garanties et la sécurité qu'il propose.

Ce n'est d'ailleurs que le début des bonnes pratiques à mettre en place pour être sûr de ne pas tout casser à révision.
