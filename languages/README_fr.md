# vkt-note

[English](../README.md) | [中文](README_zh.md) | [Deutsch](README_de.md) | [Español](README_es.md) | [日本語](README_ja.md) | Français

Outil de notes Markdown avec sélection de texte pour navigateurs Chromium. Créez des notes depuis n'importe quelle page web en un clic droit.

> Chromium · Manifest V3 · SidePanel · Stockage local

---

## Fonctionnalités

| Fonctionnalité | Description |
|----------------|-------------|
| 📝 **Enregistrer dans vkt-note** | Clic droit sur texte ou image → détecte le contenu automatiquement, convertit HTML en Markdown et enregistre |
| ✏️ **Éditeur Markdown** | Édition source avec barre de formatage, sauvegarde automatique, raccourcis clavier et aperçu plein écran |
| 🧩 **HTML → Markdown** | Utilise la bibliothèque Turndown (standard de l'industrie) pour convertir tableaux, titres, listes, liens, blocs de code, images, etc. |
| ▦ **Sélecteur de tableaux** | Liste tous les tableaux de la page actuelle — sélectionnez-en un pour l'insérer en tableau Markdown |
| 📎 **Insérer URL** | Insertion en un clic de l'URL de la page actuelle en lien Markdown |
| 📑 **Insérer titre** | Insertion en un clic du titre de la page actuelle |
| 🔗 **Lien vers la page source** | Lien cliquable affiché dans la barre d'onglets de l'éditeur |
| 🛠️ **Barre de formatage** | Gras, Italique, Barré, H1–H3, Lien, Code en ligne, Bloc de code, Liste à puces, Liste numérotée, Citation, Ligne horizontale |
| 💾 **Sauvegarde automatique** | Les notes sont sauvegardées automatiquement 2 secondes après l'édition |
| 🔒 **Stockage local** | Toutes les notes locales, pas de cloud, pas de compte |
| 📋 **Quota quotidien** | Gratuit 3 notes/jour, supprimer les notes du jour récupère le quota |
| ⭐ **Premium** | Notes illimitées et export JSON |

---

## Gratuit vs Premium

| | Gratuit | Premium |
|---|---|---|
| Notes/jour | 3 | Illimitées |
| Éditeur Markdown | ✅ | ✅ |
| Sélection de texte | ✅ | ✅ |
| Insérer URL/Titre | ✅ | ✅ |
| Export JSON | ❌ | ✅ |

---

## Utilisation

### Créer des notes

1. Cliquez sur l'icône **📝 vkt-note** pour ouvrir le panneau latéral
2. Cliquez sur **➕ Nouvelle note** pour créer une note vide
3. Ou **sélectionnez du texte** → clic droit → **Enregistrer dans vkt-note**. Ou **clic droit sur une image** → **Enregistrer dans vkt-note**

### Copier du contenu web en Markdown

- **Clic droit sur la sélection** → **Enregistrer dans vkt-note**. Le HTML est converti en Markdown via la bibliothèque Turndown.
- **Clic droit sur une image** → **Enregistrer dans vkt-note**. Le lien de l'image est sauvegardé en image Markdown.


### Édition

- Les notes sont **sauvegardées automatiquement 2 secondes** après la saisie
- Le bouton **Enregistrer** reste disponible pour une sauvegarde immédiate
- **👁 Aperçu** affiche le contenu formaté en plein écran avec un bouton retour
- **Lien vers la page source** affiché dans la barre d'onglets de l'éditeur

---

## Confidentialité

- ✅ Toutes les notes dans `chrome.storage.local` — aucune donnée transmise
- ✅ Pas d'analyse, pas de tracking
- ✅ Désinstallation supprime toutes les données

---

## Support

Questions ou retours : **support@annmax1983.com**

---

---

## Avis sur le code source

> ⚠️ **Ce dépôt ne publie pas le code source.** Il contient uniquement la documentation d'utilisation, les notes de mise à jour et les ressources d'assistance. L'extension est distribuée exclusivement via le Chrome Web Store. Aucun package d'installation hors ligne ni code source pour les utilisateurs finaux n'est fourni.


## Licence

Propriétaire. Tous droits réservés.
