# Installation

### Mac

##### Ruby

Avant tout chose, il faut vérifier que Ruby soit bien installé avec une version 2.3.3 ou plus.

Pour cela, il suffit de lancer `ruby -v` dans l'application Terminal sur votre Mac. Si votre version Ruby est inférieur, il faut la mettre à jour. Homebrew est probablement la façon la plus simple de le mettre à jour.

Ensuite, il suffit d'installer des outils pré-installés sur Mac via la commande : `xcode-select --install`.

##### Jekyll

Ensuite, il ne reste plus qu'à lancer cette nouvelle commande, toujours dans le Terminal :

```gem install bundler jekyll```

### Windows

##### Ruby

Comme sur Mac, il faut tout d'abord installer Ruby. Pour cela, je vous conseille d'installer [RubyInstaller](https://rubyinstaller.org/) et de le mettre à la racine de votre disque (exemple: `C:\` pour éviter d'avoir des espaces qui peuvent compliquer la suite).

##### Jekyll

Il suffit ensuite de lancer l'invite de commande et d'écrire : `gem install jekyll bundler`.

Et le tour est joué.