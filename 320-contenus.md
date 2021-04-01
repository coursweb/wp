---
layout: page
title: Contenus
---

Les contenus d’un site WordPress
---

En utilisant votre site WordPress, vous allez travailler avec les éléments suivants :

- Articles et Pages (et autres contenus)
- Catégories et Etiquettes (et autres taxonomies)
- Commentaires
- Menus
- Widgets

## Articles et Pages

Ce sont les deux principaux types de contenus de WordPress. En anglais, les articles sont nommés « Posts ».

Dans l'interface d'édition, ces contenus ont un champ titre et un champ d'édition à première vue identique. Néanmoins, ces contenus ont leurs particularités:

**Particularités des Articles**

* Peuvent être classées (par *Catégories* et *Etiquettes*).
* La date de publication sera généralement visible.
* Peuvent recevoir des *commentaires*.
* Peuvent utiliser les formats d’articles.
* Sont affichés dans les archives (par date, etc).
* Sont inclus dans le flux RSS du site.

**Particularités des Pages**

* Peuvent s’organiser de manière hiérarchique (page → sous-page).
* Ne sont pas affichés dans les archives.
* Peuvent utiliser les "modèles de pages" (différents pour chaque le thème).

Voici un comparatif entre Article et Page, présentant le même contenu. Le thème utilisé est *Libre*.

![Différences entre Article et Page](/cours-wp/img/articles-vs-pages.jpg)

Pour plus d’explications:

* Olivier Grobet : *[Différences entre une Page et un article](http://www.elephorm.com/tutoriel-wordpress/differences-entre-une-page-un-article)* (vidéo)
* Support WordPress.com: *[Post vs. Page](https://en.support.wordpress.com/post-vs-page/)*
* WPBeginner : *[What is the Difference Between Posts vs. Pages in WordPress](http://www.wpbeginner.com/beginners-guide/what-is-the-difference-between-posts-vs-pages-in-wordpress/)*

## Catégories, étiquettes (et taxonomies)

Afin d'organiser vos contenus, WordPress utilise le concept de "taxonomie", càd un système de classification pour subdiviser les articles en unités plus gérables.

Les **catégories** et **étiquettes** (tags) sont les deux systèmes de classement (taxonomies) actifs par défaut. Il est possible d’en rajouter d’autres selon les besoins – on parlera alors de *custom taxonomies*.

**Pour plus de détails:** voir la présentation de Benjamin Lupu, "[Architecture de l’information pour WordPress](https://wordpress.tv/2016/04/05/benjamin-lupu-architecture-de-linformation-pour-wordpress/)", au WordCamp Paris 2016.

Exercice: 
===

Un blogeur écrit des critiques de livres, de films et de jeux. 

* Créer pour cela une **taxonomie** custom, "Critiques" 
* Les critiques seront des Articles, les termes de la taxonomie seront « livres », « films », « jeux ».
* Dans une zone Sidebar, créer un **widget** pour cette Taxonomie. Ce **widget** peut contenir un **menu**, comprenant les pages d’archive des ”livres, films, jeux”.

## Post Formats (formats alternatifs)

Certains thèmes permettent l’utilisation des « formats d’articles » (*Post Formats*), qui offrent une présentation visuelle alternative pour certains formats prédéfinis. Les formats possibles sont: *En passant, Image, Vidéo, Citation, Lien, Galerie, État, Son, Discussion*. Ces formats peuvent être appliqués aux Articles, si le thème supporte cette option. 

![Le sélecteur de Format dans l’interface d’édition](/cours-wp/img/wordpress-post-formats.png)

La liste des *Post Formats* disponibles est "figée", et limitée à ces dix options. L'idée est d'encourager les concepteurs de thème à créer des affichages spécifiques pour ces formats, afin d'éviter de les perdre en cas de changement de thème.

**Note historique:** Les *Post Formats* on été introduits en 2011 ([ticket 14746](https://core.trac.wordpress.org/ticket/14746)). En 2013, au cours de la release 3.6, l'équipe de développement à tenté de donner plus d'importance aux *Post Formats* dans l'interface d'édition. Ces tentatives ont finalement été rejetées, après des débats houleux. Voir [cet article de Mark Jaquith](https://make.wordpress.org/core/2013/05/29/post-formats-ui-is-exiting-core-will-live-as-a-plugin/) pour plus de détails.

**NB:** Ne confondez pas *Post Formats* et *Custom Post Types*. Les *Post Formats* sont des articles (*Posts*) avec une présentation alternative, mais restent de simples articles. Les *Custom Post Types* ouvrent une nouvelle dimension en permettant l'ajout de nouveaux types de contenus.

## Custom Post Types (types de contenus personnalisés)

Les *Custom Post Types* permettent d’ajouter de nouveaux *types de contenus* à un site, en plus des contenus par défaut que sont les *Articles*, *Pages*, *Médias* et *Commentaires*. 

Recettes de cuisine, produits, objets immobiliers... tout dépendra des besoins de votre site. Ces contenus spécifiques sont appelés des **Custom Post Types** (types de contenus).

Par exemple, un plugin de gestion d’événements pourra ajouter un type de contenu *Evénement*. Un plugin de vente en ligne (comme WooCommerce) ajoutera souvent des *Produits*.

Comme pour les taxonomies, vous êtes libre de créer des *Custom Post Types* correspondant à vos besoins.

L'extension *[Custom Post Type UI](https://wordpress.org/plugins/custom-post-type-ui/)* vous permet de créer facilement des types de contenu et des taxonomies supplémentaires.

### L'option Portfolios avec Jetpack

L'extension **Jetpack** offre une option *Portfolios*, qui permet entre autres de présenter des projets sous forme de galerie d'images. Cette option n’est toutefois compatible qu’avec certains thèmes Wordpress.

* Une fois l'extension Jetpack installée, celle-ci apparaît dans votre tableau de bord Wordpress. Cliquez dessus, puis allez dans *Réglages*.
* Jetpack vous propose ici diverses fonctionnalités pour votre site internet. Cliquez sur l'onglet *Rédaction* (Writing), puis scrollez jusqu'à la catégorie *Types de contenus personnalisés*. Activez l'option *Portfolios*.

![Activation des Portfolios de Jetpack](/cours-wp/img/jetpack-activation-portfolio.png)

* Rechargez votre page. Un onglet *Portfolio* doit maintenant se trouver dans votre tableau de bord.
* Depuis cet onglet, vous pouvez créer des *Projets*, qui fonctionnent plus ou moins comme des *Articles*. 
* Afin de présenter vos *Projets* sous forme de galerie d'images (souvent en grille), vous devez à présent créer une *Page*, puis dans *Attributs de page* choisir le *Modèle de page Portfolio* (cela dépend de votre thème). 
* Vous pouvez également classer vos projets par *Types de projets*. Dans l'onglet *Portfolios* de votre tableau de bord, cliquez sur *Types de projets*, puis créez un nouveau type. Lorsque vous créerez un nouveau projet, vous pourrez maintenant lui attribuer un type, ce qui facilitera la navigation à travers vos différents projets.

![Modèles Portfolio dans les thèmes Argent, Illustratr, Blask et Deppo](/cours-wp/img/portfolio-themes.jpg)

Quelques thèmes qui utilisent les Porfolios de Jetpack:

* [Argent](https://wordpress.com/theme/argent), par Mel Choyce (Automattic)
* [Blask](https://wordpress.com/theme/blask), par Mel Choyce (Automattic)
* [Illustratr](https://wordpress.com/theme/illustratr), par Thomas Guillot (Automattic)
* [Deppo](https://themeskingdom.com/wordpress-themes/deppo-portfolio-wordpress-theme/), par Themes Kingdom
* [Zeitreise](https://www.elmastudio.de/en/themes/docs/zeitreise/), par Elmastudio

Jetpack n'est pas la seule possibilité pour créer un type de contenu "portfolio" - d'autres solutions existent :

- [Custom Content Portfolio](https://fr.wordpress.org/plugins/custom-content-portfolio/), une extension de Justin Tadlock. Ces portfolios comportent certains champs spécifiques (project image, URL, client, location, start/end dates, and a description).
- [Genesis Portfolio Pro](https://wordpress.org/plugins/genesis-portfolio-pro/), par StudioPress. Utilisé par les thèmes de cette agence.
- [Portfolio Post Type](https://wordpress.org/plugins/portfolio-post-type/), utilisé par les thèmes de ThemeBeans.

### Choisir le nom d'un Custom Post Type

Une autre question qui se pose lorsqu'on définit un nouveau type de contenu: faut-il utiliser le **singulier** ou le **pluriel**? P.ex. si vous ajoutez un type de contenu "Projets", faut-il que son identifiant soit "projet" ou "projets"? 

La pratique habituelle est d'utiliser le singulier. Cela donne des URL plus courtes, et c'est plus cohérent: en effet, l'URL "projet/nom-du-projet" affichera **un** projet à la fois.


## Les auteurs

Votre site comprendra un ou plusieurs auteurs avec différents niveaux d’accès. Par défaut, WordPress offre les rôles suivants : 

* **Administrateur** : tous les accès
* **Editeur** : peut publier et modifier des articles, y compris ceux des autres.
* **Auteur** : peut publier et modifier ses propres articles.
* **Contributeur** : peut écrire et gérer ses articles, mais ne peut les publier.
* **Abonné** : ne peut gérer que son profil.

Voir le Codex pour plus de détails sur les [Rôles et capacités](http://codex.wordpress.org/fr:R%C3%B4les_et_Capacit%C3%A9s).

Pour plus d’informations sur ces éléments de base, lire :

* Codex Francophone, [Premiers pas avec WordPress](http://codex.wordpress.org/fr:Premiers_pas_avec_WordPress)
* Patrick Finot, [Premiers pas dans l’administration de WordPress](http://www.informatique-enseignant.com/decouvrir-administration-wordpress/)

