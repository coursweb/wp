---
layout: page
title: Installation Hostpoint
---

Ce document indique comment installer un site WordPress chez l'hébergeur [Hostpoint](https://www.hostpoint.ch/fr/). Chez d'autres hébergeurs, la procédure sera relativement semblable. Nous utilisons l'installation "one-click" proposée par l'hébergeur.

## 1) Réglages DNS

Si votre [nom de domaine](/divers/domaines/) a été créé chez un autre registrar – p.ex. Infomaniak, Gandi, ou Freenom – vous devrez commencer par effectuer un réglage DNS.

Voici comment faire cette configuration chez Infomaniak:

- Connectez vous à la [console d'administration](https://manager.infomaniak.com) (sur la page d'accueil, cliquer *Connexion > Manager*).
- Rendez-vous dans **Noms de domaine**, cliquez sur le domaine, puis sur **Gestion des DNS**.

![Choisir Gestion des DNS](/cours-wp/img/hostpoint/Infomaniak_dns0.png)

- Cliquez "Modifier les serveurs DNS"
- Remplacez les réglages existants par les serveurs de noms suivants :

```
ns.hostpoint.ch
ns2.hostpoint.ch
ns3.hostpoint.ch
```

Décochez la case "Vérifier la disponibilité des serveurs DNS".

Voilà, c'est fait! C'est tout ce qui est nécessaire du côté d'Infomaniak. La suite se passe chez Hostpoint!

## 2) Réglages Hostpoint

Pour commencer, allez à [https://admin.hostpoint.ch/](https://admin.hostpoint.ch/) et connectez-vous.

### a) Ajouter votre nom de domaine

- Dans la barre de navigation, cliquer sur **[Domaines](https://admin.hostpoint.ch/customer/Domains/Overview)**.
- En bas de la liste, cliquer sur **Ajouter un domaine**.
- Ajouter votre domaine.

### b) Créer un site

- Dans la barre de navigation, aller dans **Services**, choisissez votre serveur et cliquez Ouvrir, puis **Sites Web** dans le menu de gauche. Vous pouvez aussi simplement aller à cette page: [https://admin.hostpoint.ch/customer/Websites/Overview](https://admin.hostpoint.ch/customer/Websites/Overview)

- Dans **Sites Web**, au bas de la liste, cliquer **Créer un site web**.
- Choisir votre nom de domaine.
- Entrez le chemin du répertoire qui contiendra votre site, selon ce modèle: `prenom/nomdusite.com/web`

![Définition du répertoire](/cours-wp/img/hostpoint/chemin-repertoire.png)

Voici les trois niveaux de dossiers utilisés dans cette configuration:

1. Chaque utilisateur a un dossier avec son prénom (p.ex. `martine`), qui contiendra ses projets.
2. Deuxièmement, chaque site aura son dossier (p.ex. `monsite.com`).
3. Finalement, la partie "visible sur Internet" du site est située dans le dossier nommé `web`. Cela permet d'avoir pour chaque site un espace "non accessible par le web", pour y placer des fichiers de configuration spécifiques au site. Par exemple, le fichier [`wp-config.php`](http://codex.wordpress.org/Hardening_WordPress#Securing_wp-config.php) pour un site WordPress.

### c) Installer WordPress:

Votre site est créé, il reste encore à installer WordPress. Voici la marche à suivre:

- Aller dans **Sites Web: Applications**
- Cliquer sur **Applications Disponibles**

![Comment installer WordPress](/cours-wp/img/hostpoint/hostpoint-applications.png)

- Choisir **WordPress > Installer**.
- Choisir votre nom de domaine dans la liste. 
- Ne PAS cocher l'option "Installer WordPress en sous-dossier".
- Accepter les conditions générales.
- Installer!

**Important:** à la fin de l'installation, une page d'informations vous affichera le **nom d’utilisateur** et **mot de passe** de votre site WordPress. Copiez ces informations, car *c'est le seul moment* où vous les verrez affichées!

![Infos de connexion](/cours-wp/img/hostpoint/infos-wp.png)

Vous pouvez désormais vous connecter à votre site WordPress, en visitant l'interface d'administration sous `nomdusite.com/wp-admin`.
