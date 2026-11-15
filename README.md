# QR-Generator

Ein **offline nutzbares Ein-Datei-Werkzeug** (eine einzige `qr-generator.html`),
das druckreife QR-Codes erzeugt – mit Beschriftung, Logo, exakten Druckmaßen,
Lesbarkeitsprüfung und Export als **PNG, SVG und CMYK-Druck-PDF**. Zusätzlich
können Kontakt-QR-Codes (vCard) und ganze **Serien** aus einer Excel-/CSV-Tabelle
gebaut werden.

Das Werkzeug ist aus der täglichen Produktionsarbeit im Kommunikationsdesign
entstanden und auf fehlerfreien Druck ausgelegt.

> **Keine Installation, kein Server, keine Cloud.** Die Datei läuft komplett im
> Browser; Inhalte und Logos verlassen den Rechner nicht. Eine strenge
> Content-Security-Policy sperrt jeden Netzzugriff.

## Loslegen

1. `qr-generator.html` herunterladen und per Doppelklick im Browser öffnen
   (Chrome, Firefox, Safari, Edge).
2. Inhalt eingeben (Link, Text oder Kontakt), Gestaltung und Druckgröße wählen.
3. Exportieren – **PNG**, **SVG** oder **Druck-PDF (CMYK)**.

Eine Web-Fassung läuft unter **https://dwbkd.de/qr/**.

## Funktionen

**Code & Lesbarkeit**
- Fehlerkorrektur wird kostenlos so hoch wie möglich gesetzt, solange die
  Version gleich bleibt.
- **Fehlerreserve** wird live berechnet (Ampel grün/gelb/rot), damit ein Logo
  den Code nie unlesbar macht.
- Laufende **Lesbarkeitsprüfung** dekodiert den gerenderten Code gegen eine
  Referenz.
- Eingabe wird bereinigt (unsichtbare Zeichen, Umlaut-Domains → Punycode,
  optionales Entfernen von Tracking-Parametern mit Versionsersparnis).

**Gestaltung**
- Beschriftung unter dem Code (Adresse oder eigener Text).
- Logo per Drag & Drop oder Einfügen (auch SVG), optional in Codefarbe
  eingefärbt, mit passender Freifläche und Auflösungswarnung.
- Modulformen (eckig, abgerundet, Konturen), eigene Farben inkl.
  CI-Farbauswahl mit Live-Kontrastprüfung, transparenter Hintergrund.

**Druck**
- Feld für **Druckgröße in mm** und Scanabstand → Ampel für die Modulgröße.
- **Druck-PDF in DeviceCMYK** (exakte CI-CMYK-Werte, dunkle Grautöne → 100 K,
  Beschriftung als hochaufgelöste Schablone, Logo als CMYK-Fläche).
- SVG in Moduleinheiten mit mm-Maßen, PNG mit ganzzahligen Pixeln pro Modul.

**Kontakte & Serien**
- Kontakt-QR als **vCard** (Android- und iPhone-tauglich), inkl. Social-Profile.
- **Serie** aus Excel/CSV: je Zeile PNG/SVG/PDF/VCF als ZIP, gleiche Modulzahl.
  Eine Vorlage liegt als [`QR-Serie-Vorlage.xlsx`](QR-Serie-Vorlage.xlsx) bei.
- Einstellungen als Datei speichern und laden.

## Haftung

Kostenlos, ohne Gewähr, Nutzung auf eigene Verantwortung – siehe
[HAFTUNGSAUSSCHLUSS.md](HAFTUNGSAUSSCHLUSS.md). Prüfen Sie jeden Code vor
Druck oder Veröffentlichung selbst durch einen Testscan.

## Lizenz

[MIT](LICENSE) · © 2026 Daniel W. Bittner · Kommunikationsdesign (dwbkd)
