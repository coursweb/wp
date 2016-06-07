---
layout: page
title: Modifier un thème
permalink: /wp/modifier
---

Modifier un thème WordPress
---

Ayant choisi un thème WordPress pour votre site, il y a de fortes chance que vous ayez envie de faire des modifications graphiques, par exemple de masquer certaines indications.

Notamment, les "métadonnées" des articles, comme l'auteur, la date de publication, les catégories et étiquettes, sont des éléments qu'i peuvent qu'on peut souhaiter masquer.

Voilà une demande typique:

> Comment modifier le design de mon site? Il y a deux-trois petites choses dont je ne vois pas l'intérêt, comme typiquement les dates apparentes sur les titres de ma page d'accueil, ou encore les différents tags et "posté sous" qui apparaissent.

Plusieurs solutions
===

Pour supprimer ces éléments inutiles, plusieurs approches sont possibles:

- Intervention en surface: masquer les éléments avec des **styles CSS personnalisés**.
- Intervention en profondeur: modifier les templates du thème utilisé, idéalement en utilisant un [thème enfant](theme-enfant).

Nous allons ici explorer la première solution, probablement plus simple à mettre en œuvre.

CSS personnalisé
===

Voilà comment nous allons procéder, en trois étapes:

1. Trouver un moyen d'ajouter du CSS personnalisé à notre site.
2. Identifier les éléments de code que nous souhaitons masquer.
3. Ecrire le CSS nécessaire pour masquer ces éléments.

Pour commencer, nous devons trouver un moyen de créer du CSS personnalisé. Pour cela, diverses possibilités:

<h4>Avec Jetpack</h4>

Le "CSS Personnalisé" est l'une des nombreuses fonctionnalités de l'extension **Jetpack**. Donc, si vous utilisez déjà cette extension, vous n'avez plus qu'à activer cette fonctionalité.

![Activation du CSS Personnalisé](/cours-web/cours-wp/img/jetpack-css.png)

Une fois cette option activée, vous allez trouver une nouvelle entrée dans le menu *Apparence : Modifier le CSS*.

![](/cours-web/cours-wp/img/jetpack-css-menu.png)

Cela vous donnera accès à un champ nommé *Editeur de Feuille de Style CSS*. Tous les styles que vous ajoutez ici seront chargés dans l'en-tête de votre site. C'est donc un bon moyen de surchager les styles de votre thème.

![](/cours-web/cours-wp/img/jetpack-css-editor.png)

<h4>Sans Jetpack</h4>

Si vous n'utilisez pas l'extension Jetpack, vous pouvez opter pour une solution plus simple: **[Simple Custom CSS](https://wordpress.org/plugins/simple-custom-css/)** est une extension qui, comme son nom l'indique, vous permet d'ajouter simplement du CSS "custom".

Une fois l'extension installée et activée, vous allez trouver une nouvelle entrée dans le menu *Apparence : Custom CSS*.

![](/cours-web/cours-wp/img/simple-custom-css.png)

Comme pour Jetpack, cette extension vous propose un champ permettant d'entrer votre CSS personnalisé:

![](/cours-web/cours-wp/img/simple-custom-css-field.png)

Trouver le code à modifier
===

Maintenant que nous avons la technique en place, nous devons trouver quel est le code correspondant à l'élément que nous souhaitons masquer.

Supposons que nous utilisons le thème Cubic, dont voici [la page de démonstration](https://cubicdemo.wordpress.com/).

![Le thème Cubic](/cours-web/cours-wp/img/cubic-homepage.jpg)

Admettons que la présence des dates nous déplait, et que nous souhaitons les masquer.

Nous allons utiliser l'inspecteur de notre navigateur, pour détecter les *identifiants* ou *classes* à utiliser pour masquer la date.

Faites un clic-droit sur l'élément que vous souhaitez investiguer, et choisissez "Inspecter".

![](/cours-web/cours-wp/img/chrome-inspect.jpg)







