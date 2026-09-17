# vkt-note

English | [中文](languages/README_zh.md) | [Deutsch](languages/README_de.md) | [Español](languages/README_es.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

Official User Manual · A lightweight Markdown note-taking extension with text selection for Chromium browsers.

> Chromium · Manifest V3 · SidePanel · Local Storage

---

## Why vkt-note?

Most note-taking extensions require accounts, cloud sync, or subscriptions. vkt-note is different: **everything stays in your browser, zero data leaves your device.**

| Advantage | Detail |
|-----------|--------|
| 📝 **Text Selection** | Select text on any webpage, right-click to save as a Markdown note instantly |
| 🔒 **Local Only** | All notes stored in `chrome.storage.local` — no cloud, no accounts, no tracking |
| ✏️ **Markdown Editor** | Source editing with formatting toolbar, auto-save, and full-screen preview |
| 🛡 **Draft Rescue** | New notes blocked by the daily limit are kept as a local draft and offered for restore — nothing you typed is silently lost |
| 📋 **Smart Quota** | Free 3 notes/day; delete today's notes to reclaim slots — never locked out |

---

## Feature List

### 🆓 Free Features

| Feature | Description |
|---------|-------------|
| 📝 **Save to vkt-note** | Right-click any selection or image → unified menu auto-detects content, converts HTML to Markdown, and saves silently |
| 🔍 **Note Search** | Quickly filter the note list by title and content |
| 📋 **Copy as Markdown** | One click copies any note as Markdown to the clipboard — a free local backup |
| ✏️ **Markdown Editor** | Source editing with formatting toolbar, auto-save, and full-screen preview |
| 🧩 **HTML → Markdown** | Uses the Turndown library (industry standard) to convert HTML — tables, headings, lists, links, code blocks, images, and more |
| ▦ **Table Picker** | List every table on the current page — pick one to insert as a Markdown table |
| 📎 **Insert URL** | One-click insert current page URL as Markdown link |
| 📑 **Insert Title** | One-click insert current page title into note |
| 🛡 **Quota Draft** | If the daily quota blocks a new note, its content is kept in a local draft and a restore prompt appears the next time the panel opens |
| 🛠️ **Formatting Toolbar** | Bold, Italic, Strikethrough, H1–H3, Link, Inline Code, Code Block, Bullet/Numbered List, Blockquote, Horizontal Rule |
| 💾 **Auto-Save** | Notes auto-save 2 seconds after editing — no need to manually click Save |
| 📋 **Daily Quota** | 3 new notes per day; editing existing notes does not consume quota |
| 🔒 **Local Storage** | All notes stored locally — no data upload, no cloud sync |
| 🏗️ **Manifest V3** | Built on Manifest V3 with SidePanel architecture |

### ⭐ Premium Features (License Required)

| Feature | Description |
|---------|-------------|
| ♾️ **Unlimited Notes** | No daily quota — create as many notes as you want |
| 📤 **Export All Notes** | Download all notes as a structured JSON backup file |
| 💬 **Priority Support** | Priority email support for Premium users |

> See [VKT Pricing](https://www.annmax1983.com/pricing.html) for license options.

---

## Preview

> 📸 Screenshots will be published here with the store listing.

---

## Supported Browsers

| Browser | Status | Minimum Version |
|---------|--------|-----------------|
| Google Chrome | ✅ Fully supported | Chrome 114+ (SidePanel API) |
| Microsoft Edge | ✅ Fully supported | Edge 114+ |
| Other Chromium-based browsers | ⚠️ Basic compatible | Must support SidePanel API |

---

## Installation

For your safety, only install vkt-note through official browser extension stores:

1. Open **Chrome Web Store** or **Microsoft Edge Add-ons**
2. Search: `vkt-note`
3. Click **"Add to Chrome"** / **"Add to Edge"**
4. Click the 📝 vkt-note icon in your toolbar to open the side panel

> ⚠️ Do not install from third-party websites. Unauthorized versions may compromise your data security.

---

## Usage

### Creating Notes

1. Click the **📝 vkt-note icon** in your browser toolbar to open the side panel
2. Click **➕ New Note** to create a blank note
3. Or **select text** on any webpage → right-click → **Save to vkt-note**
4. Or **right-click an image** → **Save to vkt-note**

### Copying Web Content as Markdown

- **Right-click a selection** → **Save to vkt-note**. The selection's HTML is converted to Markdown using the Turndown library. When the selection is inside a table cell, it is expanded to the complete cell, row, or table (the smallest complete unit).
- **Right-click an image** → **Save to vkt-note**. The image link is saved as a Markdown image in a new note.
- **▦ Table Picker** (toolbar). Lists every table on the current page; click one to insert it as a Markdown table into the open note (or a new note).

### Formatting Toolbar

The toolbar above the editor provides quick formatting: **Bold**, *Italic*, ~~Strikethrough~~, H1, H2, H3, Link, Inline Code, Code Block, Bullet List, Numbered List, Blockquote, Horizontal Rule.

### Editing Notes

- Notes **auto-save 2 seconds** after you stop typing — no need to click Save manually
- The **Save** button still works for immediate save
- Click **👁 Preview** to see formatted content in a **full-screen view** with a back button — no editor chrome visible
- Preview note: deeply nested lists flatten to a single level in preview (the saved Markdown always keeps full fidelity)
- **Quota draft**: if a new note hits the daily limit, its content is kept locally and you're asked whether to restore it the next time the panel opens
- Titles are auto-generated as `Note N` — you can edit them freely

### Free Tier Rules

- Free version: maximum **3 new notes per day**
- Creating a **new** note counts toward the daily limit (both manual save and the 2-second auto-save)
- Editing existing notes does **not** consume quota
- Deleting a note created **today** restores one quota slot
- Deleting a note from a previous day does **not** affect today's quota
- If a new note is blocked by the daily limit, its content is saved as a local draft — reopen the panel within 24 hours to restore it
- Note title sequence numbers may have gaps after deletion — this is by design

### Export (Premium Only)

- Premium users can click **📥 Export** to download all notes as a JSON file
- The exported file is for backup/reference only — **the extension does not support importing notes**

---

## FAQ

1. **Right-click menu doesn't appear?**
   The menu appears when you select text or right-click an image. It uses the unified "Save to vkt-note" option.

2. **Notes disappear after reinstalling?**
   All notes are stored in `chrome.storage.local`. Uninstalling the extension permanently deletes all data. Export your notes before uninstalling (Premium feature).

3. **Images in notes show as broken?**
   Markdown images store remote URLs only. If the source website is down, blocks hotlinking, or the image is removed, the image will not load.

4. **Can I import exported notes?**
   No. The JSON export is for manual backup only. The extension does not support importing notes back.

5. **How do I get more than 3 notes per day?**
   Delete notes created today to free up slots, or upgrade to Premium for unlimited notes.

---

## Privacy

vkt-note follows privacy-by-design principles:

- ✅ All notes stored in `chrome.storage.local` — **no data is uploaded to any server**
- ✅ No analytics, no tracking, no cookies
- ✅ Page content is accessed only when you explicitly trigger save or insert (context menu, insert buttons, table picker) — never in the background
- ✅ Exported JSON files are created locally and never transmitted

### Permissions

| Permission | Reason |
|------------|--------|
| `storage` | Save notes and settings locally |
| `sidePanel` | Display the extension UI in a side panel |
| `contextMenus` | Right-click menu for creating notes from selected text or images |
| `scripting` | Inject the HTML→Markdown converter only when you trigger save / insert / table actions |
| Host `<all_urls>` | Lets those explicit actions read the current page's selection, tables, URL and title — no background or browsing-history access |

- [Full Privacy Policy](https://annmax1983.github.io/vkt-note/privacy-policy.html)

---

## Copyright Disclaimer

1. This extension allows users to save text selections and image links from web pages into local notes. All text, images, and content copyright of each website belong to its respective publisher.
2. Saving excerpts as notes does not grant users any copyright authorization of website content. Users are strictly prohibited from using this extension to bypass website paywalls, membership restrictions, or anti-copy protection mechanisms.
3. Users shall comply with local laws and platform terms of service when using this extension.

---

## Source Code Notice

> ⚠️ **This repository does not publish source code.** It contains only usage documentation, release notes, and support resources. The extension is distributed exclusively through the Chrome Web Store. No offline installation packages or end-user source code are provided.

---

## License

Copyright © 2026 vkt-note. All rights reserved.

This software is closed-source proprietary software. Without official written authorization, the following are strictly prohibited:
- Decompiling, cracking, or modifying the program code
- Repackaging, redistribution, sharing, or commercial resale
- Embedding the program into other software for bundled distribution

---

## ❤️ Support

If you find vkt-note helpful, consider buying the developer a coffee!

**[👉 Click here to support](https://ko-fi.com/annmax?buyACoffee=true&ref=vkt-note)**
