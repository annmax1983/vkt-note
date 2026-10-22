# vkt-note

English | [中文](languages/README_zh.md) | [Deutsch](languages/README_de.md) | [Español](languages/README_es.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

Official User Manual · A lightweight Markdown note-taking extension with text selection for Chromium browsers.

> Chromium · Manifest V3 · SidePanel · Local Storage

---

## Why vkt-note?

Most note-taking extensions require accounts, cloud sync, or subscriptions. vkt-note is different: **your notes stay in your browser and are never uploaded.**

| Advantage | Detail |
|-----------|--------|
| 📝 **Text Selection** | Select text on any webpage, right-click to save as a Markdown note instantly |
| 🔒 **Local Only** | All notes stored in `chrome.storage.local` — no cloud, no accounts, no tracking |
| 🔐 **Real Encryption** | Protect one note or the whole notebook with a password — AES-256-GCM ciphertext at rest, keys never stored |
| ✏️ **Markdown Editor** | Source editing with formatting toolbar, auto-save, and live Markdown preview |
| 🗑 **Trash (Premium)** | Premium deletions stay recoverable for 30 days before automatic removal |

---

## Feature List

### 🆓 Free Features

| Feature | Description |
|---------|-------------|
| 📝 **Save to vkt-note** | Right-click any selection or image → unified menu auto-detects content, converts HTML to Markdown, and saves silently — titled after the page |
| 🔍 **Note Search** | Quickly filter the note list by title and content |
| 📋 **Copy as Markdown** | One click copies any note as Markdown to the clipboard — a free local backup |
| ↩️ **Undo Delete** | Deleted a note by mistake? Undo within 7 seconds from the note list |
| 📌 **Pin to Top** | Keep frequently used notes pinned above the list |
| 💾 **Download as .md** | Save any single note as a Markdown file — free, no copy-paste needed |
| ✏️ **Markdown Editor** | Source editing with formatting toolbar, auto-save, and live Markdown preview |
| ☑️ **Task Lists** | `- [ ]` / `- [x]` checklists render as real checkboxes in preview |
| 🧩 **HTML → Markdown** | Uses the Turndown library (industry standard) to convert HTML — tables, headings, lists, links, code blocks, images, and more |
| ▦ **Table Picker** | List every table on the current page — tick one or several, insert them in page order as Markdown, and the page highlights your picks |
| 📎 **Insert URL** | One-click insert current page URL as Markdown link |
| 📑 **Insert Title** | One-click insert current page title into note |
| 🛠️ **Formatting Toolbar** | Bold, Italic, Strikethrough, H1–H3, Link, Inline Code, Code Block, Bullet/Numbered List, Blockquote, Horizontal Rule |
| 💾 **Auto-Save** | Notes auto-save 2 seconds after editing — no need to manually click Save |
| ♾️ **Unlimited Notes** | No daily cap — create as many notes as you need |
| 🔢 **Word Count** | Status bar shows total note count and word count (CJK characters and Latin words counted properly) |
| 🔐 **Per-Note Password** | Lock a single note with its own password; it outranks the notebook password, so only one password is ever asked |
| 🔒 **Notebook Password** | Hide all note content behind one password while keeping titles in the list; unlock once per panel session |
| 🔓 **Lock Now** | One click drops every key from memory; closing the side panel locks the notebook too |
| 🔒 **Local Storage** | All notes stored locally — no note upload, no cloud sync |
| 🏗️ **Manifest V3** | Built on Manifest V3 with SidePanel architecture |

### ⭐ Premium Features (License Required)

| Feature | Description |
|---------|-------------|
| 📤 **Export All Notes** | Download all notes as a structured JSON file; notes with passwords stay ciphertext |
| 🗑 **Trash** | Premium deletions go to Trash, can be restored for 30 days, then are removed automatically |

> See [VKT Pricing](https://www.annmax1983.com/checkout.html?plugin=vktnote) for license options.

---

## Preview

> 📸 Store artwork and screenshots are kept in [`screenshot/`](screenshot/).

---

## Supported Browsers

| Browser | Status | Minimum Version |
|---------|--------|-----------------|
| Google Chrome | ✅ Fully supported | Chrome 116+ (sidePanel.open) |
| Microsoft Edge | ✅ Fully supported | Edge 116+ |
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
- **▦ Table Picker** (toolbar). Lists every table on the current page; tick one or several and click **Insert** — they are converted to Markdown and appended in page order (or a new note), and the page scrolls back to highlight the tables you picked.

### Formatting Toolbar

The toolbar above the editor provides quick formatting: **Bold**, *Italic*, ~~Strikethrough~~, H1, H2, H3, Link, Inline Code, Code Block, Bullet List, Numbered List, Blockquote, Horizontal Rule.

### Editing Notes

- Notes **auto-save 2 seconds** after you stop typing — no need to click Save manually
- The **Save** button still works for immediate save
- Click **👁 Preview** to render the note as Markdown in the preview tab
- Preview note: deeply nested lists flatten to a single level in preview (the saved Markdown always keeps full fidelity)
- Notes saved via right-click are titled after the source page; new blank notes start as `Note N` — both are freely editable

### Password Protection

Encryption is a free feature. Passwords are never stored, and your notes are encrypted on this device with AES-256-GCM before they are written to `chrome.storage.local`.

- **Notebook password** — open **Settings → Notebook password** to set one. The note list (titles, dates and word counts) stays visible; content, snippets and content-based search matches stay hidden until you unlock. The password is asked once per panel session.
- **Per-note password** — open a note, click the 🔐/🔒 button in the editor header and choose **Set note password**. That note then uses its own password. A per-note password **takes precedence** over the notebook password, so you are never asked for both.
- **Lock now** — the 🔒 button in the panel header drops the notebook key and every per-note key from memory. Closing the side panel does the same. You can also click it again to unlock.
- **Remove a password** — open the note security dialog and choose **Remove note password**, or remove the notebook password in Settings. Removing the notebook password decrypts vault-protected notes back to local plaintext; per-note passwords are kept.
- **No complexity rules** — any non-empty password is accepted.
- **Forgot a password** — there is no recovery. Deleting the note is the only way past a per-note password. If you forgot the notebook password, **Reset notebook password** permanently deletes every note, Trash item and draft protected by that password, then turns the notebook password off; notes with their own passwords remain.

Encrypted notes are still searchable by title, but their content is not indexed or shown in snippets while locked. JSON export never decrypts: encrypted notes are exported as ciphertext, and the export dialog warns you first. Because the extension does not import notes, a ciphertext export cannot be used to read those notes — to keep a readable copy, unlock the note and use **Copy as Markdown** or **Download .md** before exporting. A pending right-click clip is held in `chrome.storage.session` while a notebook password is enabled, so its plaintext does not touch disk.

### Trash (Premium)

- When Premium is active, deleting a note moves it to **Trash** instead of removing it.
- Trash items can be restored at any time within **30 days**; after that they are deleted automatically.
- **Empty Trash** and **Delete forever** remove items immediately and cannot be undone.
- Free-plan deletions are permanent: the 7-second undo is the only recovery.
- If Premium expires, existing Trash items remain available to restore or delete; only new deletions follow the Free-plan rule.

### Free Tier Notes

- No daily cap on new notes — the free plan is a complete notebook, not a trial
- Editing existing notes is always unlimited
- Note title sequence numbers may have gaps after deletion — this is by design

### Export & Download

- **Single note → .md file**: click the ⬇ icon on any note card to download it as a Markdown file (free)
- **All notes → JSON** (Premium): click **📥 Export** to download a structured JSON file; notes with passwords stay encrypted ciphertext
- Exported files are for backup/reference only — **the extension does not support importing notes**, so encrypted notes in the export cannot be read or restored from the file

---

## FAQ

1. **Right-click menu doesn't appear?**
   The menu appears when you select text or right-click an image. It uses the unified "Save to vkt-note" option.

2. **Notes disappear after reinstalling?**
   All notes are stored in `chrome.storage.local`. Uninstalling the extension permanently deletes all data. Export your notes before uninstalling (Premium exports every note as one JSON file, with password-protected notes kept as ciphertext; the free plan can copy or download notes individually).

3. **Images in notes show as broken?**
   Markdown images store remote URLs only. If the source website is down, blocks hotlinking, or the image is removed, the image will not load.

4. **Can I import exported notes?**
   No. The JSON export is for manual backup only. The extension does not support importing notes back.

5. **Is there a limit on how many notes I can create?**
   No daily limit — create as many notes as you need. Premium adds bulk JSON export and a 30-day Trash.

6. **I forgot my password. Can it be recovered?**
   No. The password is never stored, only a verifier that cannot reverse the encryption. A per-note password can only be bypassed by deleting that note. For a forgotten notebook password, the reset flow permanently deletes every note, Trash item and draft protected by it; per-note protected notes survive.

7. **Can I see note titles when the notebook is locked?**
   Yes. Titles, timestamps and word counts remain visible by design so you can find the note you want; content, snippets and content-based search matches stay hidden until it is unlocked. Title search still works.

8. **What do encrypted notes look like in an export?**
   They are exported as ciphertext, not plaintext. The export dialog warns you when encrypted notes are included. Since the extension has no import feature, the JSON file cannot be used to read or re-import those notes. To keep a readable copy, unlock the note and use **Copy as Markdown** or **Download .md**.

9. **Where do deleted notes go?**
   On Premium, they go to Trash and stay recoverable for 30 days. On the Free plan, deletion is permanent after the 7-second undo window.

---

## Privacy

vkt-note follows privacy-by-design principles:

- ✅ All notes stored in `chrome.storage.local` — **note content is never uploaded to any server**
- ✅ Optional password protection encrypts note content at rest with AES-256-GCM (PBKDF2-HMAC-SHA256, 600,000 iterations); passwords and derived keys are never stored or transmitted
- ✅ The only outbound request is the optional Premium license check (license key, random install identifier, basic browser metadata) — no notes, no page URLs
- ✅ No analytics, no tracking, no cookies
- ✅ Page content is accessed only when you explicitly trigger save or insert (context menu, insert buttons, table picker) — never in the background
- ✅ Exported JSON files are created locally and never transmitted; encrypted notes remain ciphertext in exports

### Permissions

| Permission | Reason |
|------------|--------|
| `storage` | Save notes and settings locally |
| `unlimitedStorage` | Lift the default local storage ceiling so a long note history never hits a write failure |
| `sidePanel` | Display the extension UI in a side panel |
| `contextMenus` | Right-click menu for creating notes from selected text or images |
| `scripting` | Inject the HTML→Markdown converter only when you trigger save / insert / table actions |
| `alarms` | Run the daily job that removes Trash items older than 30 days |
| Host `<all_urls>` | Lets those explicit actions read the current page's selection, tables, URL and title — no background or browsing-history access |

- [Full Privacy Policy](https://annmax1983.github.io/vkt-note/privacy-policy.html)

---

## Copyright Disclaimer

1. This extension allows users to save text selections and image links from web pages into local notes. All text, images, and content copyright of each website belong to its respective publisher.
2. Saving excerpts as notes does not grant users any copyright authorization of website content. Users are strictly prohibited from using this extension to bypass website paywalls, membership restrictions, or anti-copy protection mechanisms.
3. Users shall comply with local laws and platform terms of service when using this extension.

---

## Source Code Notice

> ⚠️ **This repository is maintained for development and release packaging.** The source code is proprietary and may not be redistributed or repackaged. The extension is distributed through official browser extension stores (Chrome Web Store and Microsoft Edge Add-ons); no offline installation packages are distributed to end users.

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
