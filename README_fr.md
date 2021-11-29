# Funkwhale pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/funkwhale.svg)](https://dash.yunohost.org/appci/app/funkwhale) ![](https://ci-apps.yunohost.org/ci/badges/funkwhale.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/funkwhale.maintain.svg)  
[![Installer Funkwhale avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=funkwhale)

*[Read this readme in english.](./README.md)*
*[Lire ce readme en français.](./README_fr.md)*

> *Ce package vous permet d'installer Funkwhale rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

Funkwhale est un projet communautaire qui vous permet d'écouter et de partager de la musique et de l'audio au sein d'un réseau ouvert et décentralisé. 

**Version incluse :** 1.1.4~ynh2

**Démo :** https://demo.funkwhale.audio

## Captures d'écran

![](./doc/screenshots/screenshot1.png)

## Avertissements / informations importantes

* L'installation nécessite un domaine ou un sous-domaine dédié. L'installation dans un chemin du domaine n'est pas prise en charge par le projet en amont en raison des exigences de dépendance.

* Admin

L'administrateur utilise le login que vous avez fourni lors de l'installation. Le mot de passe est le même que celui que vous utilisez pour YunoHost.

L'interface d'administration est accessible à l'adresse : votre.domaine.fr/api/admin
Pour ajouter une collection de fichiers musicaux à une bibliothèque dans votre installation YunoHost de Funkwhale, créez un lien symbolique vers votre collection intitulée "music" dans `/home/yunohost.app/funkwhale/data/`.
`foo@bar:~$sudo ln -s /your/music/collection /home/yunohost.app/funkwhale/data/music`
Les fichiers peuvent ensuite être ajoutés à votre bibliothèque à partir de l'onglet *Envoi* dans une bibliothèque musicale sous la rubrique **Importer de la musique de votre serveur**.

## Documentations et ressources

* Site officiel de l'app : https://funkwhale.audio/
* Documentation officielle utilisateur : https://docs.funkwhale.audio/users/index.html
* Documentation officielle de l'admin : https://docs.funkwhale.audio/admin/index.html
* Dépôt de code officiel de l'app : https://dev.funkwhale.audio/funkwhale
* Documentation YunoHost pour cette app : https://yunohost.org/app_funkwhale
* Signaler un bug : https://github.com/YunoHost-Apps/funkwhale_ynh/issues

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/funkwhale_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/funkwhale_ynh/tree/testing --debug
ou
sudo yunohost app upgrade funkwhale -u https://github.com/YunoHost-Apps/funkwhale_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** https://yunohost.org/packaging_apps