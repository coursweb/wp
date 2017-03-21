---
layout: page
title: Contenus
permalink: /wp/contenus
---

Les contenus d’un site WordPress
---

En utilisant votre site WordPress, vous allez travailler avec les éléments suivants :

- Posts et Pages
- Categories, tags et taxonomies
- Commentaires
- Les liens
- Auteurs
- Menus
- Widgets

Articles et Pages
==

Ce sont les deux principaux types de contenus de WordPress. En anglais, les articles sont nommés « Posts ».

**Particularités des articles :**

* Peuvent être classés (par *Catégories* et *Etiquettes*).
* La date de publication sera généralement visible.
* Peuvent recevoir des commentaires.
* Sont inclus dans le flux RSS du site.

**Particularités des pages :**

* Peuvent s’organiser de manière hiérarchique (page → sous-page).

Pour plus d’explications:

* Olivier Grobet : *[Différences entre une Page et un article](http://www.elephorm.com/tutoriel-wordpress/differences-entre-une-page-un-article)* (vidéo)
* Support WordPress.com: *[Post vs. Page](https://en.support.wordpress.com/post-vs-page/)*
* WPBeginner : *[What is the Difference Between Posts vs. Pages in WordPress](http://www.wpbeginner.com/beginners-guide/what-is-the-difference-between-posts-vs-pages-in-wordpress/)*

Catégories, étiquettes (et taxonomies)
===

Afin d'organiser vos contenus, WordPress utilise le concept de "taxonomie", càd un système de classification pour subdiviser les articles en unités plus gérables.

Les **catégories** et **étiquettes** (tags) sont les deux systèmes de classement (taxonomies) actifs par défaut. Il est possible d’en rajouter d’autres selon les besoins – on parlera alors de *custom taxonomies*.

**Pour plus de détails:** voir la présentation de Benjamin Lupu, "[Architecture de l’information pour WordPress](https://wordpress.tv/2016/04/05/benjamin-lupu-architecture-de-linformation-pour-wordpress/)", au WordCamp Paris 2016.

Post Formats (formats alternatifs)
===

Certains thèmes permettent l’utilisation des « formats d’articles » (*Post Formats*), qui offrent une présentation visuelle alternative pour certains formats prédéfinis. Les formats possibles sont: *En passant, Image, Vidéo, Citation, Lien, Galerie, État, Son, Discussion*. Ces formats peuvent être appliqués aux Articles, si le thème supporte cette option. 

![Le sélecteur de Format dans l’interface d’édition](/cours-wp/img/wordpress-post-formats.png)

La liste des *Post Formats* disponibles est "figée", et limitée à ces dix options. L'idée est d'encourager les concepteurs de thème à créer des affichages spécifiques pour ces formats, afin d'éviter de les perdre en cas de changement de thème.

**Note historique:** Les *Post Formats* on été introduits en 2011 ([ticket 14746](https://core.trac.wordpress.org/ticket/14746)). En 2013, au cours de la release 3.6, l'équipe de développement à tenté de donner plus d'importance aux *Post Formats* dans l'interface d'édition. Ces tentatives ont finalement été rejetées, après des débats houleux. Voir [cet article de Mark Jaquith](https://make.wordpress.org/core/2013/05/29/post-formats-ui-is-exiting-core-will-live-as-a-plugin/) pour plus de détails.

**NB:** Ne confondez pas *Post Formats* et *Custom Post Types*. Les *Post Formats* sont des articles (*Posts*) avec une présentation alternative, mais restent de simples articles. Les *Custom Post Types* ouvrent une nouvelle dimension en permettant l'ajout de nouveaux types de contenus.

Custom Post Types (types de contenus personnalisés)
===

Les *Custom Post Types* permettent d’ajouter de nouveaux *types de contenus* à un site, en plus des contenus par défaut que sont les *Articles*, *Pages*, *Médias* et *Commentaires*. 

Par exemple, un plugin de gestion d’événements pourra ajoutera un type de contenu *Evénement*. Un plugin de vente en ligne ajoutera souvent des *Produits*.

Comme pour les taxonomies, vous êtes libre de créer des *Custom Post Types* correspondant à vos besoins.

L'extension *[Custom Post Type UI](https://wordpress.org/plugins/custom-post-type-ui/)* vous permet de créer facilement des types de contenu et des taxonomies supplémentaires.

Menus
===

Les **menus** sont un élément spécifique, permettant notamment de créer une navigation pour votre site. Vous pouvez les créer et les administrer en vous rendant sous *Apparence > Menus*. Votre thème proposera un ou plusieurs emplacements pouvant accueillir des menus de navigation. La procédure de création d'une menu passe par ces étapes :

* Aller dans *Apparence → Menus*.
* Créer le menu.
* Ajouter des éléments de navigation au menu.
* Associer le menu à l’un des emplacements proposés par le thème. 

**NB:** Les menus ne servent pas uniquement à créer la navigation d'un site. Ils peuvent être utilisés pour gérer une liste de liens, p.ex. une liste de réseaux sociaux (profils Facebook, Twitter, Instagram...). Ou une liste de liens, externes ou internes, que vous souhaitez rendre accessible dans une *Sidebar* ou un *Footer*. Les menus peuvent être placés dans n'importe quelle *Zone de widget* de votre thème.

**NB2:** Si vous ne créez pas de menu, la majorité des thèmes va générer un *menu de navigation automatique*, en listant simplement les *Pages* de votre site, dans l'ordre de leur date de publication.

Widgets
===

Similaires aux Menus, les **Widgets** sont de petits modules pouvant être glissés dans les emplacements que le thème a prévus. Il peut s’agir d’une liste d’articles récents, d’un nuage de mots-clés, d’un formulaire d’abonnement à une newsletter, d’une notice en pied de page...

**NB:** un Widget peut contenir un menu (à condition de l'avoir préalablement créé).

Lors d'un changement un thème, vous ne perdez pas les menus et widgets, mais il sera nécessaire de les associer aux emplacements du nouveau thème.

Voir [le Codex WordPress](https://codex.wordpress.org/fr:Apparence_%C3%89cran_des_Widgets) pour plus de détails sur les différents Widgets.

Les vues archive
==

WordPress produit de manière automatique un certain nombre de vues: 

- La page d'accueil (qui présente plusieurs options).
- Vue d'un article, ou d'une page.
- Page 404 lorsqu'un contenu est introuvable.
- Vue des résultats de recherche.

Certaines de ces vues sont configurées pour présenter un contenu unique:

- Vue d'un article
- Vue d'une page
- Vue d'un fichier attaché

Certaines de ces vues présentent une **liste de contenus**:

- Page d'accueil (si elle n'est pas configurée sur une page, ou modifiée par le thème)
- Vue des résultats de recherche.

Le nombre d'éléments (articles) affichés correspond à ce qui est configuré dans *Réglages -> Lecture*.

Il est important de savoir que de telles vues - une liste de contenus - sont automatiquement générées par WordPress, pour les cas suivants:

- Vue archive par date (jour, mois, année)
- Vue archive par catégorie
- Vue archive par étiquette (tag)
- Vue archive par auteur
- Vue archive par taxonomie personnalisée
- Vue archive par contenu personnalisé

Les pages d’archives par catégorie ou mot-clé peuvent afficher un **descriptif**, si celui a été renseigné lors de la saisie du mot-clé.

Les auteurs
===

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

