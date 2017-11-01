---
layout: page
title: Les types de contenus
permalink: /wp/custom-post-types
---

WordPress propose certains contenus par défaut – articles, pages, médias – mais il est possible d’ajouter des types de contenus supplémentaires. Recettes de cuisine, produits, objets immobiliers... tout dépendra des besoins spéfiques de votre site. Ces contenus spécifiques sont appelés des **Custom Post Types**.

De la même manière, WordPress propose deux systèmes de classification pour vos articles : les **catégories** et les **mots-clés**. On appelle ces classifications des **taxonomies**.

Un moyen pratique pour créer des types de contenus (CPT) et taxonomies personnalisées : le plugin Custom Post Type UI.
[http://wordpress.org/plugins/custom-post-type-ui/](http://wordpress.org/plugins/custom-post-type-ui/)

Exercice: 
===

Un blogeur écrit des critiques de livres, de films et de jeux. 

* Créer pour cela une **taxonomie** custom, "Critiques" 
* Les critiques seront des articles WordPress, les termes de la taxonomie seront « livres », « films », « jeux ».
* Dans une zone Sidebar, créer un **widget** pour cette Taxonomie. Ce **widget** peut contenir un **menu**, comprenant les pages d’archive des ”livres, films, jeux”.

## Déclaration d'un Custom Post Type

Pour déclarer un nouveau Custom Post Type, il faut utiliser la fonction [`register_post_type`](https://codex.wordpress.org/Function_Reference/register_post_type), dans un thème ou un plugin.

Si vous n'êtes pas à l'aise avec le code PHP, vous pouvez utiliser l'extension [Custom Post Type UI](https://wordpress.org/plugins/custom-post-type-ui/).

### Choisir le nom d'un Custom Post Type

Quand vous spécifiez le nom de votre *Custom Post Type*, veillez à ne pas utiliser un nom déjà utilisé par WordPress. Cette page de documentation indique une liste de termes à éviter: 

* post
* page
* attachment
* revision
* nav_menu_item
* custom_css
* customize_changeset
* action
* author
* order
* theme

Une autre question qui se poste: faut-il utiliser le **singulier** ou le **pluriel**? P.ex. si vous ajoutez un type de contenu "Projets", faut-il que son identifiant soit "projet" ou "projets"? 

La pratique habituelle est d'utiliser le singulier. Cela donne des URL plus courtes, et c'est plus cohérent: en effet, l'URL "projet/nom-du-projet" affichera **un** projet à la fois.


## L'option Portfolios avec Jetpack

L'extension **Jetpack** offre une option *Portfolios*, qui permet entre autres de présenter des projets sous forme de galerie d'images. Cette option n’est toutefois compatible qu’avec certains thèmes Wordpress.

* Une fois l'extension Jetpack installée, celle-ci apparaît dans votre tableau de bord Wordpress. Cliquez dessus, puis allez dans *Réglages*.
* Jetpack vous propose ici diverses fonctionnalités pour votre site internet. Cliquez sur l'onglet *Writing*, puis scrollez jusqu'à la catégorie *Types de contenus personnalisés*. Activez la deuxième option: *Portfolios*.
* Rechargez votre page. Un onglet *Portfolio* doit maintenant se trouver dans votre tableau de bord.
* Depuis cet onglet, vous pouvez créer des *Projets*, qui fonctionnent plus ou moins comme des *Articles*. 
* Afin de présenter vos *Projets* sous forme de galerie d'images, vous devez à présent créer une *Page*, puis dans *Attributs de page* choisir le *Modèle de page du portefeuille* (cela peut varier selon le thème). 
* Vous pouvez également classer vos projets par *Types de projets*. Dans l'onglet *Portfolios* de votre tableau de bord, cliquez sur *Types de projets*, puis créez un nouveau type. Lorsque vous créerez un nouveau projet, vous pourrez maintenant lui attribuer un type, ce qui facilitera la navigation à travers vos différents projets.

Quelques thèmes qui utilisent les Porfolios:

* [Argent](https://wordpress.com/theme/argent), par Mel Choyce (Automattic)
* [Blask](https://wordpress.com/theme/blask), par Mel Choyce (Automattic)
* [Illustratr](https://wordpress.com/theme/illustratr), par Thomas Guillot (Automattic)
* [Zeitreise](https://www.elmastudio.de/en/themes/docs/zeitreise/), par Elmastudio
