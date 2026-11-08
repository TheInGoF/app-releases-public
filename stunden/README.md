[← Alle Apps](../README.md)

# Stunden

Persönliche Arbeitszeiterfassung: Arbeitszeit, Projekte, Pausen, Zuschläge, Verpflegung, Lohn-/Netto-Vorschau.
Daten liegen verschlüsselt in einer eigenen Datei oder auf einem Stunden-Server (Ende-zu-Ende-verschlüsselt).

## Download

Im [neuesten Stunden-Release](https://github.com/TheInGoF/app-releases-public/releases?q=stunden-v&expanded=true) die passende Datei wählen:

| System | Datei |
|---|---|
| Windows 10/11 | `Stunden vX.Y.Z.exe` |
| Mac mit Apple-Chip (M1 und neuer) | `Stunden-vX.Y.Z-Mac-AppleSilicon.zip` |
| Mac mit Intel-Chip | `Stunden-vX.Y.Z-Mac-Intel.zip` |
| Linux (64 Bit) | `stunden-vX.Y.Z-linux-amd64` (ARM: `…-linux-arm64`) |

Zu jeder Datei gibt es eine `.sha256` mit der Prüfsumme.

## Installation

Keine Installation nötig – die Apps sind portabel. Am besten in einen eigenen Ordner legen (z. B. `Dokumente\Stunden`).

**Windows:** Exe starten. Braucht die Microsoft Edge WebView2-Runtime (bei Windows 10/11 meist vorhanden).

**Mac:** Zip entpacken, `Stunden.app` z. B. in „Programme“ ziehen. Beim ersten Start meldet macOS „nicht verifizierter Entwickler“:
Systemeinstellungen → Datenschutz & Sicherheit → „Dennoch öffnen“ (ältere macOS: Rechtsklick → Öffnen). Nur einmal nötig.
Meldet macOS stattdessen „beschädigt“, im Terminal einmal `xattr -dr com.apple.quarantine /Applications/Stunden.app` ausführen
(Pfad anpassen) – danach startet die App. Updates lädt sie anschließend selbst.
Die App öffnet ein eigenes Fenster, wenn Chrome, Edge, Chromium oder Brave installiert ist, sonst den Standardbrowser.

**Linux:** Datei ausführbar machen (`chmod +x stunden-v…-linux-amd64`) und starten. Eigenes Fenster wie beim Mac,
sonst Standardbrowser. Die App beendet sich einige Minuten nach dem Schließen des Fensters.

## Updates

Die App prüft beim Start und alle 6 Stunden, ob es hier eine neuere Version gibt, und bietet „Jetzt aktualisieren“ an.
Die neue Version kommt in denselben Ordner, die alte wird danach gelöscht. Daten und Einstellungen bleiben.
Von Hand: Impressum → „Nach Update suchen“.

## Datenschutz

Die App selbst sendet nichts ins Internet – außer der Update-Prüfung bei GitHub und, falls eingerichtet, der Verbindung
zum eigenen Stunden-Server (dort nur verschlüsselte Daten).

## Lizenz

Private Nutzung kostenlos, beruflich/kommerziell nur mit Zustimmung. Siehe [LICENSE](../LICENSE).
