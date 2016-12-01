---
layout: page
title: Troubleshooting
permalink: /wp/troubleshooting
---

Comment résoudres des problèmes...

Identifiant de WordPress oublié:

* Avec [MAMP](installation-mamp), aller dans PhpMyAdmin
* Aller dans la base de données utilisée par WordPress
* Aller dans la table wp_users (ou prefix_users)
* Veiller à ce que l'onglet soit "Afficher" (et non pas "Structure").
* Vous verrez une liste d'un ou plusieurs utilisateurs... sélectionner le votre en cochant la case, puis cliquer sur "modifier"
* Repérer le champ "user_pass": entrer le nouveau mot de passe souhaité, et choisir dans le menu déroulant sous Fonction: "MD5".
* Cliquer sur "exécuter".

Vous pouvez maintenant retourner sur votre page de login WordPress, et vous connecter avec votre utilisateur en entrant le nouveau mot de passe.

Il est aussi possible de créer de manière similaire un nouvel utilisateur, voir [ce mode d'emploi](http://www.wpbeginner.com/wp-tutorials/how-to-add-an-admin-user-to-the-wordpress-database-via-mysql/).