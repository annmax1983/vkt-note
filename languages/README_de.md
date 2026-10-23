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
| 🔐 **Echte Verschlüsselung** | Eine Notiz oder das ganze Notizbuch mit einem Passwort schützen — AES-256-GCM-Chiffrat im Ruhezustand, Schlüssel werden nie gespeichert |
| ✏️ **Markdown-Editor** | Quellbearbeitung mit Formatierungsleiste, Auto-Speicherung und Live-Markdown-Vorschau |
| 🗑 **Papierkorb (Premium)** | Premium-Löschungen bleiben 30 Tage lang wiederherstellbar, bevor sie automatisch entfernt werden |

---

## Funktionen

### 🆓 Kostenlose Funktionen

| Funktion | Beschreibung |
|----------|-------------|
| 📝 **In vkt-note speichern** | Rechtsklick auf Text oder Bild → einheitliches Menü erkennt Inhalt automatisch, wandelt HTML in Markdown um und speichert leise — Titel kommt vom Seitentitel |
| 🔍 **Notizen durchsuchen** | Notizliste schnell nach Titel und Inhalt filtern |
| 📋 **Als Markdown kopieren** | Ein Klick kopiert jede Notiz als Markdown in die Zwischenablage — ein lokales Backup |
| ↩️ **Löschen rückgängig** | Versehentlich gelöscht? Innerhalb von 7 Sekunden aus der Notizliste wiederherstellen |
| 📌 **Anheften** | Häufig genutzte Notizen oben in der Liste fixieren |
| 💾 **Als .md herunterladen** | Einzelne Notiz als Markdown-Datei speichern — kostenlos, ohne Kopieren und Einfügen |
| ✏️ **Markdown-Editor** | Quellbearbeitung mit Formatierungsleiste, Auto-Speicherung und Live-Markdown-Vorschau |
| ☑️ **Aufgabenlisten** | `- [ ]` / `- [x]` Checklists werden in der Vorschau als echte Checkboxen gerendert |
| 🧩 **HTML → Markdown** | Nutzt die Turndown-Bibliothek (Branchenstandard) — Tabellen, Überschriften, Listen, Links, Codeblöcke, Bilder usw. |
| ▦ **Tabellenauswahl** | Listet alle Tabellen der aktuellen Seite — eine oder mehrere ankreuzen, in Seitenreihenfolge als Markdown einfügen; die Seite hebt die Auswahl hervor |
| 📎 **URL einfügen** | Ein-Klick-Einfügung der aktuellen Seiten-URL als Markdown-Link |
| 📑 **Titel einfügen** | Ein-Klick-Einfügung des aktuellen Seitentitels in die Notiz |
| 🛠️ **Formatierungsleiste** | Fett, Kursiv, Durchgestrichen, H1–H3, Link, Inline-Code, Codeblock, Aufzählung/Nummerierung, Zitat, Trennlinie |
| 💾 **Auto-Speicherung** | Notizen werden 2 Sekunden nach der Bearbeitung automatisch gespeichert |
| ♾️ **Unbegrenzte Notizen** | Kein Tageslimit — erstellen Sie so viele Notizen wie nötig |
| 🔢 **Wortzähler** | Statusleiste zeigt Gesamtzahl der Notizen und Wörter (CJK-Zeichen und lateinische Wörter korrekt gezählt) |
| 🔐 **Passwort pro Notiz** | Eine einzelne Notiz mit eigenem Passwort sperren; es hat Vorrang vor dem Notebook-Passwort, sodass immer nur ein Passwort abgefragt wird |
| 🔒 **Notebook-Passwort** | Gesamten Notizinhalt hinter einem Passwort verbergen, während die Titel in der Liste sichtbar bleiben; einmal pro Panel-Sitzung entsperren |
| 🔓 **Jetzt sperren** | Ein Klick entfernt alle Schlüssel aus dem Speicher; das Schließen der Seitenleiste sperrt das Notizbuch ebenfalls |
| 🔒 **Lokale Speicherung** | Alle Notizen lokal — keine Notiz-Übertragung, keine Cloud |
| 🏗️ **Manifest V3** | Aufgebaut auf Manifest V3 mit SidePanel-Architektur |

### ⭐ Premium-Funktionen (Lizenz erforderlich)

| Funktion | Beschreibung |
|----------|-------------|
| 📤 **Alle Notizen exportieren** | Alle Notizen als strukturierte JSON-Datei herunterladen; Notizen mit Passwort bleiben Chiffrat |
| 🗑 **Papierkorb** | Premium-Löschungen landen im Papierkorb, lassen sich 30 Tage lang wiederherstellen und werden danach automatisch entfernt |

> Siehe [VKT Pricing](https://www.annmax1983.com/checkout.html?plugin=vktnote) für Lizenzoptionen.

---

## Vorschau

> 📸 Store-Grafiken und Screenshots liegen im Verzeichnis `screenshots/`.

---

## Unterstützte Browser

| Browser | Status | Mindestversion |
|---------|--------|----------------|
| Google Chrome | ✅ Vollständig unterstützt | Chrome 116+ (sidePanel.open) |
| Microsoft Edge | ✅ Vollständig unterstützt | Edge 116+ |
| Andere Chromium-Browser | ⚠️ Grundsätzlich kompatibel | Muss SidePanel API unterstützen |

---

## Installation

| Store | Link |
|---|---|
| Chrome Web Store | Demnächst verfügbar 🚧 |
| Microsoft Edge Add-ons | [In Edge installieren](https://microsoftedge.microsoft.com/addons/detail/imdfdonlhgecdhcfaapfohphcfnjgcef) |

> Installieren Sie nur über die offiziellen Stores oben – meiden Sie Download-Seiten Dritter.

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
- Per Rechtsklick gespeicherte Notizen erhalten den Titel der Quellseite; neue leere Notizen starten als `Note N` — beides frei editierbar

### Passwortschutz

Verschlüsselung ist eine kostenlose Funktion. Passwörter werden niemals gespeichert, und Ihre Notizen werden auf diesem Gerät mit AES-256-GCM verschlüsselt, bevor sie in `chrome.storage.local` geschrieben werden.

- **Notebook-Passwort** — Öffnen Sie **Einstellungen → Notebook-Passwort**, um eines festzulegen. Die Notizliste (Titel, Datum und Wortzahl) bleibt sichtbar; Inhalt, Textauszüge und inhaltliche Suchtreffer bleiben verborgen, bis Sie entsperren. Das Passwort wird einmal pro Panel-Sitzung abgefragt.
- **Passwort pro Notiz** — Öffnen Sie eine Notiz, klicken Sie auf die 🔐/🔒-Schaltfläche in der Editor-Kopfzeile und wählen Sie **Notizpasswort festlegen**. Diese Notiz verwendet dann ihr eigenes Passwort. Ein Passwort pro Notiz hat **Vorrang** vor dem Notebook-Passwort, sodass Sie nie nach beiden gefragt werden.
- **Jetzt sperren** — Die 🔒-Schaltfläche in der Kopfzeile des Panels entfernt den Notebook-Schlüssel und alle Schlüssel einzelner Notizen aus dem Speicher. Das Schließen der Seitenleiste bewirkt dasselbe. Ein erneuter Klick entsperrt wieder.
- **Passwort entfernen** — Öffnen Sie den Sicherheitsdialog der Notiz und wählen Sie **Notizpasswort entfernen**, oder entfernen Sie das Notebook-Passwort in den Einstellungen. Das Entfernen des Notebook-Passworts entschlüsselt die dadurch geschützten Notizen wieder in lokalen Klartext; Passwörter einzelner Notizen bleiben erhalten.
- **Keine Komplexitätsregeln** — Jedes nicht leere Passwort wird akzeptiert.
- **Passwort vergessen** — Es gibt keine Wiederherstellung. Bei einem Notizpasswort ist das Löschen der Notiz der einzige Ausweg. Wenn Sie das Notebook-Passwort vergessen haben, löscht **Notebook-Passwort zurücksetzen** alle durch dieses Passwort geschützten Notizen, Papierkorb-Einträge und Entwürfe dauerhaft und schaltet das Notebook-Passwort danach aus; Notizen mit eigenem Passwort bleiben erhalten.

Verschlüsselte Notizen sind weiterhin nach Titel durchsuchbar, ihr Inhalt wird jedoch nicht indexiert und nicht in Textauszügen angezeigt, solange sie gesperrt sind. Der JSON-Export entschlüsselt nie: Verschlüsselte Notizen werden als Chiffrat exportiert, und der Export-Dialog warnt Sie vorher. Da die Erweiterung keinen Import unterstützt, lässt sich ein Chiffrat-Export nicht zum Lesen dieser Notizen verwenden — für eine lesbare Kopie entsperren Sie die Notiz und verwenden **Als Markdown kopieren** oder **.md herunterladen**. Ein ausstehender Rechtsklick-Ausschnitt wird in `chrome.storage.session` gehalten, solange ein Notebook-Passwort aktiv ist, damit sein Klartext nicht auf die Festplatte gelangt.

### Papierkorb (Premium)

- Wenn Premium aktiv ist, wandert eine gelöschte Notiz in den **Papierkorb**, statt entfernt zu werden.
- Papierkorb-Einträge lassen sich jederzeit innerhalb von **30 Tagen** wiederherstellen; danach werden sie automatisch gelöscht.
- **Papierkorb leeren** und **Endgültig löschen** entfernen Einträge sofort und können nicht rückgängig gemacht werden.
- Löschungen im kostenlosen Plan sind dauerhaft: Der 7-Sekunden-Undo ist die einzige Wiederherstellung.
- Wenn Premium abläuft, bleiben vorhandene Papierkorb-Einträge zum Wiederherstellen oder Löschen verfügbar; nur neue Löschungen folgen der Regel des kostenlosen Plans.

### Hinweise zur kostenlosen Version

- Kein Tageslimit für neue Notizen — der kostenlose Plan ist ein vollständiges Notizbuch, keine Testversion
- Die Bearbeitung bestehender Notizen ist immer unbegrenzt
- Titel-Sequenznummern können nach dem Löschen Lücken haben — das ist so gewollt

### Export & Download

- **Einzelne Notiz → .md-Datei**: Klick auf das ⬇-Symbol auf einer Notizkarte lädt sie als Markdown-Datei herunter (kostenlos)
- **Alle Notizen → JSON** (Premium): **📥 Export** lädt alle Notizen als strukturierte JSON-Datei herunter; Notizen mit Passwort bleiben Chiffrat
- Die exportierte Datei dient nur zur Sicherung/Referenz — **die Erweiterung unterstützt keinen Import von Notizen**, daher lassen sich verschlüsselte Notizen nicht aus der Datei lesen oder wiederherstellen

---

## FAQ

1. **Rechtsklick-Menü erscheint nicht?**
   Das Menü erscheint bei Textauswahl oder Rechtsklick auf ein Bild. Es verwendet die einheitliche Option „In vkt-note speichern".

2. **Notizen nach Neuinstallation verschwunden?**
   Alle Notizen sind in `chrome.storage.local` gespeichert. Deinstallation der Erweiterung löscht alle Daten dauerhaft. Exportieren Sie Ihre Notizen vor der Deinstallation (Premium exportiert alle Notizen als eine JSON-Datei, Notizen mit Passwort als Chiffrat; in der kostenlosen Version können Sie Notizen einzeln kopieren oder herunterladen).

3. **Bilder in Notizen werden nicht angezeigt?**
   Markdown-Bilder speichern nur Remote-URLs. Wenn die Quellseite nicht erreichbar ist, Hotlinking blockiert oder das Bild entfernt wurde, wird es nicht geladen.

4. **Kann ich exportierte Notizen importieren?**
   Nein. Der JSON-Export dient nur zur manuellen Sicherung. Die Erweiterung unterstützt keinen Import von Notizen.

5. **Gibt es ein Limit für neue Notizen?**
   Nein. Neue Notizen sind in beiden Plänen unbegrenzt; Premium bietet zusätzlich den Sammel-JSON-Export und einen 30-Tage-Papierkorb.

6. **Ich habe mein Passwort vergessen. Kann es wiederhergestellt werden?**
   Nein. Das Passwort wird nie gespeichert, nur ein Prüfwert, mit dem sich die Verschlüsselung nicht umkehren lässt. Ein Passwort pro Notiz lässt sich nur durch Löschen dieser Notiz umgehen. Bei einem vergessenen Notebook-Passwort löscht der Zurücksetzen-Vorgang dauerhaft alle dadurch geschützten Notizen, Papierkorb-Einträge und Entwürfe; Notizen mit eigenem Passwort bleiben erhalten.

7. **Sehe ich Notiztitel, wenn das Notizbuch gesperrt ist?**
   Ja. Titel, Zeitstempel und Wortzahlen bleiben bewusst sichtbar, damit Sie die gewünschte Notiz finden; Inhalt, Textauszüge und inhaltliche Suchtreffer bleiben verborgen, bis entsperrt wird. Die Titelsuche funktioniert weiterhin.

8. **Wie sehen verschlüsselte Notizen in einem Export aus?**
   Sie werden als Chiffrat exportiert, nicht als Klartext. Der Export-Dialog warnt Sie, wenn verschlüsselte Notizen enthalten sind. Da die Erweiterung keinen Import unterstützt, lässt sich die JSON-Datei nicht zum Lesen oder erneuten Importieren dieser Notizen verwenden. Für eine lesbare Kopie entsperren Sie die Notiz und verwenden **Als Markdown kopieren** oder **.md herunterladen**.

9. **Wohin gelangen gelöschte Notizen?**
   Mit Premium landen sie im Papierkorb und bleiben 30 Tage lang wiederherstellbar. Im kostenlosen Plan ist das Löschen nach dem 7-Sekunden-Undo-Zeitfenster endgültig.

---

## Datenschutz

vkt-note folgt den Privacy-by-Design-Prinzipien:

- ✅ Alle Notizen in `chrome.storage.local` gespeichert — **Notizinhalte werden niemals an einen Server übertragen**
- ✅ Optionaler Passwortschutz verschlüsselt Notizinhalte im Ruhezustand mit AES-256-GCM (PBKDF2-HMAC-SHA256, 600.000 Iterationen); Passwörter und abgeleitete Schlüssel werden niemals gespeichert oder übertragen
- ✅ Die einzige ausgehende Anfrage ist die optionale Premium-Lizenzprüfung (Lizenzschlüssel, eine zufällige Installationskennung, grundlegende Browser-Metadaten) — keine Notizen, keine Seiten-URLs
- ✅ Keine Analyse, kein Tracking, keine Cookies
- ✅ Seiteninhalt wird nur bei explizitem Auslösen von Speichern/Einfügen/Tabellenauswahl gelesen (Kontextmenü, Einfügen-Buttons, Tabellenauswahl) — nie im Hintergrund
- ✅ Exportierte JSON-Dateien werden lokal erstellt und niemals übertragen; verschlüsselte Notizen bleiben in Exporten als Chiffrat erhalten

### Berechtigungen

| Berechtigung | Grund |
|--------------|-------|
| `storage` | Notizen und Einstellungen lokal speichern |
| `unlimitedStorage` | Hebt die standardmäßige lokale Speichergrenze an, damit eine lange Notizhistorie nie an ein Schreiblimit stößt |
| `sidePanel` | Erweiterungs-UI in einer Seitenleiste anzeigen |
| `contextMenus` | Rechtsklick-Menü zum Erstellen von Notizen aus Textauswahl oder Bildern |
| `scripting` | HTML→Markdown-Konverter nur bei Speichern/Einfügen/Tabellen-Aktionen injizieren |
| `alarms` | Führt den täglichen Auftrag aus, der Papierkorb-Einträge entfernt, die älter als 30 Tage sind |
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
