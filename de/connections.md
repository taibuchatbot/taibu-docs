# Verbindungen und Schlüssel

**Stecker-Symbol → "Verbindungen"**. Das sind die Systeme, auf die deine KI zugreifen kann. Verbinde ein Tool einmal, dann können alle Skills und Routinen es nutzen.

Grün bedeutet bereit, Gelb bedeutet teilweise eingerichtet, Grau bedeutet nicht verbunden.

![Die Seite „Verbindungen“](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/20-connections.png)

## Drei Arten

**Tools mit API-Schlüssel**. Dazu gehören Stripe, HubSpot, QuickBooks, Meta Ads, Google Ads und lokal Merit Aktiva, Montonio, Pipedrive. Klicke auf "Verbinden". Taibu erklärt dir, welche Schlüssel du brauchst, wo du sie bekommst, und führt dich durch das Hinzufügen.

**Live-Verbindungen**. Dazu gehören Notion, Slack, ClickUp, GitHub, Browser. Klicke auf "Verbinden". Taibu richtet es dann Schritt für Schritt mit dir ein.

**Claude-Konto-Connectoren**. Dazu gehören Gmail, Google Drive, Google Calendar. Du aktivierst sie in Claudes eigenen Connector-Einstellungen. Sie sind an dein Konto gebunden, nicht an ein einzelnes Projekt. Wenn sie dort verbunden sind, funktionieren sie überall.

Welche Tools angeboten werden, hängt von der Sprache ab. Nützliche Buchhaltungs- und CRM-Tools unterscheiden sich je nach Markt.

"Test" macht einen kleinen Leseaufruf ohne Änderungen. So prüft Taibu, ob eine Verbindung funktioniert.

## Schlüssel

**Zahnrad-Symbol → Einstellungen → "Schlüssel"**

Füge einen Schlüssel mit Namen, zum Beispiel STRIPE_SECRET_KEY, und Wert hinzu. Klicke dann auf "Hinzufügen". Die Augen-Schaltfläche zeigt einen Wert an. Der Papierkorb entfernt ihn. Änderungen speichert Taibu, wenn du wegklickst oder Enter drückst.

![Der Tab „Schlüssel“](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/21-keys.png)

**Füge niemals einen API-Schlüssel in den Chat ein.** Taibu schickt dich stattdessen immer zu diesem Bereich. Schlüssel werden pro Projekt in einer einfachen Datei auf deiner Festplatte gespeichert. Behandle den Ordner deshalb wie eine Passwortdatei. Lege ihn nicht in öffentliche Repositories oder geteilte Laufwerke.
