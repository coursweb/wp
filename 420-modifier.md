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

- **Intervention en surface:** masquer les éléments avec des **styles CSS personnalisés**.
- **Intervention en profondeur:** modifier les templates du thème utilisé, idéalement en utilisant un [thème enfant](theme-enfant).

Nous allons ici explorer la première solution, plus simple à mettre en œuvre.

CSS personnalisé
===

Voilà comment nous allons procéder, en trois étapes:

1. Trouver un moyen d'ajouter du CSS personnalisé à notre site.
2. Identifier les éléments de code que nous souhaitons masquer.
3. Ecrire le CSS nécessaire pour masquer ces éléments.

Pour commencer, nous devons trouver un moyen de créer du CSS personnalisé. Depuis la version 4.7 (fin 2016), il est possible de faire cela avec l'outil *Personnaliser*. Il n'est donc plus nécessaire de recourir à des extensions comme Jetpack.

Vous trouverez cette option sous *Apparence > Personnaliser*, dans la section nommée *CSS additionnel*. Tous les styles que vous ajoutez ici seront chargés dans l'en-tête de votre site. C'est donc un bon moyen de surchager les styles de votre thème.

![Ajout de CSS additionnel](/cours-wp/img/wp-customizer-css-fr.png)

Votre CSS personnalisé sera sauvegardé séparément pour chacun de vos thèmes.

Trouver le code à modifier
===

Maintenant que nous avons la technique en place, nous devons trouver quel est le code correspondant à l'élément que nous souhaitons masquer.

Supposons que nous utilisons le thème Cubic, un thème développé par [Thomas Guillot](https://thomasguillot.com/2015/01/16/new-theme-cubic/) pour Automattic, dont voici [la page de démonstration](https://cubicdemo.wordpress.com/).

![Le thème Cubic](/cours-wp/img/cubic-homepage.jpg)

Supposons que la présence des dates de publication au-dessus des titres nous déplait, et que nous souhaitons les masquer.

Nous allons utiliser l'inspecteur de notre navigateur, pour détecter les *identifiants* ou *classes* à utiliser pour masquer la date.

Faites un clic-droit sur l'élément qui vous intéresse, et choisissez "Inspecter".

![](/cours-wp/img/chrome-inspect.jpg)

Avec l'aide de l'inspecteur, vous pouvez parcourir le code, et vérifier comment se nomme l'élément à masquer.

![](/cours-wp/img/inspection-code.png)

Ici, nous voyons que l'élément `<header class="entry-header">`contient à la fois la date et le titre. L'élément `<div class="entry-meta">` contient la date uniquement. 

C'est donc cet élément que nous souhaitons masquer. Nous allons le cibler en utilisant sa classe, `.entry-meta`.

Voyons ce qui se produit si nous ajoutons le code suivant à notre CSS custom:

```css
.entry-meta {
    display: none;
}
```

Note: la propriété [`display`](https://developer.mozilla.org/fr/docs/Web/CSS/display) avec la valeur `none` permet de masquer un élément.

![](/cours-wp/img/resultat-1.jpg)

Résultat: la date est effectivement masquée... mais l'absence d'espacement au-dessus du titre est plutôt disgrâcieux.

L'inspecteur nous indique que la marge du bas (padding-bottom) est de 6px... et que la marge du haut est tronquée par le code suivant:

```css
.entry-meta + .entry-title a {
    padding-top: 0;
    margin-top: -6px;
}
```

Nous allons reprendre ce code, en modifiant les valeurs:

```css
.entry-meta + .entry-title a {
    padding-top: 6px;
    margin-top: 0px;
}
```

Ajoutons ce code à notre CSS custom, et obervons le résultat:

![](/cours-wp/img/dates-masquees.jpg)

Un détail: nous aurions pu ajouter cette marge sur un autre élément, comme `.entry-header`, ou `.entry-title` — cela donnerait le même résultat visuellement. Pourquoi avoir choisi de le mettre sur `.entry-title a`? 

C'est simple: étant donné que le `<a>` est l'élément réagissant au clic, en attribuant la marge à cet élément, nous *agrandissons* la zone "sensible" - nous améliorons ainsi l'usabilité, p. ex. pour un usager de tablette tactile.

Un deuxième exemple...
===

Après ce premier succès, intéressons-nous aux pages individuelles des articles. Nous pouvons voir que chaque article comporte une section "Posté dans... Tagué..." qui peut paraître superflue.

![](/cours-wp/img/entry-footer.jpg)

Ici encore, l'inspecteur nous révèle le nom de cette zone:

```html
<footer class="entry-footer">
```

Essayons le code CSS custom suivant:

```css
.entry-footer {
    display: none;
}
```

Cela fonctionne, ces métadonnées sont désormais masquées. Le seul point dérangeant est la marge qui devient trop étroite (24px pour la marge du bas, alors que celle du haut est de 72px).

![](/cours-wp/img/inspect-single.jpg)

On peut voir dans le code que les 72px sont définis de la manière suivante:

```css
@media screen and (min-width: 768px) {
    .entry-content {
        padding-top: 72px;
    }
}
```

Il s'agit donc d'une Media Query, produisant cette marge supérieure de 72px si la taille de la fenêtre est de 768px ou plus (voir: [Media Queries](http://cours-web.ch/css/responsive) dans le chapitre CSS).

Nous pouvons reprendre ce code, et modifier la valeur: comme il y a déjà une marge de 24px, nous allons **ajouter 48px** pour que le total soit de 72px.

Voilà le code que nous ajoutons à notre custom CSS:

```css
@media screen and (min-width: 768px) {
    .entry-content {
        padding-bottom: 48px;
    }
}
```

Résultat: nous avons maintenant des marges inférieures et supérieures parfaitement ajustées.

Conclusion
===

Il est relativement aisé, en se servant de l'inspecteur du navigateur, de trouver les classes CSS des éléments que l'on souhaite masquer ou modifier.

La méthode décrite ici a toutefois ses limites:

- Vous ne pouvez pas faire de **versionnement** de votre code.
- Vous ne bénéficiez pas des automatismes d'un éditeur de code (comme [Atom](https://atom.io/) ou [Sublime Text](https://www.sublimetext.com/)) qui pourrait vous aider à écrire du CSS correct.
- Vous ne pouvez pas diviser votre code en plusieurs feuilles de style.
- Vous ne pouvez pas modifier les templates ou fonctions du thème.

Pour éviter ces limitations et élargir les possibilités de personnalisation, il est recommandé de créer [un thème enfant](theme-enfant).