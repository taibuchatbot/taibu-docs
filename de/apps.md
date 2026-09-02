# Apps

Taibu schreibt nicht nur über dein Unternehmen. Es kann auch **Software dafür bauen**. Du beschreibst, was du sehen willst, es holt die Daten aus den verbundenen Tools, schreibt die Seite und fügt sie hier hinzu. Kein Entwickler, keine monatliche SaaS-Gebühr, keine Preise pro Platz.

**Rastersymbol → "Apps"**

![Die Apps-Seite](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/22-apps.png)

## Eine anfordern

Das Feld oben auf der Seite ist die ganze Oberfläche. Tippe, was du sehen willst, und drücke **"Build it"** oder Strg+Enter. Das öffnet einen **neuen Agenten** für den Job: Er plant die App, baut sie und trägt sie auf dieser Seite ein, wenn er fertig ist. Du kannst in der Zwischenzeit in einem anderen Tab weiterarbeiten.

Du weißt nicht genau, was du fragen sollst? Schau auf das Feld. Es tippt echte Beispiele, solange du nichts machst.

![Die Apps-Seite, bevor etwas gebaut wurde](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/22b-apps-empty.png)

Jede Kachel ist ein **Live-Render der App selbst**, kein Symbol. So erkennst du sie auf einen Blick. Eine Kachel mit **"Not running"** ist eine Live-App, deren Server gestoppt ist. Öffne sie und drücke **"Start server"**.

## Ein Dashboard statt vier Browser-Tabs

Die meisten Unternehmen haben dieselbe Lücke. Werbeausgaben liegen in Facebook Ads. Mehr Ausgaben liegen in Google Ads. Leads kommen über ein Formular auf der Website rein. Ob daraus Geld wurde, steht im CRM. Nichts verbindet diese Daten. Darum kann niemand die einzige wichtige Frage beantworten: Welcher Kanal bringt wirklich Geld?

Verbinde diese Tools und frage dann in einem Satz:

> "Baue mir ein Live-Dashboard: Werbeausgaben aus Facebook und Google, Leads aus dem Website-Funnel und welche dieser Leads wir in ClickUp gewonnen haben. Zeige Kosten pro Lead und Rendite nach Kanal."

![Eine gebaute App, geöffnet in Taibu](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/29-app-open.png)

Schau, was das beantwortet. Facebook bringt 171 Leads zu je 29 Euro, Google bringt 84 zu 42. Bei den Kosten pro Lead gewinnt Facebook, und die meisten würden das Budget dorthin verschieben. Aber Google hat 10 seiner 84 abgeschlossen, Facebook 9 von 171. Darum brachte Google das 5,5-Fache zurück und Facebook 2,7. Der günstigere Kanal war der schlechtere. Und keine der Werbeplattformen kann dir das sagen, weil keine weiß, was abgeschlossen wurde.

## Andere Dinge, die sich lohnen

- **Liquidität und Runway**: Bank plus ausgehende Rechnungen, damit du die echte Zahl kennst
- **Pipeline nach Phase**: CRM-Deals und wie lange jedes feststeckt
- **Kundenbericht**: Eine Seite pro Kunde, die du am Monatsende schicken kannst
- **Lead-Qualität nach Quelle**: Nicht wer die meisten Leads sendet, sondern wer die Leads sendet, die unterschreiben

## Live oder Schnappschuss

| Art | So funktioniert es | Nutze es, wenn |
|---|---|---|
| **Live** | Startet einen kleinen lokalen Server und liest die Daten jedes Mal neu, wenn du es öffnest | Es ist für dich und du willst die Zahlen von heute |
| **Schnappschuss** | Eine einzelne HTML-Datei mit eingebetteten Daten, ohne Server | Du willst sie an einen Kunden oder deinen Steuerberater senden |

Ein Schnappschuss ist eine Datei. Schick sie ab und sie öffnet sich einfach. Die Person, die sie bekommt, braucht nichts installiert.

## Selbst eines hinzufügen

Manchmal gibt es nichts zu bauen: Du hast schon eine HTML-Datei oder einen eigenen Server, der schon läuft. **"Add one manually"** unten auf der Seite nimmt einen Namen, eine Adresse, wie http://localhost:8000, oder eine HTML-Datei und optional einen Startbefehl. Der Startbefehl läuft im eingebauten Terminal, wenn du die App öffnest. So startet der Server von selbst.

## Wenn eine App leer ist

Ihr Server läuft nicht. Drücke **"Start server"** oder starte ihn selbst und dann **"Reload"**. Schnappschüsse machen das nie, weil es keinen Server zum Starten gibt.

## Wohin die Daten gehen

Eine App läuft auf deinem Computer und liest aus den Tools, die du verbunden hast. Nichts wird zu Taibu hochgeladen. Die Seite ist eine Datei in deinem Projekt, die du wie jede andere öffnen, bearbeiten oder löschen kannst.
