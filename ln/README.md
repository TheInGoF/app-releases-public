[← Alle Apps](../README.md)

# Leistungsnachweis

Leistungsnachweise (Stundenzettel) je Mitarbeiter, Projekt und Monat erfassen – mit Wochenblättern, Projektübersicht,
Archiv und PDF mit Signaturfeldern. Mehrere Mitarbeiter können dieselbe Datei nutzen (z. B. im OneDrive).

## Download

Im [neuesten Leistungsnachweis-Release](https://github.com/TheInGoF/app-releases-public/releases?q=ln-v&expanded=true)
die Datei `Leistungsnachweis vX.Y.exe` laden (Windows 10/11). Zu jeder Datei gibt es eine `.sha256` mit der Prüfsumme.

## Installation

Keine Installation nötig. Die Exe in einen eigenen Ordner legen (gern im OneDrive) und starten.
Braucht die Microsoft Edge WebView2-Runtime (bei Windows 10/11 meist vorhanden).

- **Daten:** stehen in der Programmdatei selbst. Wer die Datei weitergibt, gibt die Nachweise mit.
- **Logo:** optional eine `logo.png` in denselben Ordner legen – sie erscheint auf den Blättern und im PDF.
- **PDFs:** werden im selben Ordner gespeichert.
- **Umstieg von einer älteren Version:** neue Exe in denselben Ordner legen und starten – sie übernimmt alle Daten,
  die alte Version wird danach gelöscht.

## Mehrere Nutzer, OneDrive

- Jeder Rechner/Windows-Benutzer wird einmal einem Mitarbeiter zugeordnet; die App öffnet immer dessen eigenen Leistungsnachweis.
- Ist der Nachweis eines Kollegen offen, steht oben ein Hinweis. Von dort kann man Tage nur **in den eigenen** Nachweis übernehmen.
- ↶ / ↷ oben in der Leiste nehmen Änderungen zurück bzw. wiederholen sie.
- Die App schreibt spätestens eine Minute nach einer Änderung in die Datei und liest vorher den aktuellen Stand ein.
  Legt OneDrive trotzdem Konfliktkopien an, führt die App sie beim nächsten Abgleich zusammen und löscht sie –
  bei Abweichungen gewinnt der neuere Eintrag, der andere bleibt im Verlauf.

## Updates

Die App prüft beim Start und alle 6 Stunden, ob es hier eine neuere Version gibt, und bietet „Jetzt aktualisieren“ an.
Dann speichert sie, startet die neue Version, die alle Daten übernimmt, und löscht die alte.
Von Hand: ☰ → Impressum → „Nach Update suchen“.

## Datenschutz

Alle Daten bleiben in der Programmdatei und den PDFs auf dem eigenen Rechner bzw. der eigenen Ablage.
Ins Internet geht nur die Update-Prüfung bei GitHub.

## Lizenz

Private Nutzung kostenlos, beruflich/kommerziell nur mit Zustimmung. Siehe [LICENSE](../LICENSE).
