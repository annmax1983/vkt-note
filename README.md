# vkt-note

English | [中文](languages/README_zh.md) | [Deutsch](languages/README_de.md) | [Español](languages/README_es.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

Official User Manual · A lightweight Markdown note-taking extension with text selection for Chromium browsers.

> Chromium · Manifest V3 · SidePanel · Local Storage · 6 Languages

---

## Why vkt-note?

Most note-taking extensions require accounts, cloud sync, or subscriptions. vkt-note is different: **everything stays in your browser, zero data leaves your device.**

| Advantage | Detail |
|-----------|--------|
| 📝 **Text Selection** | Select text on any webpage, right-click to create a Markdown note instantly |
| 🔒 **Local Only** | All notes stored in `chrome.storage.local` — no cloud, no accounts, no tracking |
| ✏️ **Markdown Editor** | Source editing + live preview with tables, images, code blocks, links, and more |
| 📎 **Source Tracking** | One-click insert current page URL and title — always know where your notes came from |
| 📋 **Smart Quota** | Free 3 notes/day; delete today's notes to reclaim slots — never locked out |
| 🌍 **6 Languages** | English, 中文, 日本語, Deutsch, Español, Français |

---

## Feature List

### 🆓 Free Features

| Feature | Description |
|---------|-------------|
| 📝 **Text Selection Notes** | Select text on any webpage → right-click → create Markdown note |
| ✏️ **Markdown Editor** | Source editing + live preview with full Markdown syntax support |
| 📎 **Insert URL** | One-click insert current page URL as Markdown link |
| 📑 **Insert Title** | One-click insert current page title into note |
| 📋 **Daily Quota** | 3 new notes per day; editing existing notes does not consume quota |
| 🔒 **Local Storage** | All notes stored locally — no data upload, no cloud sync |
| 🌍 **Multi-Language** | 6 languages, auto-detected from browser settings |
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

<p align="center">
  <img src="screenshot/preview.png" alt="vkt-note Preview" width="640">
</p>

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
3. Or **select text** on any webpage → right-click → **Create Markdown note from selection**
4. Or **right-click an image** → **Add image link to new note**

### Editing Notes

- Switch between **Edit** (source code) and **Preview** (rendered) modes using the tabs
- Use the **📎 Insert URL** button to insert a Markdown link to the current page
- Use the **📑 Insert Title** button to insert the current page title
- Titles are auto-generated as `笔记YYYYMMDD_N` — you can edit them freely

### Free Tier Rules

- Free version: maximum **3 new notes per day**
- Only clicking **Save** on a **new** note counts toward the daily limit
- Editing existing notes does **not** consume quota
- Deleting a note created **today** restores one quota slot
- Deleting a note from a previous day does **not** affect today's quota
- Note title sequence numbers may have gaps after deletion — this is by design

### Export (Premium Only)

- Premium users can click **📥 Export** to download all notes as a JSON file
- The exported file is for backup/reference only — **the extension does not support importing notes**

---

## FAQ

1. **Right-click menu doesn't appear?**
   Make sure you've selected text first. The menu only appears when text is selected or when right-clicking an image.

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
- ✅ No `<all_urls>` permission — only accesses page content when you explicitly trigger insert or context menu
- ✅ Exported JSON files are created locally and never transmitted

### Permissions

| Permission | Reason |
|------------|--------|
| `storage` | Save notes, draft, and settings locally |
| `activeTab` | Get current page URL/title when you click insert buttons |
| `sidePanel` | Display the extension UI in a side panel |
| `contextMenus` | Right-click menu for creating notes from selected text or images |
| `scripting` | Required for context menu interaction with page content |

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
