# Als Team arbeiten

**Personen-Symbol → "Team"**

Mit der Team-Freigabe arbeitet ihr mit demselben Firmenwissen. Alles Geteilte wird **auf deinem eigenen Computer verschlüsselt**, bevor es irgendwohin geht, und es synchronisiert sich über Infrastruktur, **die dir gehört**. Nichts läuft über einen Taibu-Server.

## So funktioniert es

Der Teamleiter erstellt **Bereiche**. Das sind Gruppen wie Vertrieb, Marketing oder ein Bereich pro Kunde. Er legt fest, wer in welchem Bereich ist, und wählt aus, was geteilt wird. Ein Teammitglied ohne Schlüssel für einen Bereich kann diesen Bereich wirklich nicht lesen, selbst wenn es den Sync-Ordner sehen kann.

![Bereiche, die Zugriffs-Matrix und die Schalter für geteilte Ordner](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/23-team-admin.png)

## Wohin es synchronisiert

| Option | Gut für |
|---|---|
| **Geteilter Ordner** | Am einfachsten und am schnellsten. Zeige auf einen Ordner, den Syncthing, ein NAS oder ein Cloud-Laufwerk synchron hält |
| **Git-Repository** | Dein eigenes privates Repo mit voller Historie. Alle müssen sich vorher bei git angemeldet haben |

Für ein Git-Repository muss sich jede Person auf ihrem Rechner bei git angemeldet haben, bevor es funktioniert. Führe `gh auth login` aus oder klone das Repo einmal von Hand, damit die Anmeldung gespeichert wird. Taibu speichert dein Token nie und nutzt deshalb die git-Anmeldung deines Systems. Wenn sie fehlt, zeigt dir die Team-Seite das an.

## Einrichten, Leiter

1. **"Ein Team erstellen"**, benenne es und wähle Ordner oder git
2. Füge einen **Bereich** hinzu, zum Beispiel `company`
3. Schalte ein, was geteilt werden soll
4. Kopiere den **Team-Code** und sende ihn an deine Kollegen

## Beitreten, Mitglied

1. Füge den Team-Code unter **"Einem Team beitreten"** ein
2. Drücke **"Jetzt synchronisieren"**. Du siehst dann "Warte auf deinen Admin"
3. Dein Leiter gibt dich mit einem Klick frei, und dein Zugriff kommt bei der nächsten Synchronisierung an

![Was ein Mitglied sieht, während es auf die Freigabe wartet](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/24-team-pending.png)

Du sendest nur ein einziges Mal einen Code.

## Was du teilen kannst

Firmen-Playbook, Firmenregeln, Erinnerungen, Firmenkontext, Skills, Referenzen, Entscheidungen, Tools und jeden Ordner, den du auswählst.

Wenn du einen Ordner ausschaltest, endet die Freigabe ab diesem Moment. Es ist kein Löschen. Jeder behält die Kopie, die schon da ist, und deine eigenen Dateien bleiben genau dort, wo sie sind.

## In eine Richtung oder in beide

Jedes Element hat die Einstellung **"Wer darf das ändern"**:

- **Nur ich**: Die Kopie des Leiters ist die maßgebliche Version. Mitglieder lesen sie. Ihre Änderungen werden nie weitergegeben. Nutze das für verbindliche Firmeninhalte
- **Jeder im Bereich**: In beide Richtungen. Alle tragen bei und erhalten Änderungen. Nutze das für geteilte Erinnerungen

Bei widersprüchlichen Änderungen bleibt die neueste Version erhalten. Die andere wird daneben gespeichert, damit nichts verloren geht.

## Firmenregeln, ohne etwas zu überschreiben

Deine Anweisungsdatei mischt Firmenvorgaben mit persönlichen Dingen wie deinem Namen, deiner Sprache und deinen Prioritäten. Deshalb synchronisiert Taibu diese Datei nie.

Stattdessen schreibt der Leiter die Firmenregeln an einer Stelle, und Taibu fügt sie bei jedem Mitglied in einem markierten Block in die eigenen Anweisungen ein. Persönliche Einstellungen bleiben unberührt. Änderst du eine Regel, bekommen sie alle.

## Was nie geteilt wird

**Dein persönliches Profil und deine Stimme verlassen nie deinen Computer**, egal was die Einstellungen sagen. Jeder behält seine eigene Art zu schreiben. Erinnerungen ohne Bereich sind privat. Das ist die Standardeinstellung.

## Team-Einblicke

Der Leiter kann Aktivitätsberichte einschalten. Jedes Mitglied entscheidet selbst, ob es mitmacht, und sieht genau, was gesendet würde.

**Gesendet:** wie viele Unterhaltungen und mit welchen Agenten, wie Erinnerungen gewachsen sind, Themen- und Skill-Namen, Aktivität pro Tag und wo Arbeit festzustecken scheint.

**Nie gesendet:** was du geschrieben hast oder die KI geantwortet hat, deine Entwürfe, deine privaten Erinnerungen, deine Schlüssel, alles Persönliche.

![Die Einwilligungs-Karte, die ein Mitglied sieht](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/25-team-consent.png)

Es wird nichts gesendet, bis du zustimmst, und du kannst es jederzeit beenden.

## Wichtige Grenzen

- Jemanden zu entfernen wirkt nur für die Zukunft. Seine Schlüssel werden ersetzt, damit er nichts Neues mehr bekommt, aber bereits synchronisierte Kopien bleiben auf seinem Rechner
- Das Gerät des Leiters enthält den Hauptschlüssel des Teams. Sichere ihn wie ein Passwort
- Teilen ist für Wissen gedacht, nicht für Medien. Es gibt ein Größenlimit pro Bereich
- Die Team-Mitgliedschaft gilt pro Projekt. Wenn du ein Projekt verbindest, bleiben deine anderen unberührt
