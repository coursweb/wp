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

Catégories, mots-clés (et taxonomies)
===

Afin d'organiser vos contenus, WordPress utilise le concept de "taxonomie", càd un système de classification pour subdiviser les articles en unités plus gérables.

Les **catégories** et **mots-clés** sont les deux systèmes de classement (taxonomies) actifs par défaut. Il est possible d’en rajouter d’autres selon les besoins – on parlera alors de *custom taxonomies*.

**Pour plus de détails:** voir la présentation de Benjamin Lupu, "[Architecture de l’information pour WordPress](https://wordpress.tv/2016/04/05/benjamin-lupu-architecture-de-linformation-pour-wordpress/)", au WordCamp Paris 2016.

Post Formats
===

Certains thèmes permettent l’utilisation des « formats d’articles » (*Post Formats*), qui permettent une présentation visuelle différente pour certains formats prédéfinis, p.ex. *En passant, Image, Vidéo, Son, Citation, Lien, Galerie*. Ces formats sont appliqués aux Articles, à la manière des Catégories et Mots-clés.

Ces *Post Formats* sont différents des *Custom Post Types*, qui permettent d’ajouter de nouveaux types de contenus à un site, en plus des Articles et Pages (p.ex. un plugin de gestion d’événements pourra ajouter un type de contenu *Evénement*).

Menus
===

Les **menus** sont un élément spécifique, que vous pourrez administrer en vous rendant sous *Apparence > Menus*. Votre thème proposera un ou plusieurs emplacements pouvant accueillir des menus de navigation. La procédure de création d'une menu passe par ces étapes :

* Aller dans *Apparence → Menus*.
* Créer le menu.
* Ajouter des éléments de navigation au menu.
* Associer le menu à l’un des emplacements proposés par le thème. 

Widgets
===

Similaires aux Menus, les **Widgets** sont de petits modules pouvant être glissés dans les emplacements que le thème a prévus. Il peut s’agir d’une liste d’articles récents, d’un nuage de mots-clés, d’un formulaire d’abonnement à une newsletter, d’une notice en pied de page...

Note : un widget peut contenir un menu.

Lors du changement un thème, vous ne perdez pas les menus et widgets, mais il sera nécessaire de les associer aux emplacements du nouveau thème.

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

