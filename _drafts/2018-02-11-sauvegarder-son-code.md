---
layout: post
title:  "Gestion de version"
date:   2018-02-11 21:17:00 +0100
image: code.jpg
comments: true
video: false
---

L'une des choses les plus importantes dans le développement informatique est la gestion de version. Cela permet, entre autre, de sauvegarder son travail et de pouvoir revenir dans le temps. On va également voir que ça sert à beaucoup d'autres choses.

* * *

La gestion de version est un domaine complet mais c'est un des seuls moyen pour travailler de façon sereine et en collaboration avec d'autres dévelopeurs.

Cela permet, par exemple lorsqu'un bug intervient et qu'il est difficile de l'identifier, il est possible de revenir en arrière sur son travail et de trouver à partir de quel moment il est apparu. Cela permet aussi de sauvegarder son travail et de travailler en équipe.

### Comment ça marche ?

Le principe est simple : regrouper les changements par un ensemble cohérent (exemple: la même fonctionnalité, la correction d'un même bug...). Cet ensemble devient une révision (ou version).

Un changement peut être l'ajout, la suppression ou la modification d'un fichier du projet.

Dès qu'on créé une révision, la suivante est basée sur celle-ci, ce qui permet de créer un chemin clair des différents changements.

Un exemple sur ce schéma :

![Révision]({{ site.url }}/content/images/commits.png)

`C1` est la première révision de ce projet. `C2` se base dessus pour apporter ses modifications et on poursuit ainsi de suite avec les suivantes. Il n'y a pas de limite aux nombres de révisions.

### Dépôt

Les fichiers _versionnés_ sont mis à disposition sur un **dépôt**, c'est à dire un espace géré par un logiciel de gestion de versions et souvent hébergé sur un serveur externe.

Pour pouvoir effectuer des modifications, il faut au préalable télécharger ce dépôt qui contient l'ensemble de ces fichiers.

Par défaut, on se base sur la dernière révision faite s'il y en a déjà eu avant.

### Branche

### Conflit

### Systèmes centralisés et décentralisés
