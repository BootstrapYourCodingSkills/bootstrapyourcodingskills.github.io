---
layout: post
title:  "Qu'est-ce qu'un site statique ?"
date:   2017-03-02 13:13:14 +0100
image: subway-notstatic.jpg
comments: true
video: false
---

Un site web statique n'est pas un site immobile, c'est un site dont le contenu ne change pas en fonction de l'utilisateur.

A l'inverse, un site dynamique présente un contenu différent selon l'utilisateur, comme par exemple votre profil Facebook qui n'est accessible que par vous. Les pages sont alors construites "à la volée" grâce à un langage de programmation qui s'exécute sur un serveur. En informatique, on appelle cette partie le backend. À l'opposé on trouve le frontend qui est la partie visible du site internet.

La plupart des sites internet sont dynamiques. Quel est alors l'intérêt d'un site statique ? Et dans quel cas est-ce avantageux ?

* * *

# Comment ça fonctionne ?

Pour créer un site statique, on utilise un générateur, par exemple [Jekyll](https://jekyllrb.com/){:target="_blank"} qui est également utilisé sur ce site. Il en existe d'ailleurs [beaucoup d'autres](https://www.staticgen.com/){:target="_blank"}.

Un site statique comprend des fichiers avec une syntaxe [Markdown]({% post_url 2017-01-17-quest-ce-que-le-markdown %}){:target="_blank"} (ou similaire) qui compose le contenu de votre site web. Le générateur va transformer les fichiers Markdown en page HTML et les intégrer dans un site web.

L'ensemble sera ensuite hébergé sur un serveur, le plus basique possible. Celui-ci se contente de transmettre les pages aux navigateurs clients. Il n'y a pas de code, pas de base de données, pas de calcul.

On est donc limité par ce qu'on peut faire : pas d'administration, pas d'envoi de mail, rien "d'intelligent"... mais on se retrouve avec un site extrêmement rapide et simple à gérer.

Il est possible d'avoir des pages HTML, du CSS et du Javascript dans un site statique. Il n'y a donc pas de différence visuelle entre un site statique et un site dynamique. Ce sont les mêmes technologies utilisées.

# Avantages et inconvénients d'un site statique

On va voir ici quels sont les points forts et les points faibles d'un site statique par rapport à un site dynamique.

Commençons d'abord par les points forts.

## Avantages

#### Rapide

Un site statique est beaucoup plus rapide qu'un site dynamique, forcément il n'y a pas de backend donc pas de base de données et pas de code. Le serveur n'a pas de calcul à effectuer, il renvoie la page demandée, c'est tout. Seule la partie visible (frontend) est chargée par l'utilisateur.

#### Sécurisé

Un autre point extrêmement important est la gestion liée à la sécurité. Comme on l'a vu plus haut, il n'y a pas de code sur le serveur, donc plus d'erreur humaine soit beaucoup moins de problèmes de sécurité. Il faut savoir que la plupart des failles des sites web sont liées à des erreurs humaines.

Les problèmes restants sont liés au serveur sur lequel est hébergé votre site web : système d'exploitation, serveur web... Problèmes qui sont également présents sur des sites dynamiques.

A savoir que tout ce que vous publiez sur un site statique peut être visible par n'importe qui. Il faut donc être prudent quand on met à jour son site.

#### Simple

La structure est simple : un dossier pour les articles, un autre pour les brouillons, un fichier de configuration, quelques fichiers HTML et CSS pour rendre ça plus sympa et c'est tout.

Avec une courbe d'apprentissage à prendre en compte, à voir dans les [inconvénients](#comptences), n'importe qui peut créer et mettre à jour un site statique. Un site statique est généralement créé avec des fichiers statiques, comme le [Markdown]({% post_url 2017-01-17-quest-ce-que-le-markdown %}){:target="_blank"}.

#### Mise à jour

La mise à jour se fait très facilement. On le fait soit via une ligne de commande soit via un outil - comme un client FTP - pour transmettre les fichiers qu'on a sur son poste vers le serveur.

C'est quelque chose de très courant et il existe beaucoup de documentation pour vous aider.

#### Bon marché

Un autre avantage est qu'il est bon marché. En effet, comme on l'a vu, il n'y a pas de backend, donc le serveur nécessaire est le plus basique possible. Pas de code, pas de base de données, un serveur simple est donc suffisant.

Il existe également des solutions (comme [Github Pages](https://pages.github.com/){:target="_blank"}) qui hébergent gratuitement le code et le déploie sur un serveur. Seul le nom de domaine est à votre charge.

#### Limité mais possible d'externaliser

On le verra dans la partie suivante mais le fait de ne pas avoir de backend peut limiter grandement ce qu'on veut faire. Il faut donc bien réfléchir à quel type de site on veut.

D'un autre côté, il est possible d'externaliser les fonctionnalités intelligentes du site en utilisant des services tiers. Par exemple, on peut afficher des commentaires via [Disqus](https://disqus.com/){:target="_blank"}, c'est donc ce service qui va gérer tous les commentaires de votre site. Il se base sur l'URL de la page pour afficher ce qu'il faut.

On peut aussi confier les statistiques des visites à [Google Analytics](https://www.google.fr/intl/fr/analytics/){:target="_blank"}.

Il existe de plus en plus de services tiers qui peuvent vous faire profiter de fonctionnalités que vous ne pourrez pas faire sur un site statique.

Ou le faire vous-même sur un autre site. Mais si vous en avez vraiment besoin, ce n'est peut-être pas un site statique qu'il vous faut.

## Inconvénients

#### Pas d'administration

L'inconvénient le plus considérable d'un site statique est qu'il est limité. On ne peut pas faire de chose "intelligente". C'est-à-dire qu'on ne peut pas utiliser de formulaire, donc pas d'administration ou de connexion/inscription. Ça veut aussi dire pas de backend, donc pas possibilité d'envoi de mail ou d'enregistrer dans une base de données. La liste n'est bien sûr pas exhaustive.

Si vous vous demandez si ce que vous voulez faire est possible, il suffit de se poser la question: "Est-ce que j'ai besoin de code sur le serveur ?". Si la réponse est oui alors un site statique n'est pas fait pour vous.

On ne peut pas avoir quelque chose de très simple, de bon marché et de très complet.

Il ne faut pas négliger cet inconvénient pour prendre la décision du type de site web qu'on veut. On utilisera donc plus facilement un site statique sur un site plutôt simple, qu'on ne mettra pas à jour trop régulièrement.

#### Pas d'e-commerce

Pour préciser la partie précédente, on ne peut pas faire de chose complexe, donc évidemment on ne peut pas créer sa boutique en ligne.

#### Compétences

Pour créer un site statique, il faut apprendre à utiliser un générateur. Il faut donc comprendre la structure des dossiers et la configuration du site ainsi que la façon dont le générateur fonctionne.

De plus, la majorité des générateurs utilise la ligne de commande pour la plupart des tâches (par exemple : lancer le serveur). Il faut donc connaître les commandes les plus basiques d'un terminal pour être efficace et comprendre ce que l'on fait.

Il est également nécessaire de comprendre la syntaxe [Markdown]({% post_url 2017-01-26-syntaxe-markdown %}){:target="_blank"}, ou autre si une syntaxe différente est utilisée, pour modifier les fichiers de contenu du site.

#### Tout installer sur son poste

Que ce soit pour créer ou simplement mettre à jour son site, il faut installer tous les outils nécessaires sur son poste. Ça veut dire qu'on ne peut pas le faire de n'importe où et qu'il faut prendre le temps pour le faire.

# Dans quels cas privilégie t-on un site statique ?

On conseille généralement un site statique pour des sites relativement simples, par exemple des sites de présentations : CV, portfolio, sites vitrines d'entreprise ou de produit, ou également pour de la documentation technique ou non. Peu importe que ce soit un site personnel ou professionnel.

La qualité perçue peut être la même que ce soit un site statique ou dynamique : ce sont les mêmes technologies qui peuvent être utilisées.

Les sites statiques font généralement moins de mise à jour que des sites dynamiques sur lesquels la modification est simplifiée via des CMS (exemple : [Wordpress](https://fr.wordpress.com/){:target="_blank"}) pour ajouter ou modifier des articles ou des pages.

Pour finir, un site statique a des limites et des inconvénients qu'il faut connaître mais qu'on peut parfois contourner en utilisant des services externes. On peut donc tout à fait utiliser un site statique pour de nombreux besoins, bien plus que ceux présentés ci-dessus.

Pour finir, je conseille, dans la mesure du possible, d'utiliser un site statique qui sera plus rapide, simple et sûr.