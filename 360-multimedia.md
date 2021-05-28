---
layout: page
title: Multimédia
permalink: multimedia.html
---

# Fichiers multimedia

- Vidéos
- Audio
- Fichiers joints

## Fichiers multimédia

WordPress vous permet d'ajouter des fichiers vidéo et audio à vos articles. WordPress inclut un lecteur qui affichera les fichiers audio (mp3) ou vidéo (mp4) sur la partie publique du site.

Pour insérer une vidéo depuis Youtube ou Vimeo (ou DailyMotion, et des dizaines d'autres services), il suffit d’insérer le lien de cette vidéo dans le corps de votre article. WordPress va automatiquement produire le lecteur vidéo correspondant.

Cette méthode d'insertion porte le nom technique "oEmbed". Dans le code de WordPress ([wp-includes/class-oembed.php](https://github.com/WordPress/WordPress/blob/master/wp-includes/class-oembed.php#L137)) se trouve la liste de tous les services pris en charge (55 en fin 2017).


### Fichiers joints

Hormis les images, il est possible d'ajouter des fichiers à vos articles (documents au format PDF, Word, Zip...). WordPress comprend une liste de formats ”autorisés” (plus de 90 types de document), qui peut être modifiée ou étendue par un plugin si nécessaire. P.ex. le format EPUB n'est pas autorisé par défaut.

La liste complète des formats est visible dans le code, vous pouvez la consulter dans [wp-includes/functions.php](https://github.com/WordPress/WordPress/blob/master/wp-includes/functions.php#L2510) - `function wp_get_mime_types()`.



