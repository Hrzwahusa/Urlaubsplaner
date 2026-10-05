# Ferienfrei-Planer

Kalender, der die Schulferien aller 16 Bundesländer anzeigt und Zeiträume findet, in denen in keinem der ausgewählten Länder Ferien sind.

- Bundesländer und Ferienarten (Winter, Ostern, Pfingsten, Sommer, Herbst, Weihnachten, Einzeltage) einzeln an- und abwählbar
- Liste der ferienfreien Zeiträume mit Mindestlänge, Kalenderwochen und Werktagen
- Jahreskalender mit Farbskala (Anzahl der Länder mit Ferien) und Tagesdetails
- Auswahl wird im Browser gespeichert (localStorage)

## Daten

Beim Öffnen werden die Termine für das aktuelle und die zwei folgenden Jahre live von der
[OpenHolidays API](https://www.openholidaysapi.org) geladen. Ist die API nicht erreichbar,
nutzt die Seite eingebaute Ersatzdaten (Stand 05.10.2026, Dez. 2025 bis Jan. 2028).

- Mecklenburg-Vorpommern: Termine der allgemeinbildenden Schulen
- Schleswig-Holstein: ohne Sonderregelung der Nordseeinseln
- Gesetzliche Feiertage werden nicht berücksichtigt

## Hosting mit GitHub Pages

Die Seite ist eine einzelne `index.html` ohne Build-Schritt.

1. Repository anlegen und `index.html` in den Hauptzweig legen
2. *Settings → Pages → Build and deployment*: Source „Deploy from a branch“, Branch `main`, Ordner `/ (root)`
3. Nach ca. einer Minute ist die Seite unter `https://<benutzername>.github.io/<repo>/` erreichbar
