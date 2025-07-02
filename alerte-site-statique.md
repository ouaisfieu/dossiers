---
# 1. Titre et layout
title: "🟥 ALERTE SITE STATIQUE 🟥"
layout: single
classes: wide
permalink: /alerte-site-statique/

# 2. SEO / jekyll-seo-tag
seo_title: "Créer votre site perso statique : Notion Sites, Obsidian Publish & GitHub Pages"
seo_description: >-
  Après une courte alerte sécurité sur les sites statiques, découvrez trois
  manières simples de lancer votre propre site web personnel : Notion Sites,
  Obsidian Publish ou GitHub Pages.
keywords:
  - site statique
  - site personnel
  - Notion Sites
  - Obsidian Publish
  - GitHub Pages
  - Jekyll
  - sécurité web
robots: index, follow

# 3. Extrait, catégories & tags
excerpt: >-
  Visibilité, performance, sécurité : apprenez d’abord pourquoi un site
  statique est sûr, puis comment en créer un en quelques clics avec Notion,
  Obsidian ou GitHub Pages.
categories:
  - Web
  - Tutoriel
  - Outils
tags:
  - site statique
  - site personnel
  - Notion Sites
  - Obsidian Publish
  - GitHub Pages
  - sécurité
  - Jekyll

# 4. Images & crédits
image:
  feature: assets/img/cover.jpg
  thumb: assets/img/clov-logo.png
  credit: "ouaisfi.eu"
  creditlink: "https://ouaisfieu.github.io/dossiers/"
og_image: "assets/img/clov-logo.png"
twitter_image: "assets/img/clov-logo.png"

# 5. Dates & auteur
date: 2025-07-02
last_modified_at: 2025-07-02
author: ouaisfi.eu

# 6. JSON-LD (Web sémantique)
json_ld: |
  {
    "@context": "https://schema.org",
    "@type": "TechArticle",
    "mainEntityOfPage": {
      "@type": "WebPage",
      "@id": "https://votresite.com/alerte-site-statique/"
    },
    "headline": "Créer votre site perso statique : Notion Sites, Obsidian Publish & GitHub Pages",
    "description": "Après une courte alerte sécurité sur les sites statiques, découvrez trois manières simples de lancer votre propre site web personnel : Notion Sites, Obsidian Publish ou GitHub Pages.",
    "image": ["https://ouaisfieu.github.io/dossiers/assets/img/head.jpg"],
    "datePublished": "2025-07-02",
    "dateModified": "2025-07-02",
    "author": {
      "@type": "Person",
      "name": "ouaisfi.eu"
    },
    "publisher": {
      "@type": "Organization",
      "name": "ouaisfi.eu",
      "logo": {
        "@type": "ImageObject",
        "url": "https://ouaisfieu.github.io/dossiers/assets/img/clov-logo.png"
      }
    },
    "about": [
    { "@type": "WebSite", "name": "Notion Sites", "url": "https://www.notion.com/help/public-pages-and-web-publishing" },
    { "@type": "WebSite", "name": "Obsidian Publish", "url": "https://publish.obsidian.md/" },
    { "@type": "WebSite", "name": "GitHub Pages", "url": "https://pages.github.com/" }
    ]
  }

---


# 🟥 ALERTE SITE STATIQUE 🟥

> Est-ce que **je risque quelque chose** si je visite un **site statique** ? **Et pourquoi** j'en créerais **pas un moi aussi** /?\\

``` groovy
Réflexion durant 9 secondes

L'utilisateur semble vouloir savoir si la visite d'un site statique comporte des risques, et pourquoi il ne créerait pas un tel site. Visiter un site statique présente peu de risques, mais il peut toujours y avoir des dangers tels que des attaques par script ou un code malveillant embarqué dans des ressources tierces. Créer un site statique peut être avantageux car c'est un projet à faible coût, idéal pour un portfolio et simple à mettre en place.

Terminé
```

### 1. Un « site statique », qu'est-ce que c'est ?

Un site statique sert uniquement des **fichiers pré-générés** (HTML, CSS, images, parfois JavaScript) que le serveur se contente de copier vers votre navigateur.  
Il ne contient pas de base de données ni de code qui s'exécute côté serveur à chaque requête (PHP, Node, Python, etc.).

------------------------------------------------------------------------

### 2. Quels risques pour le visiteur ?

| Risque | Pourquoi c'est (souvent) moins grave | Comment ça peut quand même tourner mal |
|----|----|----|
| **Exécution de code malveillant** | Il n'y a pas de PHP/SQL à pirater côté serveur. | Le site peut charger un fichier **JavaScript** dangereux ou un script tiers compromis (publicité, CDN). |
| **Collecte de données personnelles** | Un site vraiment statique n'a pas besoin de cookies. | L'auteur peut ajouter Google Analytics, Facebook Pixel, Hotjar... Vous êtes alors tracé comme ailleurs. |
| **Téléchargement forcé** | Aucune fonction « drive-by download » côté serveur. | Un lien ou script peut forcer le navigateur à télécharger un fichier, ou inciter l'utilisateur à l'ouvrir. |
| **Phishing** | Pas de formulaires d'authentification internes. | Rien n'empêche un site statique d'imiter la page de connexion d'une banque (tout est question de design). |
| **Failles du navigateur** | Moins de surface d'attaque qu'une appli web complexe. | Si votre navigateur n'est pas à jour, **n'importe** quelle page web (statique ou non) peut exploiter une faille. |

**En pratique :**

- Visiter un site statique est globalement sûr, *à condition* de garder votre navigateur à jour et de rester vigilant si le site vous propose de télécharger/installer quelque chose ou de saisir des informations sensibles.

- Les extensions de sécurité (uBlock Origin, HTTPS-Only, bloqueur de scripts tiers) abaissent encore le risque.

------------------------------------------------------------------------

### 3. Pourquoi créer votre propre site statique ?

| Avantage | Ce que ça veut dire pour vous |
|----|----|
| **Coût quasi nul** | L'hébergement de fichiers se trouve gratuitement (GitHub Pages, GitLab Pages, Cloudflare Pages, Netlify Free, Vercel Hobby...). |
| **Performance & SEO** | Les pages se chargent en quelques millisecondes, Google aime ça. |
| **Sécurité** | Pas de base de données à patcher, pas de CMS à mettre à jour. |
| **Simplicité de déploiement** | Un simple `git push` publie votre site ; vous n'avez pas besoin de gérer un serveur. |
| **Contrôle des données** | Pas de plugin opaque : vous décidez des scripts, des cookies, des polices externes... |
| **Idéal pour un portfolio** | Montrez vos textes, projets Godot, démos HTML5, sans complexité. |
| **Écosystème libre** | Les générateurs (Hugo, Jekyll, Eleventy, Astro, Zola...) sont open-source, documentés, et fonctionnent hors ligne. |

------------------------------------------------------------------------

### 4. Comment s'y prendre ?

**Spoiler:**
Pour faire **vite et/ou bien**:
**<a href="https://obsidian.md/" class="wikilink">Obsidian</a>: ou Notion Site.**

Sinon: **GitHub Pages** mais ça devient ***ardu* niveau technique et intermédiaire** pour le **grand public**.

### 💡 Pourquoi envisager Obsidian Publish ?

Obsidian Publish est idéal pour partager des notes interconnectées, des idées en cours de développement ou des ressources personnelles. Il offre une interface propre, une navigation fluide et la possibilité de personnaliser l'apparence de votre site. C'est une excellente option pour créer un site personnel, un blog ou un jardin numérique sans avoir besoin de compétences avancées en développement web.

> est ce que notion offre la possibilité de faire un site statique ?

Oui, **Notion propose une fonctionnalité appelée *Notion Sites***, qui permet de transformer n'importe quelle page Notion en un site web accessible au public. Cependant, il est important de noter que ces sites ne sont pas des sites *statiques* au sens traditionnel du terme (comme ceux générés par des outils tels que Hugo ou Jekyll).​[Notion+4Notion+4Medium+4](https://www.notion.com/help/public-pages-and-web-publishing?)

------------------------------------------------------------------------

### 🧩 Qu'est-ce que *Notion Sites* ?

*Notion Sites* vous permet de publier rapidement une page Notion sur le web. Cette fonctionnalité est idéale pour partager des contenus tels que des CV, des portfolios, des blogs ou des pages de présentation.​[Latenode Official Community+1Notion+1](https://community.latenode.com/t/can-notion-api-be-used-to-publish-pages-to-the-web/11364?)

#### ✅ Avantages :

- **Simplicité** : Publication en un clic depuis l'interface Notion.

- **Mise à jour en temps réel** : Les modifications apportées à la page Notion sont immédiatement reflétées sur le site publié.

- **Personnalisation** : Possibilité de personnaliser l'URL (par exemple, `votresite.notion.site`) et, avec un plan payant, d'ajouter un domaine personnalisé.

- **Indexation par les moteurs de recherche** : Option pour rendre le site découvrable via les moteurs de recherche.​

#### ⚠️ Limitations :

- **Contrôle limité sur le design** : Personnalisation restreinte en termes de mise en page et de style.

- **Fonctionnalités avancées absentes** : Pas de prise en charge native pour des éléments tels que les barres de navigation personnalisées, les boutons d'appel à l'action ou les animations.

- **Performances** : Étant donné que le contenu est servi dynamiquement depuis les serveurs de Notion, les performances peuvent être inférieures à celles d'un site statique traditionnel.​

------------------------------------------------------------------------

### 🔧 Alternatives pour créer un site statique avec Notion

Si vous souhaitez bénéficier des avantages d'un site statique tout en utilisant Notion comme système de gestion de contenu (CMS), plusieurs solutions s'offrent à vous :

#### 1. **Super.so**

Super transforme vos pages Notion en sites web rapides et personnalisables. Il offre des fonctionnalités telles que :​[Reddit+10Super+10Medium+10](https://super.so/?)

- **Domaine personnalisé** : Utilisez votre propre nom de domaine.

- **SEO amélioré** : Optimisation pour les moteurs de recherche.

- **Personnalisation du design** : Ajoutez des barres de navigation, modifiez les polices et les couleurs.​

Super est une solution payante, avec des plans à partir de 12 \$ par mois.​[Medium+1Super+1](https://medium.com/notion-spot/your-choice-of-tools-to-turn-a-notion-page-into-a-real-website-d0669b73a846?)

#### 2. **Potion.so**

Potion est une alternative à Super, offrant des fonctionnalités similaires pour transformer vos pages Notion en sites statiques. Il propose également des options de personnalisation et de performance améliorée.​[Medium+1Reddit+1](https://medium.com/notion-spot/your-choice-of-tools-to-turn-a-notion-page-into-a-real-website-d0669b73a846?)

#### 3. **Utiliser Notion avec un générateur de site statique**

Pour les utilisateurs ayant des compétences techniques, il est possible d'utiliser Notion en combinaison avec des générateurs de sites statiques comme Gatsby ou Next.js. Cette approche implique :​[Super+2Reddit+2blog.kowalczyk.info+2](https://www.reddit.com/r/Notion/comments/jrg2gf/how_to_give_my_notion_public_page_a_free_custom/)

- **Extraction du contenu** : Utiliser l'API de Notion pour récupérer le contenu des pages.

- **Génération du site** : Transformer le contenu en pages HTML statiques à l'aide d'un générateur de site.

- **Déploiement** : Héberger le site sur des plateformes comme Netlify ou Vercel.​[Latenode Official Community](https://community.latenode.com/t/can-notion-api-be-used-to-publish-pages-to-the-web/11364?)

Cette méthode offre un contrôle total sur le design et les fonctionnalités, mais nécessite des connaissances en développement web.​

------------------------------------------------------------------------

### 🎯 Conclusion

Bien que Notion permette de publier des pages sur le web via *Notion Sites*, ces sites ne sont pas des sites statiques au sens strict. Si vous recherchez une solution simple et rapide, *Notion Sites* peut suffire. Cependant, pour un contrôle accru sur le design, les performances et les fonctionnalités, envisager des alternatives comme Super, Potion ou l'intégration avec un générateur de site statique peut être plus approprié.​

------------------------------------------------------------------------



Il existe de nombreux sites créés avec **Obsidian Publish**, couvrant des domaines variés tels que les blogs, les portfolios, les journaux de recherche et les jardins numériques. Voici une sélection de sites pour vous inspirer :

------------------------------------------------------------------------

### 🌐 Exemples de sites réalisés avec Obsidian Publish

#### 1. [Fork My Brain](https://nicolevanderhoeven.com/)

Un blog technique sur la performance logicielle et l'ingénierie de fiabilité, avec une structure claire et une utilisation efficace des liens internes.​

#### 2. [Yomaru.dev](https://yomaru.dev)

Un site personnel bien conçu, mettant en avant des notes interconnectées et une navigation fluide.​

#### 3. [Zach Daniel](https://zachdaniel.dev/)

Un portfolio de développeur mettant en valeur des projets et des réflexions personnelles.​

#### 4. [ObsidianTTRPGTutorials](https://obsidianttrpgtutorials.com/)

Un guide détaillé pour les jeux de rôle sur table, illustrant comment Obsidian peut être utilisé pour la documentation et les tutoriels.​

#### 5. [The Integral Guide](https://IntegralGuide.com)

Un jardin numérique axé sur la psychologie, la thérapie et la croissance personnelle, offrant une perspective unique sur l'utilisation d'Obsidian pour le développement personnel.​

#### 6. [Kneecaps.org](https://kneecaps.org/)

Un site mettant en avant des personnalisations CSS pour Obsidian Publish, offrant des idées pour personnaliser l'apparence de votre propre site.​

#### 7. Rosie Campbell

Un mélange de pensées, de recettes et de ressources, illustrant comment Obsidian peut être utilisé pour partager des idées variées.​

#### 8. Anthony Agbay

Un site explorant la chimie, l'ingénierie et la médecine, démontrant l'utilisation d'Obsidian pour des sujets scientifiques.​

#### 9. Brian Jenks

Un exemple de structure Zettelkasten, principalement axé sur les statistiques et la programmation, offrant une organisation claire des notes.​

------------------------------------------------------------------------

### 🔍 Où trouver d'autres exemples ?

- **Obsidian Hub** : Une collection organisée de sites créés avec Obsidian Publish, offrant des exemples et des modèles pour divers cas d'utilisation. ​[Obsidian](https://publish.obsidian.md/hub/03%2B-%2BShowcases%2B%26%2BTemplates/%F0%9F%97%82%EF%B8%8F%2B03%2B-%2BShowcases%2B%26%2BTemplates?)

- **Forum Obsidian** : De nombreux utilisateurs partagent leurs sites et expériences avec Obsidian Publish. ​

- **Reddit r/ObsidianMD** : Des discussions communautaires où les utilisateurs partagent leurs sites et demandent des retours. ​

------------------------------------------------------------------------

### 💡 Pourquoi ne pas déjà envisager Obsidian gratuit sans publication payante pour le moment, organiser les notes et publier provisoirement via Notion puis diffuser les liens via les réseaux sociaux ? Et ensuite voir si ça vaut le coup de mettre... Combien déjà ?

Réflexion durant 38 secondes

Voici la feuille de route la plus rapide et la moins coûteuse : commencez GRATUITEMENT avec Obsidian pour écrire et structurer vos notes ; publiez temporairement les pages que vous voulez montrer via **Notion Sites** (en mode gratuit, donc sous *notion.site*) et propagez simplement les liens sur vos réseaux. Quand votre audience, votre charge de travail ou vos besoins de personnalisation réclameront mieux, vous passerez à **Obsidian Publish** (8 \$ / site / mois en annuel, 10 \$ en mensuel) sans rien perdre : vos notes resteront dans le même dépôt Markdown.

------------------------------------------------------------------------

## Pourquoi ce « sandwich » Obsidian ⇄ Notion ?

### Obsidian côté coulisses

- **Zéro coût** : le logiciel de bureau est gratuit et local ; vous gardez un contrôle complet sur vos fichiers Markdown.

- **Architecture évolutive** : vos liens, tags et graphes restent intacts si vous migrez plus tard vers Publish ou un générateur statique.

- **Workflow hors-ligne** : vous pouvez rédiger même sans connexion et pousser vos changements quand bon vous semble.

### Notion pour la vitrine provisoire

- **Publication en un clic** sur *notion.site* incluse dans le plan gratuit, sans aucune configuration serveur. [Notion](https://www.notion.com/help/notion-sites-availability-and-pricing)

- **Mise à jour instantanée** : toute modification dans Notion se reflète immédiatement en ligne.

- **Partage simplissime** : un lien web ordinaire que Facebook ou X reconnaissent comme *Open Graph* --- pratique pour teaser vos contenus.

------------------------------------------------------------------------

## Combien ça coûte vraiment ?

| Plateforme | Gratuit | Payant (mensuel) | À quoi ça sert ? |
|----|----|----|----|
| **Obsidian (desktop)** | 0 € | -- | Rédaction & organisation locale |
| **Notion Sites** | 0 € (sous *.notion.site*) | Plus : 10 \$/membre + **8--10 \$/domaine** pour retirer le branding et brancher votre URL | Vitrine rapide |
| **Obsidian Publish** | -- | 10 \$ / mois (8 \$ si fact. annuelle) **par site** | Site hyper-liant, graph, thèmes CSS |



> **Verdict financier** : en phase d'exploration, la combinaison « Obsidian local + Notion gratuit » coûte 0 €. Dès que vous voudrez un domaine propre ET une navigation type wiki/graph, **Publish** revient moins cher qu'un duo Notion Plus + add-on domaine (18 \$/mois minimum) et vous évite de dupliquer le contenu.

------------------------------------------------------------------------

## Étapes concrètes pour démarrer aujourd'hui

### 1️⃣ Structurer votre vault Obsidian

1.  **Créez un dossier `/00-Inbox`** pour les jets bruts et un dossier `/10-Articles` pour les notes destinées au public.

2.  **Appliquez un modèle "note atomique"** : titre H1, résumé, tags, liens entrants/sortants. Le Zettelkasten préconise des notes courtes avec un seul concept. [Obsidian Forum](https://forum.obsidian.md/t/how-do-i-structure-notes-effectively-in-obsidian/49734?)[Obsidian Forum](https://forum.obsidian.md/t/organizing-and-integrating-notes/68988?)[Obsidian Forum](https://forum.obsidian.md/t/please-suggest-how-to-organise-notes/3722?)

3.  **Utilisez les tags et les aliases YAML** pour préparer des permaliens stables (utile quand vous migrerez).

### 2️⃣ Exporter/Importer vers Notion

- Dans Obsidian, sélectionnez les fichiers destinés au public, puis **Exporter en Markdown**.

- Dans Notion : *Settings → Import → Text & Markdown* et chargez le zip. [Notion](https://www.notion.com/help/import-data-into-notion?)

- Si vous voulez automatiser plus tard, sachez que l'API Notion ne prend pas le Markdown brut : chaque paragraphe devient un "block" qu'il faut créer un par un. [Make Community](https://community.make.com/t/how-do-i-get-markdown-formatted-text-content-into-notion/27379?)

### 3️⃣ Mettre la page Notion en ligne

1.  Activez **Share → Publish → Public web**.

2.  Copiez l'URL `votre-slug.notion.site`.

3.  Optionnel : dans un plan payant, branchez votre domaine et activez Google Analytics. [Notion](https://www.notion.com/help/notion-sites-availability-and-pricing)

### 4️⃣ Diffuser et mesurer

- Postez le lien sur vos réseaux ; l'aperçu Open Graph est généré automatiquement.

- Suivez l'engagement ; si vous manquez de stats, préfixez l'URL avec des paramètres UTM ou passez sur un plan payant pour l'intégration GA. [Notion](https://www.notion.com/pricing?)

------------------------------------------------------------------------

## Bonnes pratiques pour que la transition soit fluide

- **Gardez le Markdown maître dans Obsidian** ; Notion ne sert qu'à l'affichage public pendant la phase bêta.

- **Uniformisez vos titres de fichiers et vos slugs** dès le départ ; Publish les réutilisera tels quels.

- **Évitez les embeds spécifiques à Notion** (Excalidraw, Figma...) qui n'existent pas côté Publish.

- **Sauvegardez votre vault dans Git** : vous gagnez le versioning et la diffusion gratuite via GitHub + Netlify si un jour vous passez à un site statique pur.

------------------------------------------------------------------------

## Quand (et comment) passer à Obsidian Publish ?

| Indice d'opportunité | Signal à surveiller | Action |
|----|----|----|
| **Audience \> 1 000 visites/mois** | Vous sentez les limites SEO et branding de *notion.site* | Souscrivez Publish annuel (96 \$/an) et branchez votre DNS |
| **Besoins de navigation exploratoire** | Vos lecteurs réclament la *graph view* ou les hover-previews | Activez Publish, importez votre CSS, gardez la même structure de fichiers |
| **Maintenance double devient pénible** | Copier-coller entre Obsidian et Notion vous fait perdre du temps | Supprimez la couche Notion, basculez le CNAME vers Publish |

La migration est 1-pour-1 : copiez simplement le dossier ; aucun export compliqué.

------------------------------------------------------------------------

## Prochain pas (ce soir si vous voulez)

1.  **Installez Obsidian** et ouvrez un nouveau vault.

2.  **Définissez trois modèles** (note atomique, article, page-index).

3.  **Écrivez 3-5 notes** et exportez-les.

4.  **Importez dans Notion et publiez**.

5.  **Partagez le lien** sur LinkedIn/X/Fediverse, et mesurez le retour.

En moins de deux heures, vous aurez un flux complet « rédaction → publication » à coût zéro, que vous pourrez faire monter en gamme (domaine perso, Publish, ou même générateur statique) quand vous le jugerez pertinent.
