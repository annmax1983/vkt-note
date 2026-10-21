# vkt-note

[English](../README.md) | [中文](README_zh.md) | [Deutsch](README_de.md) | [Español](README_es.md) | [日本語](README_ja.md) | Français

Manuel officiel · Une extension légère de prise de notes en Markdown avec sélection de texte pour navigateurs Chromium.

> Chromium · Manifest V3 · SidePanel · Stockage local

---

## Pourquoi vkt-note ?

La plupart des extensions de prise de notes nécessitent des comptes, une synchronisation cloud ou des abonnements. vkt-note est différent : **vos notes restent dans votre navigateur et ne sont jamais envoyées.**

| Avantage | Détail |
|-----------|--------|
| 📝 **Sélection de texte** | Sélectionnez du texte sur n'importe quelle page web, faites un clic droit pour sauvegarder instantanément en note Markdown |
| 🔒 **100 % local** | Toutes les notes stockées dans `chrome.storage.local` — pas de cloud, pas de comptes, pas de suivi |
| ✏️ **Éditeur Markdown** | Édition en source avec barre d'outils de formatage, sauvegarde automatique et aperçu Markdown en direct |
| 🛡 **Sauvetage de brouillon** | Les notes bloquées par la limite quotidienne sont conservées dans un emplacement de brouillon local et proposées pour restauration |
| 📋 **Quota intelligent** | 3 notes/jour gratuites ; supprimez les notes du jour pour récupérer des emplacements — jamais bloqué |

---

## Liste des fonctionnalités

### 🆓 Fonctionnalités gratuites

| Fonctionnalité | Description |
|---------|-------------|
| 📝 **Sauvegarder dans vkt-note** | Clic droit sur n'importe quelle sélection ou image → le menu unifié détecte automatiquement le contenu, convertit le HTML en Markdown et sauvegarde silencieusement — titre repris de la page |
| 🔍 **Recherche de notes** | Filtrez rapidement la liste des notes par titre et contenu |
| 📋 **Copier en Markdown** | Un clic copie n'importe quelle note en Markdown dans le presse-papiers — une sauvegarde locale gratuite |
| ↩️ **Annuler la suppression** | Note supprimée par erreur ? Annulez dans les 7 secondes — le quota aussi |
| 📌 **Épingler en haut** | Gardez les notes fréquentes épinglées en tête de liste |
| 💾 **Télécharger en .md** | Enregistrez n'importe quelle note en fichier Markdown — gratuit, sans copier-coller |
| ✏️ **Éditeur Markdown** | Édition en source avec barre d'outils de formatage, sauvegarde automatique et aperçu Markdown en direct |
| ☑️ **Listes de tâches** | Les listes `- [ ]` / `- [x]` s'affichent comme de vraies cases à cocher dans l'aperçu |
| 🧩 **HTML → Markdown** | Utilise la bibliothèque Turndown (standard de l'industrie) pour convertir le HTML — tableaux, titres, listes, liens, blocs de code, images, etc. |
| ▦ **Sélecteur de tableaux** | Liste chaque tableau de la page courante — cochez-en un ou plusieurs et insérez-les dans l'ordre de la page en Markdown ; la page met en surbrillance vos choix |
| 📎 **Insérer une URL** | Insérez en un clic l'URL de la page courante en tant que lien Markdown |
| 📑 **Insérer un titre** | Insérez en un clic le titre de la page courante dans la note |
| 🛡 **Brouillon de quota** | Si le quota quotidien bloque une nouvelle note, son contenu est conservé comme brouillon local et une restauration est proposée à la prochaine ouverture du panneau |
| 🛠️ **Barre d'outils de formatage** | Gras, Italique, Barré, H1–H3, Lien, Code inline, Bloc de code, Liste à puces/numérotée, Citation, Ligne horizontale |
| 💾 **Sauvegarde automatique** | Les notes se sauvegardent automatiquement 2 secondes après la modification — pas besoin de cliquer sur Sauvegarder manuellement |
| 📋 **Quota quotidien** | 3 nouvelles notes par jour ; la modification de notes existantes ne consomme pas de quota |
| 🔢 **Compteur de mots** | La barre d'état affiche le nombre total de notes et de mots (caractères CJK et mots latins comptés correctement) |
| 🔒 **Stockage local** | Toutes les notes stockées localement — aucun envoi de notes, pas de synchronisation cloud |
| 🏗️ **Manifest V3** | Construit sur le Manifest V3 avec l'architecture SidePanel |

### ⭐ Fonctionnalités Premium (licence requise)

| Fonctionnalité | Description |
|---------|-------------|
| ♾️ **Notes illimitées** | Pas de quota quotidien — créez autant de notes que vous voulez |
| 📤 **Exporter toutes les notes** | Téléchargez toutes les notes en fichier JSON structuré |

> Voir les [tarifs VKT](https://www.annmax1983.com/checkout.html?plugin=vktnote) pour les options de licence.

---

## Aperçu

> 📸 Les visuels de la boutique et les captures d'écran se trouvent dans le répertoire `screenshot/`.

---

## Navigateurs compatibles

| Navigateur | Statut | Version minimum |
|---------|--------|-----------------|
| Google Chrome | ✅ Entièrement pris en charge | Chrome 116+ (sidePanel.open) |
| Microsoft Edge | ✅ Entièrement pris en charge | Edge 116+ |
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
- **▦ Sélecteur de tableaux** (barre d'outils). Liste chaque tableau de la page courante ; cochez-en un ou plusieurs et cliquez sur **Insérer** — ils sont convertis en Markdown et ajoutés dans l'ordre de la page (ou dans une nouvelle note), et la page revient en surlignant les tableaux choisis.

### Barre d'outils de formatage

La barre au-dessus de l'éditeur propose un formatage rapide : **Gras**, *Italique*, ~~Barré~~, H1, H2, H3, Lien, Code inline, Bloc de code, Liste à puces, Liste numérotée, Citation, Ligne horizontale.

### Modifier des notes

- Les notes se **sauvegardent automatiquement 2 secondes** après la fin de la saisie — pas besoin de cliquer sur Sauvegarder manuellement
- Le bouton **Sauvegarder** fonctionne toujours pour une sauvegarde immédiate
- Cliquez sur **👁 Aperçu** pour afficher le Markdown rendu dans l'onglet d'aperçu de l'éditeur
- Note d'aperçu : les listes profondément imbriquées sont aplaties à un seul niveau dans l'aperçu (le Markdown sauvegardé conserve toujours toute la fidélité)
- **Brouillon de quota** : si une nouvelle note atteint la limite quotidienne, son contenu est conservé localement et il vous est demandé de la restaurer à la prochaine ouverture du panneau
- Les notes sauvegardées par clic droit reprennent le titre de la page source ; les nouvelles notes vides commencent en `Note N` — les deux sont modifiables librement

### Règles du niveau gratuit

- Version gratuite : maximum **3 nouvelles notes par jour**
- La création d'une **nouvelle** note compte dans la limite quotidienne (sauvegarde manuelle et sauvegarde automatique après 2 secondes incluses)
- La modification de notes existantes ne **consomme pas** de quota
- La suppression d'une note créée **aujourd'hui** restaure un emplacement de quota
- La suppression d'une note d'un jour précédent n'**affecte pas** le quota du jour
- Si une nouvelle note est bloquée par la limite quotidienne, son contenu est enregistré comme brouillon local — rouvrez le panneau dans les 24 heures pour le restaurer
- Les numéros de séquence des titres de notes peuvent présenter des trous après suppression — c'est prévu ainsi

### Exporter et télécharger

- **Note individuelle → fichier .md** : cliquez sur l'icône ⬇ de n'importe quelle note pour la télécharger en fichier Markdown (gratuit)
- **Toutes les notes → JSON** (Premium) : cliquez sur **📥 Exporter** pour télécharger toutes les notes en sauvegarde JSON structurée
- Le fichier exporté est destiné à la sauvegarde/consultation uniquement — **l'extension ne supporte pas l'import de notes**

---

## FAQ

1. **Le menu contextuel n'apparaît pas ?**
   Le menu apparaît quand vous sélectionnez du texte ou faites un clic droit sur une image. Il utilise l'option unifiée « Sauvegarder dans vkt-note ».

2. **Les notes disparaissent après réinstallation ?**
   Toutes les notes sont stockées dans `chrome.storage.local`. La désinstallation de l'extension supprime définitivement toutes les données. Exportez vos notes avant la désinstallation (Premium exporte toutes les notes dans un seul fichier JSON ; la version gratuite permet de copier ou télécharger les notes une par une).

3. **Les images dans les notes s'affichent cassées ?**
   Les images Markdown stockent uniquement les URLs distantes. Si le site source est en panne, bloque le hotlinking ou si l'image est supprimée, elle ne se chargera pas.

4. **Puis-je importer les notes exportées ?**
   Non. L'export JSON est uniquement destiné à la sauvegarde manuelle. L'extension ne supporte pas la réimportation de notes.

5. **Comment obtenir plus de 3 notes par jour ?**
   Supprimez les notes créées aujourd'hui pour libérer des emplacements, ou passez à Premium pour des notes illimitées.

---

## Confidentialité

vkt-note respecte les principes de confidentialité dès la conception :

- ✅ Toutes les notes stockées dans `chrome.storage.local` — **le contenu des notes n'est jamais envoyé à un serveur**
- ✅ La seule requête sortante est la vérification facultative de licence Premium (clé de licence, un identifiant d'installation aléatoire, métadonnées de navigateur de base) — aucune note, aucune URL de page
- ✅ Pas d'analytics, pas de suivi, pas de cookies
- ✅ Le contenu des pages n'est accédé que lorsque vous déclenchez explicitement une sauvegarde ou une insertion (menu contextuel, boutons d'insertion, sélecteur de tableaux) — jamais en arrière-plan
- ✅ Les fichiers JSON exportés sont créés localement et jamais transmis

### Permissions

| Permission | Raison |
|------------|--------|
| `storage` | Sauvegarder les notes et les paramètres en local |
| `unlimitedStorage` | Relève le plafond de stockage local par défaut afin qu'un long historique de notes ne rencontre jamais d'échec d'écriture |
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

> ⚠️ **Ce dépôt est maintenu pour le développement et le conditionnement des versions.** Le code source est propriétaire et ne peut être ni redistribué ni reconditionné. L'extension est distribuée via les boutiques officielles d'extensions de navigateur (Chrome Web Store et Microsoft Edge Add-ons) ; aucun package d'installation hors ligne n'est fourni.

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
