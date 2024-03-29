---
layout: page
title: Images
permalink: images.html
---

WordPress permet d’ajouter des médias (images, fichiers audio et vidéo, etc) à vos contenus.

Images
---

Petit rappel : il existe de nombreux formats d’image, et tous ne sont pas adaptés au web. Les navigateurs actuels pourront afficher les formats suivants : 

* **JPEG** (ou JPG), généralement recommandé pour des images photographiques (la majorité de vos images). 
* **PNG**, un format de compression sans perte, recommandé pour préserver des aplats de couleurs. Par exemple certaines images vectorielles, ou des captures d’écrans de logiciels, pourront bénéficier d’un meilleur rendu.
* **GIF**, similaire au PNG. Possibilité de contenir une série d’images (les fameux GIFs animés).

Mis à part ces trois formats, tous les autres formats d’images (TIFF, PSD, BMP, PICT...) ne seront *pas affichés* par un navigateur. Ils seront traités comme un simple fichier attaché.

La taille des images
===

Il faudra prêter attention à la taille de vos images, en terme de poids (en Kb ou Mb) et en terme de format (nombre de pixels).

Les dimensions optimales des images vont dépendre de la mise en page de votre thème WordPress.

Les formats configurés
===

WordPress crée trois tailles supplémentaires de votre image uploadée (*miniature*, *moyenne*, *grande*). Les dimensions sont définies lors de la [configuration du thème](reglages).

Choisir la taille insérée en fonction de vos besoins, mais surtout en fonction du thème. Généralement, la taille moyenne sera la plus appropriée.

Pour reformater un grand nombre d’images (p.ex. suite à un changement de thème), le  plugin **[Regenerate Thumbnails](http://wordpress.org/plugins/regenerate-thumbnails/)** facilite l’opération.

Attention: Si vous mettez en ligne des images de très grand format (5000 x 4000 pixels et au-delà), il se peut que votre serveur ne parvienne pas à calculer les versions miniatures. Il affichera dans ce cas la version originale, dont le poids va considérablement ralentir le chargement de votre site. Veillez donc à mettre en ligne des images de taille raisonnable. Le format vidéo HD actuel – 1920 pixels de large – est une limite supérieure appropriée pour les écrans actuels.

Vous pouvez utiliser une extension comme "[Resize Image After Upload](https://fr.wordpress.org/plugins/resize-image-after-upload/)" pour limiter la taille des images.

Définir une image « à la une »
===

Votre thème peut utiliser la fonction « image à la une ». Si c’est le cas, vous verrez un champ correspondant apparaître dans l’interface d’édition des articles. 

Insertion d'images
===

Il y a deux manières d'insérer des images dans WordPress.

**Insérer une image unique.**

Il est possible d'insérer une suite d'images, puis de rédiger l'article entre les images.

**Insérer une galerie d’images.**

Voir aussi : 

* Patrick Finot, *[La gestion des images dans WordPress](http://www.informatique-enseignant.com/gestion-images-wordpress/)*, septembre 2013 

## Extensions pour les galeries d'images

Quelques extensions qui améliorent l'expérience des galeries, en appliquant une fenêtre modale de type "Lightbox".

- [Jetpack](https://wordpress.org/plugins/jetpack/), qui inclut un [Carousel](https://jetpack.com/support/carousel/) pour les galeries. Propose des vues en mosaique (effet Masonry).
- [Lightbox with PhotoSwipe](https://wordpress.org/plugins/lightbox-photoswipe/).
- [WP Featherlight](https://wordpress.org/plugins/wp-featherlight/)
- [Liste des extensions](https://wordpress.org/plugins/tags/lightbox/) avec le tag "lightbox".

Voir aussi la documentation concernant les librairies JavaScript Lightbox.

TODO: 

- reformater, crop d'une image.
- galeries d'images.
- lier vers l'image (fichier) ou "attachment page".

Exercices: 

* insérer une image unique.
* insérer une suite d'images, écrire du texte entre les images.
* insérer un lien vers une vidéo Youtube.