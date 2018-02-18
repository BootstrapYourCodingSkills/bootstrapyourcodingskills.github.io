---
layout: post
title:  "Gestion de version"
date:   2018-02-11 21:17:00 +0100
image: git.png
comments: true
video: false
---

L'une des choses les plus importantes dans le développement informatique est la gestion de version. Cela permet, entre autre, de sauvegarder son travail, de travailler en équipe et de pouvoir revenir dans le temps... et n'est pas tout.

* * *

La gestion de version est un domaine complet mais c'est un des seuls moyen pour travailler de façon sereine et en collaboration avec d'autres dévelopeurs.

Par exemple, cela permet de revenir en arrière lorsqu'un bug est difficile à identifier et de trouver à partir de quel moment il est apparu. Cela permet aussi de sauvegarder son travail et de travailler en équipe.

Il existe plusieurs logiciels qui permettent de mettre cette gestion de version en place.

### Comment ça marche ?

Le principe est simple : regrouper les changements par un ensemble cohérent (exemple : la même fonctionnalité, la correction d'un même bug...). Cet ensemble devient ce qu'on appelle une révision (ou une version).

Un changement peut être l'ajout, la suppression ou la modification d'un fichier.

Dès qu'on créé une révision, la suivante est basée sur celle-ci, ce qui permet de créer un chemin clair des différents changements.

Un exemple sur ce schéma :

![Révision]({{ site.url }}/content/images/commits.png)

`C1` est la première révision de ce projet. `C2` se base dessus pour apporter ses modifications et on poursuit ainsi de suite avec les suivantes. Il n'y a pas de limite aux nombres de révisions.

De cette façon on parvient à créer un historique de toutes les modifications en conservant leurs ordres d'arrivées. Il y a toujours une révision précédente, il ne peut pas y en avoir plusieurs en même temps. Grâce à ce système, on peut revenir sur une ancienne révision pour avoir un état précédant ou vérifier d'où vient un bug qu'on vient de détecter.

Peu importe le langage, les outils de développement, le système d'exploitation, il est nécessaire d'avoir ce genre d'outil.

### Dépôt

Les fichiers **versionnés** sont mis à disposition sur un **dépôt**, c'est à dire un espace géré par un logiciel de gestion de versions et souvent hébergé sur un serveur externe.

Pour pouvoir effectuer des modifications, il faut au préalable télécharger ce dépôt qui contient l'ensemble de ces fichiers.

Par défaut, quand on récupère ce dépôt, on se base sur la dernière révision faite s'il y en a déjà eu avant.

### Branche

Pour faciliter le travail sur plusieurs fonctionnalités à la fois, ou le travail en équipe, il est possible de créer ce qu'on appelle une branche.

Une branche permet de créer un autre chemin et d'y ajouter des révisions qu'on ne verra pas sur le chemin principal.

On peut voir sur ce schéma qu'on a deux chemins, le principal et un autre appellé "feature1". On s'aperçoit également que le chemin principal est également une branche. Par convention on la nomme "master".

![Branche]({{ site.url }}/content/images/branch.png)

Pour créer une autre branche, on part d'une révision de départ, ici on vient de la deuxième révision de la branche **master** et de la même façon qu'au début, on y ajoute des révisions. Quand la fonctionnalité est terminé et validée, on peut merger cette branche dans la branche principale.

Cette façon de faire permet à deux personnes de travailler en parallèle sans être déranger par le développement de l'autre.

C'est pour cette raison qu'on parle souvent d'arbre de révision ou d'arborescence. Chaque branche contient des noeuds (ou feuille, ou révision) qui viennent d'un tronc commun.

### Conflit

Qui dit gestion de version, dit gestion de conflit.

Prenons un example simple, Julien travaille sur la nouvelle page d'accueil du site internet et Hervé sur le nouveau système de connexion, toujours sur le site internet. Chacun va donc travailler dans une branche pour ne pas gêner l'autre. Pas de bol, les deux vont modifier le fichier `style.css` qui contient les styles du site internet.

Julien va terminer son travail le premier et merger sa branche dans **master**. Quand Hervé va vouloir merger sa propre branche, il va avoir un conflit dans le fichier `style.css`.

La plupart des outils arrive à détecter -  de façon plutôt intelligente - les différences entres les deux versions d'un fichier. Hervé devra donc prendre garde à récupérer les modifications de son collègue et d'y ajouter les siennes.

Bien sûr dans la vraie vie, il peut y avoir des conflits sur plusieurs fichiers et/ou plusieurs fois dans le même fichier.

### Systèmes centralisés et décentralisés

Il existe deux grandes catégories d'outils de gestion de version.

Les premiers sont ceux qu'on appelle **centralisés**, c'est à dire qu'un seul dépôt est la référence et contient tout l'historique et les changements du projet.

C'est le cas par exemple avec des logiciels comme [CVS](https://www.nongnu.org/cvs/) ou [SVN](https://subversion.apache.org/).

Dans l'autre cas, chaque dépôt contient l'ensemble des modifications du projet. Un dépôt peut donc être désynchronisé par rapport à un autre mais cela permet de ne pas être dépendant d'une seule machine.

Les logiciels [Mercurial](https://www.mercurial-scm.org/) et [Git](https://git-scm.com/) sont dans cette catégorie.

### Git

Il existe bien sûr d'autres outils que je ne mentionne pas mais je voulais mettre en avant [Git](https://git-scm.com/) qui est le logiciel le plus utilisé pour la gestion de version.

Il existe énormément de services qui sont basés dessus dont le plus connus, [Github](https://github.com/) qui regroupe des milliers de bibliothèque open-source, d'exemple de code ou des outils diverses. On peut aussi citer [Bitbucket](https://bitbucket.org/product) ou [GitLab](https://about.gitlab.com/) qui permettent d'héberger ses dépôts Git et offrent d'autres services à partir du code sources.

Git est probablement le logiciel le plus complet malgré le fait qu'il soit complexe à appréhender et demande un effort particulier à prendre en main.

