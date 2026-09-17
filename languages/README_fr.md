# vkt-note

[English](../README.md) | [中文](README_zh.md) | [Deutsch](README_de.md) | [Español](README_es.md) | [日本語](README_ja.md) | Français

Manuel officiel · Une extension légère de prise de notes en Markdown avec sélection de texte pour navigateurs Chromium.

> Chromium · Manifest V3 · SidePanel · Stockage local

---

## Pourquoi vkt-note ?

La plupart des extensions de prise de notes nécessitent des comptes, une synchronisation cloud ou des abonnements. vkt-note est différent : **tout reste dans votre navigateur, zéro donnée ne quitte votre appareil.**

| Avantage | Détail |
|-----------|--------|
| 📝 **Sélection de texte** | Sélectionnez du texte sur n'importe quelle page web, faites un clic droit pour sauvegarder instantanément en note Markdown |
| 🔒 **100 % local** | Toutes les notes stockées dans `chrome.storage.local` — pas de cloud, pas de comptes, pas de suivi |
| ✏️ **Éditeur Markdown** | Édition en source avec barre d'outils de formatage, sauvegarde automatique et prévisualisation plein écran |
| 🛡 **Sauvetage de brouillon** | Les nouvelles notes bloquées par la limite quotidienne sont conservées comme brouillon local et proposées pour restauration — rien de ce que vous écrivez n'est perdu |
| 📋 **Quota intelligent** | 3 notes/jour gratuites ; supprimez les notes du jour pour récupérer des emplacements — jamais bloqué |

---

## Liste des fonctionnalités

### 🆓 Fonctionnalités gratuites

| Fonctionnalité | Description |
|---------|-------------|
| 📝 **Sauvegarder dans vkt-note** | Clic droit sur n'importe quelle sélection ou image → le menu unifié détecte automatiquement le contenu, convertit le HTML en Markdown et sauvegarde silencieusement |
| 🔍 **Recherche de notes** | Filtrez rapidement la liste des notes par titre et contenu |
| 📋 **Copier en Markdown** | Un clic copie n'importe quelle note en Markdown dans le presse-papiers — une sauvegarde locale gratuite |
| ✏️ **Éditeur Markdown** | Édition en source avec barre d'outils de formatage, sauvegarde automatique et prévisualisation plein écran |
| 🧩 **HTML → Markdown** | Utilise la bibliothèque Turndown (standard de l'industrie) pour convertir le HTML — tableaux, titres, listes, liens, blocs de code, images, etc. |
| ▦ **Sélecteur de tableaux** | Liste chaque tableau de la page courante — choisissez-en un pour l'insérer en tant que tableau Markdown |
| 📎 **Insérer une URL** | Insérez en un clic l'URL de la page courante en tant que lien Markdown |
| 📑 **Insérer un titre** | Insérez en un clic le titre de la page courante dans la note |
| 🛡 **Brouillon de quota** | Si le quota quotidien bloque une nouvelle note, son contenu est conservé comme brouillon local et une restauration est proposée à la prochaine ouverture du panneau |
| 🛠️ **Barre d'outils de formatage** | Gras, Italique, Barré, H1–H3, Lien, Code inline, Bloc de code, Liste à puces/numérotée, Citation, Ligne horizontale |
| 💾 **Sauvegarde automatique** | Les notes se sauvegardent automatiquement 2 secondes après la modification — pas besoin de cliquer sur Sauvegarder manuellement |
| 📋 **Quota quotidien** | 3 nouvelles notes par jour ; la modification de notes existantes ne consomme pas de quota |
| 🔒 **Stockage local** | Toutes les notes stockées localement — aucun envoi de données, pas de synchronisation cloud |
| 🏗️ **Manifest V3** | Construit sur le Manifest V3 avec l'architecture SidePanel |

### ⭐ Fonctionnalités Premium (licence requise)

| Fonctionnalité | Description |
|---------|-------------|
| ♾️ **Notes illimitées** | Pas de quota quotidien — créez autant de notes que vous voulez |
| 📤 **Exporter toutes les notes** | Téléchargez toutes les notes en fichier JSON structuré |
| 💬 **Support prioritaire** | Support e-mail prioritaire pour les utilisateurs Premium |

> Voir les [tarifs VKT](https://www.annmax1983.com/pricing.html) pour les options de licence.

---

## Aperçu

> 📸 Les captures d'écran seront publiées ici avec la présentation de la boutique.

---

## Navigateurs compatibles

| Navigateur | Statut | Version minimum |
|---------|--------|-----------------|
| Google Chrome | ✅ Entièrement pris en charge | Chrome 114+ (API SidePanel) |
| Microsoft Edge | ✅ Entièrement pris en charge | Edge 114+ |
| Autres navigateurs basés sur Chromium | ⚠️ Compatibilité de base | Doit supporter l'API SidePanel |

---

## Installation

Pour votre sécurité, n'installez vkt-note que via les boutiques officielles d'extensions :

1. Ouvrez le **Chrome Web Store** ou **Microsoft Edge Add-ons**
2. Recherchez : `vkt-note`
3. Cliquez sur **« Ajouter à Chrome »** / **« Ajouter à Edge »**
4. Cliquez sur l'icône 📝 vkt-note dans votre barre d'outils pour ouvrir le panneau latéral

> ⚠️ N'installez pas depuis des sites tiers. Les versions non autorisées peuvent compromettre la sécurité de vos données.

---

## Utilisation

### Créer des notes

1. Cliquez sur l'**icône 📝 vkt-note** dans la barre d'outils pour ouvrir le panneau latéral
2. Cliquez sur **➕ Nouvelle note** pour créer une note vierge
3. Ou **sélectionnez du texte** sur n'importe quelle page web → clic droit → **Sauvegarder dans vkt-note**
4. Ou **faites un clic droit sur une image** → **Sauvegarder dans vkt-note**

### Copier du contenu web en Markdown

- **Clic droit sur une sélection** → **Sauvegarder dans vkt-note**. Le HTML de la sélection est converti en Markdown via la bibliothèque Turndown. Quand la sélection se trouve dans une cellule de tableau, elle est étendue à la cellule complète, la ligne ou le tableau (l'unité complète la plus petite).
- **Clic droit sur une image** → **Sauvegarder dans vkt-note**. Le lien de l'image est sauvegardé en tant qu'image Markdown dans une nouvelle note.
- **▦ Sélecteur de tableaux** (barre d'outils). Liste chaque tableau de la page courante ; cliquez-en un pour l'insérer en tant que tableau Markdown dans la note ouverte (ou dans une nouvelle note).

### Barre d'outils de formatage

La barre au-dessus de l'éditeur propose un formatage rapide : **Gras**, *Italique*, ~~Barré~~, H1, H2, H3, Lien, Code inline, Bloc de code, Liste à puces, Liste numérotée, Citation, Ligne horizontale.

### Modifier des notes

- Les notes se **sauvegardent automatiquement 2 secondes** après la fin de la saisie — pas besoin de cliquer sur Sauvegarder manuellement
- Le bouton **Sauvegarder** fonctionne toujours pour une sauvegarde immédiate
- Cliquez sur **👁 Aperçu** pour voir le contenu formaté en **vue plein écran** avec un bouton de retour — aucune interface d'éditeur visible
- Note d'aperçu : les listes profondément imbriquées sont aplaties à un seul niveau dans l'aperçu (le Markdown sauvegardé conserve toujours toute la fidélité)
- **Brouillon de quota** : si une nouvelle note atteint la limite quotidienne, son contenu est conservé localement et il vous est demandé de la restaurer à la prochaine ouverture du panneau
- Les titres sont générés automatiquement sous la forme `Note N` — vous pouvez les modifier librement

### Règles du niveau gratuit

- Version gratuite : maximum **3 nouvelles notes par jour**
- La création d'une **nouvelle** note compte dans la limite quotidienne (sauvegarde manuelle et sauvegarde automatique après 2 secondes incluses)
- La modification de notes existantes ne **consomme pas** de quota
- La suppression d'une note créée **aujourd'hui** restaure un emplacement de quota
- La suppression d'une note d'un jour précédent n'**affecte pas** le quota du jour
- Si une nouvelle note est bloquée par la limite quotidienne, son contenu est enregistré comme brouillon local — rouvrez le panneau dans les 24 heures pour le restaurer
- Les numéros de séquence des titres de notes peuvent présenter des trous après suppression — c'est prévu ainsi

### Export (Premium uniquement)

- Les utilisateurs Premium peuvent cliquer sur **📥 Exporter** pour télécharger toutes les notes en fichier JSON
- Le fichier exporté est destiné à la sauvegarde/consultation uniquement — **l'extension ne supporte pas l'import de notes**

---

## FAQ

1. **Le menu contextuel n'apparaît pas ?**
   Le menu apparaît quand vous sélectionnez du texte ou faites un clic droit sur une image. Il utilise l'option unifiée « Sauvegarder dans vkt-note ».

2. **Les notes disparaissent après réinstallation ?**
   Toutes les notes sont stockées dans `chrome.storage.local`. La désinstallation de l'extension supprime définitivement toutes les données. Exportez vos notes avant la désinstallation (fonctionnalité Premium).

3. **Les images dans les notes s'affichent cassées ?**
   Les images Markdown stockent uniquement les URLs distantes. Si le site source est en panne, bloque le hotlinking ou si l'image est supprimée, elle ne se chargera pas.

4. **Puis-je importer les notes exportées ?**
   Non. L'export JSON est uniquement destiné à la sauvegarde manuelle. L'extension ne supporte pas la réimportation de notes.

5. **Comment obtenir plus de 3 notes par jour ?**
   Supprimez les notes créées aujourd'hui pour libérer des emplacements, ou passez à Premium pour des notes illimitées.

---

## Confidentialité

vkt-note respecte les principes de confidentialité dès la conception :

- ✅ Toutes les notes stockées dans `chrome.storage.local` — **aucune donnée n'est envoyée à un serveur**
- ✅ Pas d'analytics, pas de suivi, pas de cookies
- ✅ Le contenu des pages n'est accédé que lorsque vous déclenchez explicitement une sauvegarde ou une insertion (menu contextuel, boutons d'insertion, sélecteur de tableaux) — jamais en arrière-plan
- ✅ Les fichiers JSON exportés sont créés localement et jamais transmis

### Permissions

| Permission | Raison |
|------------|--------|
| `storage` | Sauvegarder les notes et les paramètres en local |
| `sidePanel` | Afficher l'interface de l'extension dans un panneau latéral |
| `contextMenus` | Menu contextuel pour créer des notes à partir de texte ou d'images sélectionnés |
| `scripting` | Injecter le convertisseur HTML→Markdown uniquement quand vous déclenchez une action de sauvegarde / insertion / tableau |
| Hôte `<all_urls>` | Permet à ces actions explicites de lire la sélection de la page courante, les tableaux, l'URL et le titre — pas d'accès en arrière-plan ni à l'historique de navigation |

- [Politique de confidentialité complète](https://annmax1983.github.io/vkt-note/privacy-policy.html)

---

## Avertissement relatif au droit d'auteur

1. Cette extension permet aux utilisateurs de sauvegarder des sélections de texte et des liens d'images depuis des pages web dans des notes locales. Tous les droits d'auteur des textes, images et contenus de chaque site appartiennent à leurs éditeurs respectifs.
2. La sauvegarde d'extraits en notes ne confère aux utilisateurs aucun droit d'auteur sur le contenu des sites. Il est strictement interdit d'utiliser cette extension pour contourner les paywalls, les restrictions d'adhésion ou les protections anti-copie des sites web.
3. Les utilisateurs doivent se conformer aux lois locales et aux conditions d'utilisation des plateformes lors de l'utilisation de cette extension.

---

## Avis sur le code source

> ⚠️ **Ce dépôt ne publie pas le code source.** Il contient uniquement la documentation d'utilisation, les notes de version et les ressources d'assistance. L'extension est distribuée exclusivement via le Chrome Web Store. Aucun package d'installation hors ligne ni code source destiné aux utilisateurs finaux n'est fourni.

---

## Licence

Copyright © 2026 vkt-note. Tous droits réservés.

Ce logiciel est un logiciel propriétaire fermé. Sans autorisation écrite officielle, les actions suivantes sont strictement interdites :
- Décompiler, cracker ou modifier le code du programme
- Reconditionner, redistribuer, partager ou revendre commercialement
- Intégrer le programme dans d'autres logiciels pour une distribution groupée

---

## ❤️ Soutenir

Si vkt-note vous est utile, offrez un café au développeur !

**[👉 Cliquez ici pour soutenir](https://ko-fi.com/annmax?buyACoffee=true&ref=vkt-note)**
