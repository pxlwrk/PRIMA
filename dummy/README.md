# PRIMA – Klick-Dummy

Ansprechender, moderner Klick-Dummy für das PRIMA Service-Portal (**Mobile First**). Zeigt das Dashboard und die sechs Services (Störung melden, Fortbildung, Raum buchen, Dienstreise, Krank- & Gesundmeldung) mit klickbarer Navigation.

- **Smartphone:** Oberer Header (Logo + User), Inhalt, feste Bottom-Navigation
- **Tablet/Desktop (ab 768px):** Sidebar mit Navigation, kein Bottom-Nav, mehrspaltige Karten/Listen

## Anzeigen

`index.html` im Browser öffnen (Doppelklick oder „Mit Browser öffnen“). Es wird kein Server benötigt.

```bash
open dummy/index.html
```

Oder mit einem lokalen Server (z. B. Python):

```bash
cd dummy && python3 -m http.server 8080
```

Dann im Browser: http://localhost:8080

## Inhalt

- **Übersicht:** Dashboard mit vier Service-Karten
- **Störung melden:** Formular (Kategorie, Beschreibung, Details)
- **Fortbildung beantragen:** Formular (Art, Anbieter, Zeitraum, Begründung)
- **Raum buchen:** Datum/Zeit + Auswahl verfügbarer Räume (Klick = Buchung)
- **Dienstreise beantragen:** Formular (Ziel, Datum, Verkehrsmittel)
- **Krank- & Gesundmeldung:** Tab-Umschaltung „Krankmelden“ / „Gesundmelden“ mit je eigenem Formular (Daten, Anmerkung)

Navigation über Sidebar und „Zurück zur Übersicht“. Bei „Absenden“ erscheint eine kurze Bestätigung (Toast). Keine Daten werden gespeichert.
