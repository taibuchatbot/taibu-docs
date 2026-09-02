# Deine Daten: was Taibu über dich schreibt

Taibu speichert alles, was es weiß, in normalen Dateien in deinem Projektordner. Nichts steckt versteckt in einer Datenbank, und nichts liegt auf einem Taibu-Server. Diese Seite ist die Karte dazu: was jede Datei enthält, wie sie geschrieben wird und welche Dateien je einen Kollegen erreichen können.

Öffne jede davon im Dateibaum links.

## Du, persönlich

| Datei | Wie sie geschrieben wird | Was darin ist |
|---|---|---|
| `intake.md` | Der Einrichtungsassistent und danach **Einstellungen → "Meine Daten und Ziele"** | Deine sieben Antworten: wer du bist und was du verkaufst, ein oder zwei Beispiele deines Schreibstils, deine Prioritäten für das Quartal, wo Umsatz eingeht, wo du mit Leuten sprichst, wo deine Dokumente liegen und was deine Woche auffrisst |
| `context/persona.md` | Nur der Skill `/learn-me`, und nur nachdem du jede Änderung freigegeben hast | Dein digitales Abbild: deine Sprach- und Stilregeln, was du erreichen willst und warum, wie du entscheidest, was du magst und was dich nervt, die Menschen um dich herum |

**Keine dieser beiden Dateien wird je mit einem Team geteilt.** Sie werden auf der Sync-Ebene blockiert. So bleiben sie auf deinem Computer, selbst wenn jemand den Ordner teilt, in dem sie liegen. Sie sind auch der Grund, warum Taibu wie du klingt und nicht wie ein generischer Assistent. Darum lohnt es sich, sie genau zu halten.

`persona.md` wird nie heimlich neu geschrieben. `/learn-me` schlägt Änderungen aus echten Belegen vor, aus deinen tatsächlichen Entwürfen und deinen Korrekturen, und du gibst sie einzeln frei.

## Dein Unternehmen

| Datei | Was hineingehört |
|---|---|
| `company/offer.md` | Was du verkaufst, deine Preise, was dich unterscheidet |
| `company/icp.md` | An wen du verkaufst, welches Problem diese Leute haben, wo du sie findest |
| `company/strategy.md` | Wohin das Unternehmen geht und was gerade wichtig ist |
| `company/sops/<process>.md` | Eine Datei pro wiederholbarem Prozess: so machen wir X |

Diese Dateien füllen sich beim Arbeiten. Beschreibe, wie etwas gemacht wird, setze einen Preis fest, definiere einen Kunden oder gib eine Richtung vor, und Taibu schreibt es in die richtige Datei und sagt dir in einer Zeile, was es festgehalten hat.

Die Trennung ist wichtig: **`company/` ist das, was das Unternehmen weiß, und es kann mit einem Team geteilt werden. `context/persona.md` und `intake.md` sind das, wer du bist, und sie können es nicht.** Genau deshalb sind es getrennte Ordner.

## Entscheidungen, Referenzen, Verbindungen

| Datei oder Ordner | Was es ist |
|---|---|
| `decisions/log.md` | Datierte Entscheidungen mit dem Grund dahinter. Wenn du etwas entscheidest, bietet Taibu an, es zu protokollieren |
| `references/` | Frameworks, Sprachbeispiele und ein Leitfaden pro verbundenem Tool. `references/voice.md` ist das Verzeichnis, in das Taibu schreibt |
| `connections.md` | Das Verzeichnis aller Systeme, die Taibu kennt, verbunden oder nicht. **Führe `/audit` aus, um den echten Status zu sehen** |
| `.env` | Deine API-Schlüssel. Nie geteilt, nie im Chat gezeigt, und ausgefüllt über **Einstellungen → "Schlüssel"** statt von Hand |

## Deine Anweisungen

`CLAUDE.md` im Projektstamm ist die dauerhafte Anweisungsdatei: wie Taibu mit dir arbeiten soll, wo Dinge liegen, welche Regeln es befolgen muss. Sie wird am Anfang jedes Gesprächs geladen. `AGENTS.md` ist dasselbe für die OpenAI Codex Engine.

Du kannst sie bearbeiten. Wenn du merkst, dass du eine Anweisung im Chat wiederholst, schreibe sie stattdessen dort hinein, dann gilt sie ab dann.

Wenn du in einem Team bist, erscheinen die geteilten Regeln deines Admins in einem markierten Block in dieser Datei. Alles außerhalb dieses Blocks bleibt deins.

## Erinnerung

Die drei Ebenen der Erinnerung, `memory.md`, `memory/facts/` und `memory/journal/`, haben eine eigene Seite. Siehe **Woran sich Taibu erinnert**.

## Das Aktivitätsprotokoll

Taibu führt ein Protokoll darüber, was in der App passiert: was du angefragt hast, jedes Tool, das ein Agent ausgeführt hat und womit, und Dateien, die die App geschrieben, umbenannt oder gelöscht hat. Es gibt dieses Protokoll, damit es auf die Frage, was passiert ist, eine klare Antwort gibt und nicht nur eine Erinnerung.

Drei Dinge machen es nützlich:

- **Es ist immer an.** Du kannst es nicht ausschalten, und Taibu auch nicht. Ein Protokoll, das man vor einer Handlung abschalten kann, ist kein Protokoll.
- **Es kann nicht bearbeitet werden.** Jeder Eintrag ist an den vorherigen gebunden. Wenn ein Eintrag geändert oder entfernt wird, ist danach alles kaputt. **Einstellungen → Aktivitätsprotokoll** zeigt dir, ob es intakt ist, und nennt den ersten Eintrag, der es nicht ist, falls etwas verändert wurde.
- **Eine unabhängige Stelle bestätigt es.** Von Zeit zu Zeit sendet Taibu eine Prüfsumme des Protokolls, und sonst nichts, an einen unabhängigen Zeitstempel-Dienst. Das beweist, dass das Protokoll genau in diesem Zustand zu diesem Zeitpunkt existierte. Deine Prompts, Dateien und Pfade verlassen nie den Rechner, nur eine 32-stellige Prüfsumme.

Passwörter und API-Schlüssel werden entfernt, bevor etwas geschrieben wird.

**Wo es liegt:** im eigenen Ordner von Taibu auf deinem Computer, nicht in deinem Projekt. Teamfreigaben kommen damit nie in Berührung, und die KI kann nicht hineinschreiben.

**Wer es lesen kann:** du. Es wird nie hochgeladen, und MGR Tech Solutions bekommt es nie. Wenn du je beweisen musst, was passiert ist, legst du es vor und jeder kann es mit dem Prüfwerkzeug kontrollieren, das mit Taibu kommt.

**Was es nicht macht:** es zeichnet auf, was angefragt wurde und was getan wurde, nicht alles, was die KI zurückgesagt hat. Und nichts auf deinem eigenen Computer kann jemanden mit Administratorrechten daran hindern, den ganzen Ordner zu löschen. Die Garantie ist: Ein Protokoll, das noch da ist, wurde nicht unbemerkt verändert.

## Arbeit, die die App verwaltet

Der Ordner `.taibu/` ist die eigene Buchhaltung der App: deine Chats, die Entwürfe im Postausgang, die Berichte aus deinen Routinen und deine Team-Schlüssel und dein Sync-Status. Du musst ihn nicht öffnen, und du lässt ihn am besten in Ruhe.

## Was deinen Computer verlassen kann

| Daten | Verlässt den Computer? |
|---|---|
| `intake.md`, `context/persona.md`, `.env` | **Nie** |
| Erinnerung ohne Scope | **Nie**, und kein Scope ist der Standard |
| `company/`, `references/`, `decisions/`, Skills, Erinnerung mit Scope | Nur wenn dein Admin diesen Ordner mit einem Scope geteilt hat, in dem du bist, und nur verschlüsselt |
| Deine Arbeit, an MGR Tech Solutions | **Nie.** Keine Datei, kein Prompt und keine Antwort wird je hochgeladen |
| Dein Lizenzschlüssel, eine anonyme Maschinen-ID und deine E-Mail | Werden beim Aktivieren und bei jedem Start der App gesendet, um zu prüfen, ob die Lizenz gültig ist |
| Eine Prüfsumme des Aktivitätsprotokolls | Wird an einen unabhängigen Zeitstempel-Dienst gesendet. 32 Zeichen, kein Inhalt |
| Anfragen an deine KI-Engine | Gehen an den Anbieter, den du gewählt hast, Anthropic oder OpenAI, unter deinem eigenen Konto und deren Bedingungen |

Alles oben ist eine Klartextdatei. Du kannst sie in jedem Editor öffnen, sichern, in git legen oder löschen. Wenn du Taibu nicht mehr nutzt, bleibt dein Wissen genau dort, wo es ist.
