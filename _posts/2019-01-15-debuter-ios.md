---
layout: post
title:  "Créer une application iOS (iPhone ou iPad)"
date:   2019-01-15 20:00:00 +0100
image: iphone.jpg
comments: true
video: false
---

Vous avez envie de faire une application iOS ? Voici comment débuter facilement la création d'une application pour iPhone ou iPad.

Attention, ceci n'est pas un tutoriel pour apprendre à coder en Objective-C ou en Swift - qui sont les 2 langages utilisés sur iOS - mais un article qui décrit un chemin simple pour savoir par où et comment commencer.

* * *

# Intro

Que ce soit sur iPhone ou iPad, le système d'exploitation utilisé est le même : iOS. Depuis la sortie de l'iPhone 1 (2007), cet environnement est utilisé sur tous les appareils Apple - même si le nom a changé depuis la 1ère génération de l'iPhone.

Grâce à cet environnement, on peut créer ses propres applications et les proposer à tous les utilisateurs d'appareils Apple et ça en fait des utilisateurs potentiels. En effet on compte environ 800 millions d'utilisateurs d'iPhone dans le monde.

Avec ces chiffres, Apple propose un système qui permet à n'importe qui de publier son application sur leur "store" mais en contrepartie elle récupère 30% de tout ce que l'application vous rapporte : pub, application payante ou in-app (achat dans l'application).

Cet article explique seulement la création d'application dite "native", c'est-à-dire spécifiquement pour iOS. On parle à contrario d'applications hybrides quand le même code peut être utilisé sur des plateformes différentes. Les principaux intérêts des applications natives est de pouvoir utiliser toutes les fonctionnalités du système ainsi que de meilleurs performances.

# Comment commencer

## Mac

La première chose qu'il faut pour débuter la création d'applications iOS, c'est un Mac. Malheureusement c'est obligatoire, que ce soit pour télécharger Xcode (plus de détail ci-dessous) ou tous les outils nécessaires pour déployer une application.

Il est possible d'installer macOS sur certaines machines Windows mais ça demande un peu de travail et on entre dans une zone grise juridique.

## « Apple Developer »

La souscription "Apple Developer" n'est pas obligatoire pour commencer à développer. En effet vous pourrez télécharger les outils nécessaires, coder et déployer l'application sur un véritable appareil (ce qui n'était pas le cas il y a quelques années). Dans ce cas votre application restera 7 jours sur votre appareil avant d'être supprimée.

Pour souscrire au programme il vous faut créer un [compte développeur Apple](https://developer.apple.com){:target="_blank"}. Vous pouvez utiliser votre compte Apple si vous en avez un ou bien en créer un nouveau.

Vous devez être majeur pour participer au programme. 

### Programmes "Individuals / Organizations"

Le programme "individuals" est disponible si vous souscrivez au programme en tant qu'individu ou que vous êtes le propriétaire de votre entreprise. La création se fera sous votre nom et plus rapidement parce qu'il vous faudra seulement une carte bancaire.

A l'inverse la version entreprise est plus complète et permet de pouvoir gérer plusieurs utilisateurs et leurs rôles dans le déploiement d'applications (Admin, Manager, Developer, Marketing...).

Cette inscription coûte 99$ par an, peu importe votre choix.

A savoir: un abonnement peut vous être offert si vous êtes association.

### Apple Developer Enterprise Program

Ce programme est un peu différent des 2 premiers. En effet il permet d'avoir une gestion beaucoup plus précise de la distribution des applications. Ce programme ouvre l'accès d'un "App Store" privé et géré par l'entreprise elle-même.

Elle peut être utile pour les grosses entreprises qui veulent déployer des applications à tous leurs salariés sans la mettre à disposition publiquement.

Cette inscription coûte 299$ par an.

# Technologie

## Xcode

La façon la plus simple de télécharger Xcode est de passer par l'App Store sur votre Mac. Cela vous permettra de faire la mise à jour (régulière - quelques fois par an) automatiquement.

Xcode est l'IDE (Environnement de développement) par défaut pour tous les développements d'applications iOS, watchOS (Apple Watch) et macOS (Mac). C'est grâce à cet outil que vous allez pouvoir développer, déployer votre application sur un appareil iOS et déployer sur l'App Store.

![Xcode]({{ site.url }}/content/images/xcode.png)

## Objective-C / Swift

Il existe 2 principaux langages de programmations disponibles sur iOS.

L'Objective-C est le 1er langage utilisé sur cette plateforme. Il a été créé par Apple en 1983 pour ses propres produits et est toujours employé dans la plupart des applications.

Swift est arrivé bien plus tard (2014) pour moderniser l'Objective-C. Ce langage est maintenant largement mis en avant par Apple et se veut être le remplaçant du vieillissant Objective-C.

Si vous commencez à coder, privilégiez donc le Swift sauf si vous devez utiliser du C++ dans quel cas vous n'avez pas d'autres choix que de prendre l'Objective-C.

Heureusement, les deux langages sont interopérables et peuvent être utilisés dans le même projet, dans des fichiers différents.

# Déploiement sur iPhone/iPad

Si vous ne disposer pas de compte Apple Developer, vous n'avez rien de spécial à faire. Il suffit de brancher votre appareil sur votre Mac, de le déverrouiller et d'accepter les demandes du Mac (popups qui s'affichent automatiquement).

Dans le cas où vous avez un compte Apple Developer, il vous faut le configurer. Xcode est maintenant capable de gérer ça automatiquement - dans la plupart des cas. Il va ajouter votre "Bundle Id" qui est l'identifiant de votre application, rajouter votre appareil dans la liste des appareils autorisés et enfin créer les profils qui contiennent ces informations.

Il existe au minimum un profil de distribution et potentiellement un autre de développement. Ils sont gérés depuis votre espace de [développeur Apple](https://developer.apple.com){:target="_blank"}

Pour faire tout ça, le plus simple est de créer un projet de test sur Xcode. Ensuite vous allez dans les propriétés de votre projet et sélectionner (ou ajouter) votre compte Apple et tout devrait se mettre en place après quelques secondes / minutes. Si vous n'avez pas de d'erreur c'est que tout se passe bien (voir ci-dessous).

![Compte]({{ site.url }}/content/images/xcode-account.png)

Pour en être sûr, lancer votre projet via le bouton lecture en haut à gauche de Xcode.

Cette étape est nécessaire pour chaque projet et chaque nouvel appareil que vous voudrez utiliser. Sur le site Apple Developer vous pourrez voir tous vos utilisateurs, vos appareils, vos profils et vos certificats créés.

A savoir : Vous êtes limités à 100 appareils.

Vous pouvez bien sûr utiliser le simulateur qui permet de lancer rapidement et de tester une application sur tous les appareils souhaités, sans avoir besoin d'un compte Apple.

# Développement

Maintenant que tout est configuré correctement, il reste le développement de votre application.

Il existe beaucoup de tutoriaux et d'articles qui expliquent comment débuter la programmation Swift ou Objective-C.

On n'ira pas plus loin dans cet aspect mais je vous propose quelques liens qui vous permettront de le faire.

- [OpenClassRooms](https://openclassrooms.com/fr/courses/2582746-developpez-votre-premiere-application-pour-ios) (fr) : une référence dans les tutoriaux de programmation. Très bon tutorial pour commencer ou approfondir ses connaissances sur iOS.
- [raywenderlich](https://www.raywenderlich.com/ios) (en) : est un des sites les plus connus dans le communauté iOS. Il contient des articles et des vidéos très intéressants pour aller plus loin (en anglais).
- [Site officiel Swift](https://developer.apple.com/swift/) (en) : la référence officielle de la documentation Swift  

# Distribution sur App Store

Pour mettre votre application sur l'App Store, vous avez besoin de participer au programme Apple Developer.

Prévoyez quelques jours de validation d'Apple après soumission de votre application. Vous pouvez également recevoir des demandes complémentaires ou essuyer un rejet complet de votre application. Il vous faudra donc la modifier pour la resoumettre.

## iTunes Connect

[Itunes Connect (ou App Store Connect)](https://itunesconnect.apple.com/){:target="_blank"} est un autre site web qui vous permet de gérer votre application sur l'App Store. Votre compte est le même que celui utilisé sur le portail [Apple Developer](https://developer.apple.com){:target="_blank"}).

C'est la partie "App" qui nous intéressera ici.

Si c'est votre première visite sur cette espace, il faudra accepter quelques règles d'Apple et créer votre application. De nombreuses informations vous seront demandées pour cette création. Préparez-vous à passer un peu de temps à remplir tous les champs des formulaires.

Vous retrouverez de l'aide sur la documentation officielle [App Store Connect](https://developer.apple.com/support/app-store-connect/){:target="_blank"}.

### Informations contractuelles, bancaires et fiscales

Pour mettre en place une application payante ou des achats in-app, il faut renseigner les champs dans la page « Agreements Tax, and Banking » sur iTunes Connect. Vous aurez plusieurs variantes de contrat sur iTunes Connect à disposition pour commercialiser une application. À vous de sélectionner la plus adaptée.

À noter : toutes les demandes ou acceptations de nouveaux contrats ne peuvent être gérées que par l’agent d’équipe de iTunes Connect.

Dans l’aide [d’iTunes Connect](https://developer.apple.com/support/app-store-connect/){:target="_blank"}, vous trouverez toutes les informations nécessaires sur les possibilités de configuration.

## Paramètre de l'application

Retournons dans Xcode où il faut renseigner certains paramètres avant d'aller plus loin. Si vous l'avez déjà fait vous pouvez directement créer l'archive de votre application.

### Icone

Il est nécessaire de créer sa propre icone qui sera affichée sur l'appareil iOS. Vous pouvez ajouter ou modifier vos icones dans le fichier `Asset.xcassets` (depuis Xcode 9). C'est la même icone que vous devez produire en plusieurs tailles pour qu'elle s'affiche bien sur tous types d'appareils.

Je vous conseille de passer un peu de temps sur votre design, Apple étant assez regardant sur les icônes des applications.

### Identité

Il faut ensuite vérifier que certaines informations sont correctement renseignées. Pour les afficher et/ou les modifier sélectionner votre projet dans l'explorateur et allez ensuite dans l'onglet Général.

Vérifiez que ces informations sont bien renseignées :

- Display name : le nom de votre application
- Bundle ID : l'identifant unique (aucune autre application ne peut avoir le même)
- Version : la version de votre application (ce qui permet de faire des mises à jour de votre application)
- Build : (souvent égal à 1) cela permet de compléter la version. Une version peut avoir plusieurs builds.

## Création de l'archive

Toujours dans Xcode sélectionnez "Generic iOS device" dans la liste en haut à gauche des appareils. Lancez ensuite la création de l'application dans le menu Product (Produit) -> Archive. Cela va créer un fichier IPA qui contiendra toute votre application.

Vous pourrez ensuite uploader ce fichier dans la nouvelle fenêtre une fois que l'archive est créée.

## Soumission de votre application

Allez dans votre espace "App" dans [iTunes Connect](https://developer.apple.com/support/app-store-connect/){:target="_blank"}.

- Sélectionner (ou créer) votre application
- Vérifier / modifier les informations de votre version (Version, Build...)
- Sélectionner la façon de distribution:
    - Manuelle : c'est vous qui appuierez sur le bouton pour mettre votre application sur l'App Store dès qu'elle est validée
    - Automatique: l'application sera directement mise sur l'App Store
- Dans le coin en haut à droite, lancez la validation via le bouton "Submit for review"

Pour plus d'information, voici [l'aide officielle](https://help.apple.com/app-store-connect/#/dev301cb2b3e){:target="_blank"} (en).

La validation passera par plusieurs étapes au fur et à mesure :

- Finaliser avant soumission
- En attente de vérification
- En cours de vérification
- Prêt à la vente

## App Store

Félicitation d'être arrivé jusqu'ici !

Il ne vous reste qu'à patienter quelques jours le temps de recevoir la validation (ou non) de votre application.

Vous retrouverez ensuite votre application sur le store.

# Fin

N'hésitez pas à poser vos problèmes ou vos questions dans les commentaires ci-dessous.

La création d'une application iOS pose souvent quelques accrocs et il est difficile d'être exhaustif sur toutes les étapes de création.

Même si la gestion du compte Apple et la mise à disposition sur l'App Store d'une application sont un peu compliquées, je vous conseille de commencer à créer votre produit avant.

Vous pouvez par exemple ne pas créer de compte Apple Developer, utiliser le simulateur pour la plupart des cas d'utilisation; seules certaines contraintes vous obligeront à utiliser un appareil physique (besoin du GPS, musique, nom de l'appareil...).

Cela ayant pour but d'éviter de participer au "Apple Developer Program" et devoir débourser 99$ au début de votre projet.