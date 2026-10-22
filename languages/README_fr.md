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
| 🔐 **Chiffrement réel** | Protégez une note ou tout le carnet par mot de passe — texte chiffré au repos en AES-256-GCM, clés jamais stockées |
| ✏️ **Éditeur Markdown** | Édition en source avec barre d'outils de formatage, sauvegarde automatique et aperçu Markdown en direct |
| 🗑 **Corbeille (Premium)** | Les suppressions Premium restent récupérables pendant 30 jours avant leur suppression automatique |

---

## Liste des fonctionnalités

### 🆓 Fonctionnalités gratuites

| Fonctionnalité | Description |
|---------|-------------|
| 📝 **Sauvegarder dans vkt-note** | Clic droit sur n'importe quelle sélection ou image → le menu unifié détecte automatiquement le contenu, convertit le HTML en Markdown et sauvegarde silencieusement — titre repris de la page |
| 🔍 **Recherche de notes** | Filtrez rapidement la liste des notes par titre et contenu |
| 📋 **Copier en Markdown** | Un clic copie n'importe quelle note en Markdown dans le presse-papiers — une sauvegarde locale gratuite |
| ↩️ **Annuler la suppression** | Note supprimée par erreur ? Annulez dans les 7 secondes depuis la liste |
| 📌 **Épingler en haut** | Gardez les notes fréquentes épinglées en tête de liste |
| 💾 **Télécharger en .md** | Enregistrez n'importe quelle note en fichier Markdown — gratuit, sans copier-coller |
| ✏️ **Éditeur Markdown** | Édition en source avec barre d'outils de formatage, sauvegarde automatique et aperçu Markdown en direct |
| ☑️ **Listes de tâches** | Les listes `- [ ]` / `- [x]` s'affichent comme de vraies cases à cocher dans l'aperçu |
| 🧩 **HTML → Markdown** | Utilise la bibliothèque Turndown (standard de l'industrie) pour convertir le HTML — tableaux, titres, listes, liens, blocs de code, images, etc. |
| ▦ **Sélecteur de tableaux** | Liste chaque tableau de la page courante — cochez-en un ou plusieurs et insérez-les dans l'ordre de la page en Markdown ; la page met en surbrillance vos choix |
| 📎 **Insérer une URL** | Insérez en un clic l'URL de la page courante en tant que lien Markdown |
| 📑 **Insérer un titre** | Insérez en un clic le titre de la page courante dans la note |
| 🛠️ **Barre d'outils de formatage** | Gras, Italique, Barré, H1–H3, Lien, Code inline, Bloc de code, Liste à puces/numérotée, Citation, Ligne horizontale |
| 💾 **Sauvegarde automatique** | Les notes se sauvegardent automatiquement 2 secondes après la modification — pas besoin de cliquer sur Sauvegarder manuellement |
| ♾️ **Notes illimitées** | Pas de limite quotidienne — créez autant de notes que nécessaire |
| 🔢 **Compteur de mots** | La barre d'état affiche le nombre total de notes et de mots (caractères CJK et mots latins comptés correctement) |
| 🔐 **Mot de passe par note** | Verrouillez une seule note avec son propre mot de passe ; il prime sur celui du carnet : un seul mot de passe est demandé, jamais les deux |
| 🔒 **Mot de passe du carnet** | Masquez tout le contenu des notes derrière un seul mot de passe tout en gardant les titres dans la liste ; déverrouillez une fois par session du panneau |
| 🔓 **Verrouiller maintenant** | Un clic retire toutes les clés de la mémoire ; fermer le panneau latéral verrouille aussi le carnet |
| 🔒 **Stockage local** | Toutes les notes stockées localement — aucun envoi de notes, pas de synchronisation cloud |
| 🏗️ **Manifest V3** | Construit sur le Manifest V3 avec l'architecture SidePanel |

### ⭐ Fonctionnalités Premium (licence requise)

| Fonctionnalité | Description |
|---------|-------------|
| 📤 **Exporter toutes les notes** | Téléchargez toutes les notes en fichier JSON structuré ; les notes avec mot de passe restent chiffrées |
| 🗑 **Corbeille** | Les suppressions Premium vont dans la Corbeille, peuvent être restaurées pendant 30 jours, puis sont supprimées automatiquement |

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
- Les notes sauvegardées par clic droit reprennent le titre de la page source ; les nouvelles notes vides commencent en `Note N` — les deux sont modifiables librement

### Protection par mot de passe

Le chiffrement est une fonctionnalité gratuite. Les mots de passe ne sont jamais stockés et vos notes sont chiffrées sur cet appareil avec AES-256-GCM avant d'être écrites dans `chrome.storage.local`.

- **Mot de passe du carnet** — ouvrez **Paramètres → Mot de passe du carnet** pour en définir un. La liste des notes (titres, dates et nombre de mots) reste visible ; le contenu, les extraits et les correspondances de recherche sur le contenu restent masqués jusqu'au déverrouillage. Le mot de passe est demandé une fois par session du panneau.
- **Mot de passe par note** — ouvrez une note, cliquez sur le bouton 🔐/🔒 dans l'en-tête de l'éditeur et choisissez **Définir le mot de passe de la note**. Cette note utilise alors son propre mot de passe. Un mot de passe par note **prime** sur le mot de passe du carnet, si bien que les deux ne vous sont jamais demandés.
- **Verrouiller maintenant** — le bouton 🔒 dans l'en-tête du panneau retire de la mémoire la clé du carnet et toutes les clés par note. Fermer le panneau latéral fait de même. Cliquez à nouveau dessus pour déverrouiller.
- **Retirer un mot de passe** — ouvrez la boîte de dialogue de sécurité de la note et choisissez **Retirer le mot de passe de la note**, ou retirez le mot de passe du carnet dans les Paramètres. Retirer le mot de passe du carnet déchiffre les notes protégées par le carnet en clair local ; les mots de passe par note sont conservés.
- **Aucune règle de complexité** — tout mot de passe non vide est accepté.
- **Mot de passe oublié** — il n'existe aucune récupération. Supprimer la note est la seule façon de contourner un mot de passe par note. Si vous avez oublié le mot de passe du carnet, **Réinitialiser le mot de passe du carnet** supprime définitivement chaque note, élément de la Corbeille et brouillon protégés par ce mot de passe, puis désactive le mot de passe du carnet ; les notes dotées de leur propre mot de passe sont conservées.

Les notes chiffrées restent recherchables par titre, mais leur contenu n'est ni indexé ni affiché dans les extraits tant qu'elles sont verrouillées. L'export JSON ne déchiffre jamais : les notes chiffrées sont exportées sous forme de texte chiffré et la boîte de dialogue d'export vous en avertit au préalable. Comme l'extension ne prend pas en charge l'import, un export chiffré ne permet pas de lire ces notes : pour en conserver une copie lisible, déverrouillez la note et utilisez **Copier en Markdown** ou **Télécharger .md**. Un extrait de clic droit en attente est conservé dans `chrome.storage.session` lorsqu'un mot de passe de carnet est activé, afin que son texte en clair ne touche pas le disque.

### Corbeille (Premium)

- Lorsque Premium est actif, la suppression d'une note la déplace vers la **Corbeille** au lieu de la supprimer.
- Les éléments de la Corbeille peuvent être restaurés à tout moment dans un délai de **30 jours** ; passé ce délai, ils sont supprimés automatiquement.
- **Vider la corbeille** et **Supprimer définitivement** retirent les éléments immédiatement et sont irréversibles.
- Les suppressions du niveau gratuit sont définitives : l'annulation de 7 secondes est la seule récupération.
- Si Premium expire, les éléments déjà présents dans la Corbeille restent disponibles pour restauration ou suppression ; seules les nouvelles suppressions suivent la règle du niveau gratuit.

### Notes sur le niveau gratuit

- Pas de limite quotidienne de nouvelles notes : le niveau gratuit est un carnet complet, pas un essai
- La modification de notes existantes est toujours illimitée
- Les numéros de séquence des titres de notes peuvent présenter des trous après suppression — c'est prévu ainsi

### Exporter et télécharger

- **Note individuelle → fichier .md** : cliquez sur l'icône ⬇ de n'importe quelle note pour la télécharger en fichier Markdown (gratuit)
- **Toutes les notes → JSON** (Premium) : cliquez sur **📥 Exporter** pour télécharger toutes les notes dans un fichier JSON structuré ; les notes avec mot de passe restent chiffrées
- Le fichier exporté est destiné à la sauvegarde/consultation uniquement — **l'extension ne supporte pas l'import de notes**, donc les notes chiffrées ne peuvent être ni lues ni restaurées depuis ce fichier

---

## FAQ

1. **Le menu contextuel n'apparaît pas ?**
   Le menu apparaît quand vous sélectionnez du texte ou faites un clic droit sur une image. Il utilise l'option unifiée « Sauvegarder dans vkt-note ».

2. **Les notes disparaissent après réinstallation ?**
   Toutes les notes sont stockées dans `chrome.storage.local`. La désinstallation de l'extension supprime définitivement toutes les données. Exportez vos notes avant la désinstallation (Premium exporte toutes les notes dans un seul fichier JSON, les notes avec mot de passe restant chiffrées ; la version gratuite permet de copier ou télécharger les notes une par une).

3. **Les images dans les notes s'affichent cassées ?**
   Les images Markdown stockent uniquement les URLs distantes. Si le site source est en panne, bloque le hotlinking ou si l'image est supprimée, elle ne se chargera pas.

4. **Puis-je importer les notes exportées ?**
   Non. L'export JSON est uniquement destiné à la sauvegarde manuelle. L'extension ne supporte pas la réimportation de notes.

5. **Y a-t-il une limite de nouvelles notes ?**
   Non. La création est illimitée dans les deux offres ; Premium ajoute l'export JSON complet et une Corbeille de 30 jours.

6. **J'ai oublié mon mot de passe. Peut-il être récupéré ?**
   Non. Le mot de passe n'est jamais stocké, seulement un vérificateur qui ne permet pas d'inverser le chiffrement. Un mot de passe par note ne peut être contourné qu'en supprimant la note. Pour un mot de passe de carnet oublié, la réinitialisation supprime définitivement chaque note, élément de la Corbeille et brouillon protégés par ce mot de passe ; les notes protégées par leur propre mot de passe survivent.

7. **Puis-je voir les titres des notes quand le carnet est verrouillé ?**
   Oui. Les titres, horodatages et nombres de mots restent visibles par conception pour vous permettre de retrouver la note voulue ; le contenu, les extraits et les correspondances de recherche sur le contenu restent masqués jusqu'au déverrouillage. La recherche par titre fonctionne toujours.

8. **À quoi ressemblent les notes chiffrées dans un export ?**
   Elles sont exportées sous forme de texte chiffré, pas en clair. La boîte de dialogue d'export vous avertit lorsque des notes chiffrées sont incluses. Comme l'extension ne prend pas en charge l'import, le fichier JSON ne permet pas de lire ni de réimporter ces notes. Pour en conserver une copie lisible, déverrouillez la note et utilisez **Copier en Markdown** ou **Télécharger .md**.

9. **Où vont les notes supprimées ?**
   Avec Premium, elles vont dans la Corbeille et restent récupérables pendant 30 jours. Avec le niveau gratuit, la suppression est définitive après la fenêtre d'annulation de 7 secondes.

---

## Confidentialité

vkt-note respecte les principes de confidentialité dès la conception :

- ✅ Toutes les notes stockées dans `chrome.storage.local` — **le contenu des notes n'est jamais envoyé à un serveur**
- ✅ Une protection facultative par mot de passe chiffre le contenu des notes au repos avec AES-256-GCM (PBKDF2-HMAC-SHA256, 600 000 itérations) ; les mots de passe et les clés dérivées ne sont jamais stockés ni transmis
- ✅ La seule requête sortante est la vérification facultative de licence Premium (clé de licence, un identifiant d'installation aléatoire, métadonnées de navigateur de base) — aucune note, aucune URL de page
- ✅ Pas d'analytics, pas de suivi, pas de cookies
- ✅ Le contenu des pages n'est accédé que lorsque vous déclenchez explicitement une sauvegarde ou une insertion (menu contextuel, boutons d'insertion, sélecteur de tableaux) — jamais en arrière-plan
- ✅ Les fichiers JSON exportés sont créés localement et jamais transmis ; les notes chiffrées restent chiffrées dans les exports

### Permissions

| Permission | Raison |
|------------|--------|
| `storage` | Sauvegarder les notes et les paramètres en local |
| `unlimitedStorage` | Relève le plafond de stockage local par défaut afin qu'un long historique de notes ne rencontre jamais d'échec d'écriture |
| `sidePanel` | Afficher l'interface de l'extension dans un panneau latéral |
| `contextMenus` | Menu contextuel pour créer des notes à partir de texte ou d'images sélectionnés |
| `scripting` | Injecter le convertisseur HTML→Markdown uniquement quand vous déclenchez une action de sauvegarde / insertion / tableau |
| `alarms` | Exécuter la tâche quotidienne qui supprime les éléments de la Corbeille âgés de plus de 30 jours |
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
