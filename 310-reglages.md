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

1) La visibilité du site
==

Sous *Réglages → Lecture → Visibilité pour les moteurs de recherche*. Ce réglage permet d’empêcher l’indexation d’un site par les engins de recherche. Votre site n’apparaîtra donc pas dans les résultats de recherche Google. Utile si le contenu du site est bidon et que le site n'est pas prêt. **Attention à ne pas oublier de changer ce réglage lorsque vous finissez la phase développement!**

2) La structure des permaliens
==

La structure choisie pour les permaliens de votre site aura un impact important sur le placement de votre site dans les résultats de recherche.

Dans la page de configuration *Réglages → Permaliens*, vous pouvez choisir une structure parmi les "réglages courants" proposés. 

La structure recommandée par spécialistes de l’optimisation pour moteurs de recherche (SEO) est la plus simple : *Nom de l’article*. 

Ainsi le permalien de votre article va ressembler à `monsite.com/recette-tarte-aux-pommes` – il sera à la fois plus parlant pour l’utilisateur, et plus pertinent pour l’indexation par les moteurs de recherche.

NB: dans les versions de WordPress plus anciennes, la structure *Nom de l’article* était déconseillée pour des raisons de performance. Depuis la version 3.3, sortie en décembre 2011, ce problème est résolu (ticket #16687), et cette structure peut désormais être utilisée sans pénalisation.

3) Commentaires ouverts ou fermés
==

Décidez si les articles de votre site permettront généralement des commentaires, ou pas.

Cette option se trouve dans *Réglages → Discussion*, et s’intitule Autoriser les visiteurs à publier des commentaires sur les derniers articles. Par défaut, les commentaires sont ouverts sur tous vos articles – ainsi que sur les pages de vos images et fichiers attachés.

Désactivez ce réglage si vous ne souhaitez pas ouvrir les commentaires sur tous vos articles. 

Attention : l’effet de ce réglage n’est pas rétroactif. Les articles déjà publiés ne seront pas affectés. Si vous souhaitez fermer les commentaires sur plusieurs articles déjà publiés, faites ceci :

* Aller dans *Articles → Tous les articles*.
* Si besoin, ouvrir l’onglet *Options de l’écran* et augmenter le nombre d’articles affichés sur chaque page (20 par défaut).
* Sélectionner tous les articles concernés.
* Dans le menu *Actions groupées*, choisir *Modifier*. 
* Parmi les options proposées dans le champ *Modifications groupées*, repérer le menu déroulant des Commentaires, et choisir *Refuser* pour fermer les commentaires.
* Cliquer sur le bouton *Mettre à jour* – mission accomplie !

4) Les formats d’images
==

Configurer les formats des versions *miniatures*, *moyennes* et *grandes* de vos images. Ce réglage se trouve sous *Réglages → Médias*. Les dimensions idéales vont varier en fonction du thème que vous utilisez.

De manière générale, les valeurs proposées risquent de produire des images un peu trop petites pour le standards de 2016. Voici un réglage qui paraît plus approprié:

* **Miniatures:** 500 x 500 px
* **Moyennes:** 900 x 900 px
* **Grandes:** 2000 x 2000 px

Attention: en cas de modification de ces valeurs, les nouveaux réglages seront pris en compte pour les futurs ajouts, mais *ne vont **pas** s'appliquer* aux images déjà existantes. Si des images ont déjà été importées, il faudra "recalculer les miniatures", ce que l'on peut faire au moyen d'un extension.
