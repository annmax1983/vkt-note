# vkt-note

[English](../README.md) | [中文](README_zh.md) | Deutsch | [Español](README_es.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Offizielle Anleitung · Eine leichtgewichtige Markdown-Notiz-Erweiterung mit Textauswahl für Chromium-Browser.

> Chromium · Manifest V3 · SidePanel · Lokale Speicherung

---

## Warum vkt-note?

Die meisten Notiz-Erweiterungen brauchen Konten, Cloud-Sync oder Abos. vkt-note ist anders: **Ihre Notizen bleiben in Ihrem Browser und werden niemals hochgeladen.**

| Vorteil | Detail |
|---------|--------|
| 📝 **Textauswahl** | Text auf jeder Webseite auswählen, Rechtsklick → sofort als Markdown-Notiz speichern |
| 🔒 **Nur lokal** | Alle Notizen in `chrome.storage.local` — keine Cloud, kein Konto, kein Tracking |
| ✏️ **Markdown-Editor** | Quellbearbeitung mit Formatierungsleiste, Auto-Speicherung und Live-Markdown-Vorschau |
| 🛡 **Entwurf-Schutz** | Vom Tageslimit blockierte Notizen bleiben in einem lokalen Entwurf-Slot erhalten und werden zur Wiederherstellung angeboten |
| 📋 **Smartes Kontingent** | Kostenlos 3 Notizen/Tag; löschen Sie heutige Notizen, um Slots freizugeben — nie ausgesperrt |

---

## Funktionen

### 🆓 Kostenlose Funktionen

| Funktion | Beschreibung |
|----------|-------------|
| 📝 **In vkt-note speichern** | Rechtsklick auf Text oder Bild → einheitliches Menü erkennt Inhalt automatisch, wandelt HTML in Markdown um und speichert leise — Titel kommt vom Seitentitel |
| 🔍 **Notizen durchsuchen** | Notizliste schnell nach Titel und Inhalt filtern |
| 📋 **Als Markdown kopieren** | Ein Klick kopiert jede Notiz als Markdown in die Zwischenablage — ein lokales Backup |
| ↩️ **Löschen rückgängig** | Versehentlich gelöscht? Innerhalb von 7 Sekunden wiederherstellen — Kontingent inklusive |
| 📌 **Anheften** | Häufig genutzte Notizen oben in der Liste fixieren |
| 💾 **Als .md herunterladen** | Einzelne Notiz als Markdown-Datei speichern — kostenlos, ohne Kopieren und Einfügen |
| ✏️ **Markdown-Editor** | Quellbearbeitung mit Formatierungsleiste, Auto-Speicherung und Live-Markdown-Vorschau |
| ☑️ **Aufgabenlisten** | `- [ ]` / `- [x]` Checklists werden in der Vorschau als echte Checkboxen gerendert |
| 🧩 **HTML → Markdown** | Nutzt die Turndown-Bibliothek (Branchenstandard) — Tabellen, Überschriften, Listen, Links, Codeblöcke, Bilder usw. |
| ▦ **Tabellenauswahl** | Listet alle Tabellen der aktuellen Seite — eine oder mehrere ankreuzen, in Seitenreihenfolge als Markdown einfügen; die Seite hebt die Auswahl hervor |
| 📎 **URL einfügen** | Ein-Klick-Einfügung der aktuellen Seiten-URL als Markdown-Link |
| 📑 **Titel einfügen** | Ein-Klick-Einfügung des aktuellen Seitentitels in die Notiz |
| 🛡 **Kontingent-Entwurf** | Blockiert das Tageskontingent eine neue Notiz, bleibt der Inhalt als lokaler Entwurf erhalten — beim nächsten Öffnen des Panels erscheint eine Wiederherstellungsabfrage |
| 🛠️ **Formatierungsleiste** | Fett, Kursiv, Durchgestrichen, H1–H3, Link, Inline-Code, Codeblock, Aufzählung/Nummerierung, Zitat, Trennlinie |
| 💾 **Auto-Speicherung** | Notizen werden 2 Sekunden nach der Bearbeitung automatisch gespeichert |
| 📋 **Tageskontingent** | Maximal 3 neue Notizen pro Tag; Bearbeitung bestehender Notizen verbraucht kein Kontingent |
| 🔢 **Wortzähler** | Statusleiste zeigt Gesamtzahl der Notizen und Wörter (CJK-Zeichen und lateinische Wörter korrekt gezählt) |
| 🔒 **Lokale Speicherung** | Alle Notizen lokal — keine Notiz-Übertragung, keine Cloud |
| 🏗️ **Manifest V3** | Aufgebaut auf Manifest V3 mit SidePanel-Architektur |

### ⭐ Premium-Funktionen (Lizenz erforderlich)

| Funktion | Beschreibung |
|----------|-------------|
| ♾️ **Unbegrenzte Notizen** | Kein Tageslimit — erstellen Sie so viele Notizen wie Sie möchten |
| 📤 **Alle Notizen exportieren** | Alle Notizen als strukturierte JSON-Backup-Datei herunterladen |

> Siehe [VKT Pricing](https://www.annmax1983.com/checkout.html?plugin=vktnote) für Lizenzoptionen.

---

## Vorschau

> 📸 Store-Grafiken und Screenshots liegen im Verzeichnis `screenshot/`.

---

## Unterstützte Browser

| Browser | Status | Mindestversion |
|---------|--------|----------------|
| Google Chrome | ✅ Vollständig unterstützt | Chrome 116+ (sidePanel.open) |
| Microsoft Edge | ✅ Vollständig unterstützt | Edge 116+ |
| Andere Chromium-Browser | ⚠️ Grundsätzlich kompatibel | Muss SidePanel API unterstützen |

---

## Installation

Zu Ihrer Sicherheit vkt-note nur über offizielle Browser-Erweiterungstores installieren:

1. **Chrome Web Store** oder **Microsoft Edge Add-ons** öffnen
2. Suche: `vkt-note`
3. **„Zu Chrome hinzufügen"** / **„Zu Edge hinzufügen"** klicken
4. Das 📝 vkt-note-Symbol in der Symbolleiste klicken, um die Seitenleiste zu öffnen

> ⚠️ Nicht von Drittanbieter-Webseiten installieren. Nicht autorisierte Versionen können Ihre Datensicherheit gefährden.

---

## Nutzung

### Notizen erstellen

1. **📝 vkt-note-Symbol** in der Symbolleiste klicken, um die Seitenleiste zu öffnen
2. **➕ Neue Notiz** klicken, um eine leere Notiz zu erstellen
3. Oder **Text auswählen** → Rechtsklick → **In vkt-note speichern**
4. Oder **Rechtsklick auf Bild** → **In vkt-note speichern**

### Webinhalte als Markdown kopieren

- **Rechtsklick auf Auswahl** → **In vkt-note speichern**. Das HTML der Auswahl wird mit der Turndown-Bibliothek in Markdown umgewandelt. Wenn die Auswahl in einer Tabellenzelle steht, wird sie auf die vollständige Zelle, Zeile oder Tabelle erweitert (die kleinste vollständige Einheit).
- **Rechtsklick auf Bild** → **In vkt-note speichern**. Der Bildlink wird als Markdown-Bild in einer neuen Notiz gespeichert.
- **▦ Tabellenauswahl** (Toolbar). Listet alle Tabellen der aktuellen Seite; eine oder mehrere ankreuzen und auf **Einfügen** klicken — sie werden in Seitenreihenfolge als Markdown angehängt (oder in eine neue Notiz), und die Seite scrollt zurück und hebt die gewählten Tabellen hervor.

### Formatierungsleiste

Die Leiste über dem Editor bietet schnelle Formatierung: **Fett**, *Kursiv*, ~~Durchgestrichen~~, H1, H2, H3, Link, Inline-Code, Codeblock, Aufzählung, Nummerierung, Zitat, Trennlinie.

### Notizen bearbeiten

- Notizen werden **2 Sekunden** nach der letzten Eingabe automatisch gespeichert — kein manueller Klick auf Speichern nötig
- Der **Speichern**-Button funktioniert weiterhin für sofortiges Speichern
- **👁 Vorschau** zeigt die gerenderten Markdown-Inhalte im Vorschau-Tab des Editors
- **Kontingent-Entwurf**: Blockiert das Tageslimit eine neue Notiz, wird der Inhalt lokal behalten und beim nächsten Öffnen des Panels eine Wiederherstellung angeboten
- Per Rechtsklick gespeicherte Notizen erhalten den Titel der Quellseite; neue leere Notizen starten als `Note N` — beides frei editierbar

### Regeln für die kostenlose Stufe

- Kostenlose Version: maximal **3 neue Notizen pro Tag**
- Eine **neue** Notiz zählt für das Tageslimit (sowohl manuelles Speichern als auch die 2-Sekunden-Auto-Speicherung)
- Bearbeitung bestehender Notizen verbraucht **kein** Kontingent
- Löschen einer **heute** erstellten Notiz gibt einen Slot frei
- Löschen einer Notiz von einem früheren Tag beeinflusst **nicht** das heutige Kontingent
- Blockiert das Tageslimit eine neue Notiz, wird ihr Inhalt als lokaler Entwurf gespeichert — stellen Sie ihn wieder her, indem Sie das Panel innerhalb von 24 Stunden erneut öffnen
- Titel-Sequenznummern können nach dem Löschen Lücken haben — das ist so gewollt

### Export & Download

- **Einzelne Notiz → .md-Datei**: Klick auf das ⬇-Symbol auf einer Notizkarte lädt sie als Markdown-Datei herunter (kostenlos)
- **Alle Notizen → JSON** (Premium): **📥 Export** lädt alle Notizen als strukturiertes JSON-Backup herunter
- Die exportierte Datei dient nur zur Sicherung/Referenz — **die Erweiterung unterstützt keinen Import von Notizen**

---

## FAQ

1. **Rechtsklick-Menü erscheint nicht?**
   Das Menü erscheint bei Textauswahl oder Rechtsklick auf ein Bild. Es verwendet die einheitliche Option „In vkt-note speichern".

2. **Notizen nach Neuinstallation verschwunden?**
   Alle Notizen sind in `chrome.storage.local` gespeichert. Deinstallation der Erweiterung löscht alle Daten dauerhaft. Exportieren Sie Ihre Notizen vor der Deinstallation (Premium exportiert alle Notizen als eine JSON-Datei; in der kostenlosen Version können Sie Notizen einzeln kopieren oder herunterladen).

3. **Bilder in Notizen werden nicht angezeigt?**
   Markdown-Bilder speichern nur Remote-URLs. Wenn die Quellseite nicht erreichbar ist, Hotlinking blockiert oder das Bild entfernt wurde, wird es nicht geladen.

4. **Kann ich exportierte Notizen importieren?**
   Nein. Der JSON-Export dient nur zur manuellen Sicherung. Die Erweiterung unterstützt keinen Import von Notizen.

5. **Wie bekomme ich mehr als 3 Notizen pro Tag?**
   Löschen Sie heute erstellte Notizen, um Slots freizugeben, oder upgraden Sie auf Premium für unbegrenzte Notizen.

---

## Datenschutz

vkt-note folgt den Privacy-by-Design-Prinzipien:

- ✅ Alle Notizen in `chrome.storage.local` gespeichert — **Notizinhalte werden niemals an einen Server übertragen**
- ✅ Die einzige ausgehende Anfrage ist die optionale Premium-Lizenzprüfung (Lizenzschlüssel, eine zufällige Installationskennung, grundlegende Browser-Metadaten) — keine Notizen, keine Seiten-URLs
- ✅ Keine Analyse, kein Tracking, keine Cookies
- ✅ Seiteninhalt wird nur bei explizitem Auslösen von Speichern/Einfügen/Tabellenauswahl gelesen (Kontextmenü, Einfügen-Buttons, Tabellenauswahl) — nie im Hintergrund
- ✅ Exportierte JSON-Dateien werden lokal erstellt und niemals übertragen

### Berechtigungen

| Berechtigung | Grund |
|--------------|-------|
| `storage` | Notizen und Einstellungen lokal speichern |
| `unlimitedStorage` | Hebt die standardmäßige lokale Speichergrenze an, damit eine lange Notizhistorie nie an ein Schreiblimit stößt |
| `sidePanel` | Erweiterungs-UI in einer Seitenleiste anzeigen |
| `contextMenus` | Rechtsklick-Menü zum Erstellen von Notizen aus Textauswahl oder Bildern |
| `scripting` | HTML→Markdown-Konverter nur bei Speichern/Einfügen/Tabellen-Aktionen injizieren |
| Host `<all_urls>` | Ermöglicht diesen Aktionen, die aktuelle Seitenauswahl, Tabellen, URL und Titel zu lesen — kein Hintergrund- oder Verlaufszugriff |

- [Vollständige Datenschutzerklärung](https://annmax1983.github.io/vkt-note/privacy-policy.html)

---

## Haftungsausschluss

1. Diese Erweiterung ermöglicht es Nutzern, Textauswahlen und Bildlinks von Webseiten in lokale Notizen zu speichern. Alle Texte, Bilder und Inhalte der jeweiligen Websites unterliegen dem Urhehrrecht des jeweiligen Herausgebers.
2. Das Speichern von Auszügen als Notizen erteilt den Nutzern keine Urheberrechtsbefugnis an den Website-Inhalten. Es ist strengstens untersagt, diese Erweiterung zu verwenden, um Bezahlschranken, Mitgliedschaftseinschränkungen oder Anti-Kopier-Schutzmechanismen zu umgehen.
3. Nutzer haben die örtlichen Gesetze und die Nutzungsbedingungen der Plattformen bei der Verwendung dieser Erweiterung einzuhalten.

---

## Hinweis zum Quellcode

> ⚠️ **Dieses Repository wird für die Entwicklung und das Verpacken von Releases gepflegt.** Der Quellcode ist proprietär und darf nicht weiterverbreitet oder neu verpackt werden. Die Erweiterung wird über offizielle Browser-Erweiterungstores (Chrome Web Store und Microsoft Edge Add-ons) vertrieben; es werden keine Offline-Installationspakete bereitgestellt.

---

## Lizenz

Copyright © 2026 vkt-note. Alle Rechte vorbehalten.

Diese Software ist Closed-Source-Proprietärsoftware. Ohne offizielle schriftliche Genehmigung ist Folgendes strengstens untersagt:
- Dekompilieren, Knacken oder Modifizieren des Programmcodes
- Umverpackung, Weiterverbreitung, Weitergabe oder kommerzieller Wiederverkauf
- Einbetten der Software in andere Software zur gebündelten Verteilung

---

## ❤️ Unterstützung

Wenn Ihnen vkt-note gefällt, kaufen Sie dem Entwickler doch einen Kaffee!

**[👉 Hier unterstützen](https://ko-fi.com/annmax?buyACoffee=true&ref=vkt-note)**
