# BETA ComputerZ Solutions

**TODO - WORK IN PROGRESS**

Le renouveau du site web est en marche ! Avec cette nouvelle version, le futur arrive !

Ici, pas de découverte/présentation du CMS hugo, uniquement la mise en place et la configuration effectuée pour ComputerZ Solutions

## Installation et préparation de hugo

**TODO - WORK IN PROGRESS**

Avant d'exploiter Hugo, installons quelques outils pratiques (à modifier selon votre usage et vos besoins)

```bash
# Debian based distributions
apt install git rsync hugo

# Archlinux based distributions
pacman -S git rsync hugo
```

Utilisons maintenant les commandes `hugo` pour créer un nouveau site, initialisons le dépôt git et commençons le travail.

```bash
cd ~/hugo new site beta-czs
cd beta-czs
git init
```

Une configuration basique est alors générée, avec le strict nécessaire pour pouvoir lancer le site web. Par défaut, grâce au serveur intégré dans hugo, vous pourrez accéder à votre site via `http://localhost:1313`

```bash
# lancer un serveur web minimaliste pour votre site hugo, en affichant toutes les pages/posts

hugo server -D
```

## Mise en place d'une CI

**TODO - WORK IN PROGRESS**

L'intérêt, c'est de s'abstraire complètement d'un serveur dédié ou d'un VPS et de toute son adminitration. De plus, grâce à hugo, terminé la gestion des bases de données ou encore des dépendances pour un langage de programmation web (PHP...).

Pour ComputerZ Solutions, le dépôt git est placé sur GitHub et est ensuite généré par un JAMstack sur [CloudFlare Pages](https://pages.cloudflare.com/). L'idée, c'est d'avoir un site hautement disponible, généré à partir des pages/CMS hugo, depuis GitHub et le tout, gratuitement.

### CloudFlare Pages

**TODO - WORK IN PROGRESS**

Dirigez-vous sur la page officielle de [CloudFlare Pages](https://pages.cloudflare.com/). Cliquez sur le bouton "Sign Up" pour y créer un compte. Si vous avez déjà un compte CloudFlare, alors cliquez uniquement sur le bouton "Se connecter", vous serez redirirgez vers votre tableau de bord.

1. 

## Inspirations

De nombreux sites web sous Hugo ont leurs sources sur des dépôts Git sur GitHub. J'ai utilisé des lignes de configuration quant à ces sites web :

- [gohugoio @GitHub.com](https://github.com/gohugoio/hugoBasicExample)
- [letsencrypt @GitHub.com](https://github.com/letsencrypt/website)
- [regisphilibert @GitHub.com](https://github.com/regisphilibert/regisphilibert.com)
