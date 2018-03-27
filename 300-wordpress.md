---
layout: page
title: WordPress
permalink: /wp/
---

Introduction à WordPress.

Définitions
---

**WordPress** est un système de gestion de contenus (CMS, pour Content Management System). 

Par défaut, WordPress comprend un certain nombre de fonctionnalités (p.ex: types de contenus, gestion des menus, gestion des médias, gestion des utilisateurs...). On parle de fonctionnalités faisant partie du noyau de WordPress ("core functionality").

D'autres fonctionalités peuvent être ajoutés par des **extensions** (en anglais: *plugins*). Exemple: ajouter un formulaire de contact. Un grand nombre d'extensions est disponible gratuitement (sur le site WordPress.org), d'autres font l'objet d'une distribution commerciale, ou sont développées sur mesure pour un besoin spécifique.

Le **thème** définit la présentation visuelle d'un site WordPress. Il est nécessaire d'avoir un thème activé, pour qu'un site WordPress soit fonctionnel. Tout comme pour les plugins, les thèmes WordPress peuvent être disponibles gratuitement ou contre paiement.

Un petit historique:
===

L’année 2018 marquera le 15e anniversaire de WordPress, la version 1.0 ayant vu le jour en 2003.

En 2005, Matt Mullenweg, initiateur de WordPress, fonde sa compagnie Automattic, et lance la plate-forme d’hébergement WordPress.com. 

WordPress devient en quelques années le système de gestion de sites (CMS) le plus utilisé dans le monde. En 2011, WordPress faisait tourner près de 15% des sites Internet. Son usage dépasse les 25% en 2015, et se situe en début 2018 à 30%. Cela correspondrait à 300 millions de sites, sur un nombre total estimé à un milliard.

![Statistiques d'utilisation des CMS de 2011 à 2017.](/cours-wp/img/wordpress-usage-2017.png)

Pour plus d’infos sur l’historique de WordPress, lire [https://github.com/WordPress/book](https://github.com/WordPress/book) (en anglais).

Blog vs. CMS
===

Si dans ses débuts, WordPress était un « simple outil de blogging », il est devenu au fil du temps un système de gestion de contenus polyvalent. Il est utilisé couramment pour des sites d’entreprises, d’institutions, ou de commerce en ligne.

Un logiciel libre
===

WordPress est un logiciel libre, sa liberté étant garantie par la licence GPL. Chacun est libre de l’utiliser, de le modifier, et de le distribuer. Le développement est assuré par une communauté internationale. 

Thèmes et Extensions
---

Les **thèmes** et les **extensions** (plugins) sont deux éléments fondamentaux pour faire fonctionner votre site WordPress.

Les thèmes
==

Le thème définit l’habillage graphique de votre site WordPress.

On peut utiliser un thème gratuit, acquérir un thème payant, ou développer un thème sur mesure pour des besoins spécifiques.



Choisir un thème gratuit
===

Quelques thèmes gratuits de haute qualité:

- Les thèmes l’équipe Automattic : [http://profiles.wordpress.org/automattic/](http://profiles.wordpress.org/automattic/)
- Le blog ThemeShaper présente des thèmes récents: [https://themeshaper.com/](https://themeshaper.com/) 
- Une collection de thèmes par Hugo Baeta: [http://hugobaeta.com/portfolio/thefivethemes/](http://hugobaeta.com/portfolio/thefivethemes/)
- Les thèmes d'Anders Norén: [http://www.andersnoren.se/teman/](http://www.andersnoren.se/teman/)

À noter : WordPress est accompagné par plusieurs thèmes par défaut. Un nouveau thème est développé chaque année. Le plus récent se nomme *TwentySeventeen*.

![Quelques-uns des thèmes par défaut de WordPress](/cours-wp/img/wordpress-default-themes.jpg)

Choisir un thème commercial (“premium”)
===

Quelques boutiques de thèmes intéressantes (parmi les milliers qui existent):

* Elma Studio – [https://www.elmastudio.de/en/themes/](https://www.elmastudio.de/en/themes/)
* The Theme Foundry – [https://thethemefoundry.com/](https://thethemefoundry.com/)
* Array Themes – [https://arraythemes.com/](https://arraythemes.com/)
* Themes Kingdom - [https://themeskingdom.com](https://themeskingdom.com)


Il existe de nombreuses autres sources de thèmes commerciaux – voici une liste de boutiques: [http://wordpress.org/themes/commercial/](http://wordpress.org/themes/commercial/)

Lire aussi à ce sujet :

* Thèmes WordPress: Comment les choisir?, [http://goo.gl/DNSxfj](http://goo.gl/DNSxfj)
* Le blog WpThemesPro, par Alex Bortolotti : [http://wp-themes-pro.com/](http://wp-themes-pro.com/)

À noter : normalement, un thème WordPress définit **l’apparence visuelle**, mais n’ajoute pas de fonctionnalités à un site (comme p.ex. un formulaire de contact). Si c’était le cas, cela obligerait l’utilisateur à toujours conserver le même thème, sous peine de perdre la fonctionnalité concernée. 

Les **fonctionnalités** sont en principe fournies par les extensions (plugins). Certains thèmes vont donc recommander l'installation d'extensions spécifiques (p.ex. pour activer de nouveaux types de contenus, tels qu'un "portfolio").

Les extensions
===

Les **extensions** sont des outils permettant d'étendre les fonctionnalités de WordPress. Les extensions offrent des fonctions personnalisées pour répondre à des besoins spécifiques.

Le site WordPress.org est la source numéro 1 d'extensions. Les extensions qui s’y trouvent ont été approuvées par une équipe de volontaires. Ils sont obligatoirement gratuits et sous licence GPL.

Ce site propose actuellement près de 30’000 extensions couvrant toutes sortes de besoins. 

[http://wordpress.org/plugins/](http://wordpress.org/plugins/)

Voici quelques extensions particulièrement utiles. Elles sont toutes gratuites, et se trouvent dans la liste des extensions de wordpress.org.

<div class="cards"></div>

* **BuddyPress** - Permet de créer un réseau social interne à un site WordPress.
* **bbPress** - Permet de créer un forum.
* **Jetpack** - Un ensemble de fonctionnalités, développées à l’origine pour les usagers de WordPress.com. Cela inclut notamment un “carrousel” pour la présentation des galeries d’images, des fonctions de partage sur les réseaux sociaux, un module de statistiques pour analyser les visites de votre site...
* **WooCommerce** - Permet la création d’une boutique en ligne. Lancé en 2011, ce plugin est en passe de devenir la solution de vente en ligne [la plus utilisée au monde](https://trends.builtwith.com/shop). Lire aussi : Allain Lagadic, [WooCommerce : Passer d’un blog à une boutique en ligne](https://interactif.com/woocommerce-boutique-en-ligne-wordpress/), Août 2013.
* **MailPoet** - Permet d’administrer une newsletter depuis votre site WordPress.
* **Contact Form 7** - Permet de créer un formulaire de contact. À noter qu’un formulaire de contact est également inclus dans Jetpack.
* **Statify** - Permet d’avoir des statistiques sur la fréquentation de votre site. Développée en Allemagne, cette extension respecte la réglementation européenne en matière de protection des données. 
* **AntispamBee** - Une extension anti-spam, pour réduire la quantité de spams dans les commentaires de votre site.
* **BackWpUp** - Une extension de backup, qui permet de créer périodiquement des sauvegardes des contenus de votre site.
* **Duplicate Post** - Permet de partir d’un article existant comme modèle pour créer de nouveaux contenus.
* **Search Everything, Relevanssi** - Deux extensions différentes qui permettent d’étendre la fonctionnalité de recherche de WordPress.

Plus d’informations sur le choix des extensions :

Jonathan Buttigieg: *[10 conseils pour choisir un plugin WordPress](http://www.geekpress.fr/comment-choisir-plugin/)*.

WordPress.org ≠ WordPress.com
---

Il est important de comprendre les différences entre **WordPress.ORG** (version communautaire et indépendante de WordPress) et **WordPress.COM** (service hébergé proposé par Automattic).

**WordPress.ORG** est la source de téléchargement pour WordPress, c'est là où vous trouverez la version que vous pouvez installer sur un hébergement web de votre choix. WordPress.ORG propose également un large choix de Thèmes et d'Extensions gratuites et open-source, validées par une équipe bénévole. WordPress.ORG sert aussi de portail vers les forums, la documentation pour développeurs, et le système de tickets permettant de rapporter des bugs ou proposer de nouvelles fonctionalités. Le domaine WordPress.ORG est géré par la Fondation WordPress.

Particularités d’une installation indépendante (.ORG) :

* Peut être hébergée partout sur le web.
* Permet une totale liberté dans l’usage de thèmes et de plugins.
* N'inclut pas de nom de domaine et d'hébergement.
* Vous devrez appliquer les mises à jour régulièrement pour garantir la sécurité de votre site.

**WordPress.COM** est un service commercial (avec une version de base gratuite, et des services payants) fourni par la firme Automattic.

Particularités d’une installation hébergée (.COM) :

* Permet de lancer rapidement (et gratuitement) un site.
* Un choix limité de thèmes (gratuits ou payants).
* Ne permet pas l’installation de plugins.
* Exige de payer un supplément pour certaines fonctions.

![Les offres freemium de WP.COM, fin 2017](/cours-wp/img/wpcom-plans.png)

Plus d’informations sur cette question : 

* Patrick Finot : *[WordPress.org et WordPress.com, pourquoi deux systèmes? Comment choisir?](http://www.informatique-enseignant.com/deux-systemes-wordpress-comment-choisir/)*, décembre 2012.
* Fabrice Ducarme : *[WordPress.com ou WordPress.org, quelle différence ?](https://wpformation.com/wordpress-com-vs-wordpress-org-quelle-difference/)*, avril 2013.

## Technique

WordPress est une application web reposant sur PHP et MySQL (la base de données).

En publiant des contenus, vos pages, articles, commentaires, ainsi que tous vos réglages, sont enregistrés dans la base de données MySQL de votre site.

D'autre part, les attachements (images, pdfs, tout type de fichier que vous ajoutez à vos articles) sont stockés dans un dossier spécifique du site (par défaut: `wp-content/uploads`).

Lors d'un déménagement de site, il est indispensable d'exporter la base de données, et de préserver votre dossier `wp-content/uploads`: ces deux éléments constituent vos données personnalisées.

De nombreuses solutions de backup existent, vous permettant de faire des sauvegardes de votre base de données, et des fichiers du site.

Pour les questions relatives aux domaines et à l'hébergement, [voir ce chapitre](/divers/domaines/).