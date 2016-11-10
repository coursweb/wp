---
layout: page
title: Installation MAMP
permalink: /wp/installation-mamp
---

Ce document indique comment installer un site WordPress localement (sur votre ordinateur) avec [MAMP](https://www.mamp.info/en/).

- Télécharger MAMP, installer.
- Au premier lancement, MAMP vous proposera de lancer MAMP PRO. Optez pour MAMP, la version gratuite.
- Dans la fenêtre de lancement de MAMP, aller dans les préférences.
- Cliquer sur l'onglet "Web Server".
- Cliquer sur l'icone du dossier (à côté de Document Root) et naviguez vers votre emplacement de travail, pour définir le dossier racine qui qui sera utilisé par MAMP. Confirmer.

### Base de données MySQL

Créer la base de données MySQL qui sera utilisée par WordPress:

- Cliquer sur "Démarrer les serveurs".
- Cela va vous amener à la "WebStart Page" (localhost:8888/MAMP/?language=French)
- Sous MySQL, noter les informations de compte par défaut:
- Hôte: localhost
- Port: 8889
- User: root
- Mot de passe: root
- Ouvrir PhpMyAdmin, en cliquant sur l'un des liens phpMyAdmin
- Créer une base de données (cliquer sur "Nouvelle base de données" dans le menu de gauche)
- Lui donner un nom, p.ex. `wordpress`
- Cliquer sur "créer".
- La nouvelle base de données apparaitra dans le menu de gauche (on verra le message "Aucune table n'a été trouvée dans cette base de données"... c'est normal).
- Vous pouvez fermer cette fenêtre et passer à l'opération suivante:

### Obtenir WordPress: 

- Aller à l'adresse [https://fr.wordpress.org/](https://fr.wordpress.org/)
- Téléchargez la version actuelle de WordPress
- Dézippez (si ce n'est pas fait automatiquement), et déplacez le dossier "wordpress" dans le dossier "Fichiers MAMP" que vous avez créé précédemment.
- Retournez dans le panneau MAMP, cliquez sur "Open WebStart Page".
- Arrivé sur la WebStartPage, cliquez dans le menu sur "Mon Site Web".
- Vous arriverez sur la page localhost:8888, et devriez voir le nom du dossier wordpress.
- Cliquez sur ce lien, et vous arriverez sur la page qui lance l'installation de WordPress.
- Adresse de la base de données: correspond au champ Hôte (localhost)
- Nom de la base de données: le nom que vous avez indiqué en créant la base de données ("wordpress").
- Identifiant: correspond à l'Utilisateur MySQL = root
- Le mot de passe: root
- Le préfixe des tables: on peut laisser
- Terminez l'installation.

Un tutoriel complet en anglais:

[https://www.wpmayor.com/how-to-install-wordpress-locally-on-mac-with-mamp/](https://www.wpmayor.com/how-to-install-wordpress-locally-on-mac-with-mamp/)

Note concernant Jetpack:

Pour certains thèmes, il faut installer l'extension Jetpack. Jetpack pourra vous demander l'activation du *Custom Content Types Module*. Pour cela, il faut aller dans le menu: *Jetpack > Settings*, puis dans l'onglet *Writing*. Parmi les différents modules proposées, activer celui qui se nomme "Custom Content Types".


***