---
layout: page
title: Réglages
permalink: /wp/reglages
---

Réglages initiaux d’un site WordPress
---

Quelques réglages initiaux qu’il est utile de faire aussi tôt que possible lors de la mise en place d’un site WordPress:

- Visibilité du site.
- Permaliens.
- Commentaires ouverts ou fermés.

## 1) La visibilité du site

Sous *Réglages → Lecture → Visibilité pour les moteurs de recherche*. Ce réglage permet d’empêcher l’indexation d’un site par les engins de recherche. Votre site n’apparaîtra donc pas dans les résultats de recherche Google. Utile si le contenu du site est bidon et que le site n'est pas prêt. **Attention à ne pas oublier de changer ce réglage lorsque vous finissez la phase développement!**

![Réglage visibilité](/cours-wp/img/config/visibilite-google.png)

## 2) La structure des permaliens

La structure choisie pour les permaliens de votre site aura un impact important sur le placement de votre site dans les résultats de recherche.

Dans la page de configuration *Réglages → Permaliens*, vous pouvez choisir une structure parmi les "réglages courants" proposés. 

La structure recommandée par spécialistes de l’optimisation pour moteurs de recherche (SEO) est la plus simple : *Nom de l’article*.

![Réglage permaliens](/cours-wp/img/config/permaliens.png)

Ainsi le permalien de votre article va ressembler à `monsite.com/recette-tarte-aux-pommes` – il sera à la fois plus parlant pour l’utilisateur, et plus pertinent pour l’indexation par les moteurs de recherche.

NB: dans les versions de WordPress plus anciennes, la structure *Nom de l’article* était déconseillée pour des raisons de performance. Depuis la version 3.3, sortie en décembre 2011, ce problème est résolu ([ticket #16687](https://core.trac.wordpress.org/ticket/16687)), et cette structure peut désormais être utilisée sans pénalisation.

## 3) Commentaires ouverts ou fermés

Décidez si les articles de votre site autoriseront les commentaires, ou pas.

Cette option se trouve dans *Réglages → Discussion*, et s’intitule *Autoriser les visiteurs à publier des commentaires sur les nouveaux articles* (la 3e case). Par défaut, les commentaires sont ouverts sur tous vos articles – ainsi que sur les pages de vos images et fichiers attachés.

Désactivez ce réglage si vous ne souhaitez pas ouvrir les commentaires sur tous vos articles.

Par la même occasion, désactivez la 2ème case: *Autoriser les liens de notification*.

![Options de discussion](/cours-wp/img/config/options-discussion.png)

**Attention :** l’effet de ces réglages n’est pas rétroactif. Les articles déjà publiés ne seront pas affectés. Si vous souhaitez fermer les commentaires sur plusieurs articles déjà publiés, faites ceci :

* Aller dans *Articles → Tous les articles*.
* Si besoin, ouvrir l’onglet *Options de l’écran* et augmenter le nombre d’articles affichés sur chaque page.
* Sélectionner tous les articles concernés.
* Dans le menu *Actions groupées*, choisir *Modifier*. 
* Parmi les options proposées dans le champ *Modifications groupées*, repérer le menu déroulant des Commentaires, et choisir *Refuser* pour fermer les commentaires.
* Cliquer sur le bouton *Mettre à jour* – mission accomplie !

**PS:** si vous souhaitez désactiver complètement les commentaires sur un site, vous pouvez utiliser l'extension [Disable Comments](https://wordpress.org/plugins/disable-comments/), qui fera cela très simplement et proprement.

## 4) Les formats d’images

Configurer les formats des versions *miniatures*, *moyennes* et *grandes* de vos images. Ce réglage se trouve sous *Réglages → Médias*. Les dimensions idéales vont varier en fonction du thème que vous utilisez.

![Tailles par défaut des images](/cours-wp/img/config/medias-default.png)

De manière générale, les valeurs proposées (150 px pour les miniatures, 300 pour les moyennes, 1024 pour les grandes), qui ont été définies en 2008, vont produire des images trop petites selon les standards actuels. Il est donc indiqué d'augmenter ces valeurs lors de la configuration du site.

Voici un exemple de réglage plus approprié:

* **Miniatures:** 500 x 500 px
* **Moyennes:** 1000 x 1000 px
* **Grandes:** 2000 x 2000 px

![Tailles suggérées](/cours-wp/img/config/medias-custom.png)

**Attention:** en cas de modification de ces valeurs, les nouveaux réglages seront pris en compte pour les futurs ajouts uniquement. Ils *ne vont pas s'appliquer* aux images déjà existantes. Pour les images précédemment importées, il faudra "recalculer les miniatures", ce que l'on peut faire au moyen d'une extension (p.ex. *[Regenerate Thumbnails](https://wordpress.org/plugins/regenerate-thumbnails/)*).
