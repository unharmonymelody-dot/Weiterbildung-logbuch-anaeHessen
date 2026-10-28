# Weiterbildungs-Logbuch Anästhesiologie

Persönliche Dokumentationshilfe für die Facharztweiterbildung **Anästhesiologie** nach der **Weiterbildungsordnung für Ärztinnen und Ärzte in Hessen 2020** (zuletzt geändert am 23.11.2024). Funktioniert auf iPhone, Android und am Computer, ohne Account und ohne Installation aus einem App-Store.

**App öffnen:** https://BENUTZERNAME.github.io/weiterbildung-logbuch/

## Was die App kann

- Alle Weiterbildungsinhalte des Facharztes Anästhesiologie und die „Allgemeinen Inhalte Abschnitt B“ (107 Inhalte, 22 Richtzahlen)
- Tageweise erfassen: Zähler mit +1, Kenntnisse und Fertigkeiten abzeichnen, optional kurze Notiz
- Fortschritt je Kategorie und gesamt, mit Ist, Soll und noch Fehlendem
- Weiterbildungszeiten (60 Monate, davon 12 Monate Intensivmedizin) mit Abschnitten
- Verlauf aller Einträge, bearbeiten und löschen
- Export als CSV (Excel), Sicherungsdatei, druckbarer Bericht

## Als App installieren

**iPhone / iPad (Safari)**
1. Link in **Safari** öffnen.
2. Unten auf das Teilen-Symbol (Quadrat mit Pfeil nach oben) tippen.
3. „Zum Home-Bildschirm“ wählen und bestätigen.
4. Die App künftig nur noch über das Icon auf dem Home-Bildschirm öffnen.

Wichtig: Installiere die App, **bevor** du Daten einträgst. Die installierte App hat einen eigenen Speicher und übernimmt keine Daten aus dem Safari-Tab. Ohne Installation löscht Safari Website-Daten nach 7 Tagen ohne Nutzung.

**Android (Chrome)**
1. Link in **Chrome** öffnen.
2. Auf „Jetzt installieren“ tippen oder im Menü (drei Punkte) „App installieren“ bzw. „Zum Startbildschirm hinzufügen“ wählen.

**Computer (Chrome, Edge)**: In der Adressleiste auf das Installieren-Symbol klicken, oder die Seite einfach im Browser nutzen.

## Daten und Datenschutz

- Alle Einträge bleiben **auf deinem Gerät**. Es gibt kein Konto, keinen Server der App und keine Nachverfolgung.
- Bitte **keine Patientennamen oder -daten** in Notizen eintragen. Die App ist für Zähler und Kürzel gedacht.
- Die Daten sind pro Gerät getrennt. Wer Handy und Computer nutzt, überträgt sie über „Daten → Sicherung speichern“ und „Sicherung laden“ (Zusammenführen).
- **Sicherungen:** Speichere unter „Daten“ regelmäßig eine Sicherungsdatei und lege sie in deiner Cloud ab. Wird die App gelöscht oder der Browserspeicher geleert, sind die Einträge sonst weg.
- Beim Aufruf der Seite verarbeitet der Hoster (GitHub Pages) technisch bedingt Server-Logdaten wie die IP-Adresse. Nach dem ersten Laden läuft die App ohne Internet.

## Updates

Neue Versionen laden sich automatisch, sobald du die App mit Internetverbindung öffnest. Beim nächsten Start ist die neue Version aktiv. Deine Daten bleiben dabei erhalten. Die Versionsnummer steht unter „Daten → Hinweise“.

## Wichtige Hinweise

- Dies ist **keine offizielle Anwendung** der Landesärztekammer Hessen und ersetzt nicht das elektronische Logbuch. Die verbindliche Dokumentation erfolgt dort mit mindestens jährlicher Bestätigung durch den Weiterbildungsbefugten (§ 2a Abs. 7 und § 8 WBO).
- Die Inhalte wurden sorgfältig aus der WBO 2020 übernommen, ersetzen aber nicht den Originaltext. Maßgeblich sind die aktuelle Weiterbildungsordnung und die Vorgaben der Landesärztekammer. **Keine Gewähr** für Vollständigkeit und Richtigkeit. Bitte Änderungen der WBO selbst prüfen.
- Die Monatsberechnung bei den Zeiten ist eine Näherung. Maßgeblich sind die Zeugnisse der Weiterbildungsbefugten.

## Fehler oder Wünsche

Bitte über den Reiter **Issues** dieses Repositorys melden. Bitte dort **keine** persönlichen Daten angeben.

## Für Entwickler

Reine statische Seite ohne Build-Schritt und ohne externe Abhängigkeiten:
`index.html` (App mit Daten), `manifest.webmanifest`, `sw.js` (Offline-Cache), Icons.
Bei einer neuen Version die Nummer in `sw.js` (`CACHE`) und in `index.html` (`APP_VERSION`) erhöhen.
Die WBO-Inhalte stehen als Datenstruktur (`const DATA`) am Anfang des Skripts in `index.html`.
