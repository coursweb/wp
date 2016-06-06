---
layout: page
title: Installation
permalink: /wp/installation
---

Installation de WordPress

Ce document indique comment installer un site WordPress chez l'hébergeur o2switch. Chez d'autres hébergeurs, la prodécude sera semblable. Nous utilisons l'installation "one-click" proposée par l'hébergeur, cela nous évite l'étape de création d'une base de données.

1) Choix du nom de domaine. 
=== 

Notre site devra être accessible sous un nom de domaine. Nous avons deux possibilités: un domaine ou un sous-domaine.

Le premier cas sera celui d'un nouveau domaine - **example.com** - que nous aurons réservé auprès d'un Registrar. 

Dans l'interface o2switch, nous devons nous rendre dans la partie concernant la gestion des noms de domaine, pour l'y ajouter.

Dans le deuxième cas, si nous optons pour un sous-domaine - du type **sousdomaine**.example.com - nous allons nous rendre sur l'écran concernant les sous-domaines. Nous allons ajouter un nouveau sous-domaine, en chosissant dans la liste le domaine parent.

2) Choix de la structure des dossiers
===

Durant cette procédure, l'hébergeur nous demande d'indiquer le dossier qui correspondra à ce site. En effet, chaque site faisant partie de l'hébergement pointe vers un endroit spécifique dans la structure des dossiers.

Voici une structure possible, sachant qu'il s'agit d'un hébergement partagé par plusieurs utilisateurs pouvant avoir chacune plusieurs sites. Nous utilisons uniquement des caractères minuscules et sans accents.

/sites/martine/mon-premier-site/web/

Il y a donc quatre niveaux de dossiers:

1. Nous rangeons tous les sites dans le dossier "sites" à la racine du répertoire.
2. Ensuite, chaque utilisateur a un dossier avec son prénom (p.ex. "martine"), qui contiendra ses projets.
3. Troisièmement, chaque site a son propre dossier (p.ex. "mon-premier-site"). Vous êtes libre de choisir son nom.
4. Finalement, la partie "visible sur Internet" du site est située dans le dossier nommé "web". Cela permet d'avoir pour chaque site un espace "non accessible par le web", pour y placer des fichiers de configuration spécifiques au site. Par exemple, le dossier wp-config.php pour un site WordPress.

3) Installation de WordPress
===

Nous pourrions maintenant faire la procédure classique: télécharger le fichier ZIP de la dernière version de WordPress, le dézipper, le mettre en ligne par FTP, créer une base de données, parcourir les étapes de l'installeur de WordPres... 

Mais puisque notre hébergeur propose une interface qui automatise toutes ces étapes, nous pouvons aller encore plus vite.

Rendez-vous dans la partie permettant d'installer des applications:

Choisissez l'installation de WordPress.

Il vous faut à présent renseigner quelques champs:

- Choisir **le nom du site**. Ce nom pourra être changé à tout moment. Il s'agit d'un champ pouvant contenir accents et charactères spéciaux.
- Répertoire: veillez à ce que le champ soit vide, sinon WordPress sera installé dans un sous-répertoire du site, comme ceci: example.com/wp.
- Choisir un **nom d'utilisateur**. Ça pourrait être votre prénom, mais évitez d'utiliser "admin". Attention, cet identifiant *ne pourra pas* être changé (même si vous pourrez ajouter de nouveaux utilisateurs à volonté).
- Choisir un **mot de passe**. Sachant que ce login sera certainement la cible de tentatives d'intrusion quotidiennes par des robots spammeurs, vous avez tout intérêt à chosir un mot de passe suffisamment long et unique pour résister à ces attaques.

Cliquez sur installer ... et votre site est prêt, vous pouvez à présent vous connecter à l'espace d'administration et vous occuper des [réglages initiaux](reglages).

***