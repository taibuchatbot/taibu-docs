# Woran sich Taibu erinnert

Taibu merkt sich deine Arbeit über Monate. Alles sind normale Dateien in deinem Projekt. Du kannst sie lesen, bearbeiten oder löschen.

**Zahnrad-Symbol → Einstellungen → "Memory"**

![Der Speicherbereich](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/15-memory.png)

## Drei Ebenen und die Dateien dahinter

| Ebene | Speicherort | Was es ist |
|---|---|---|
| **Zusammengefasste Wahrheit** | `memory.md` | Eine kurze, gepflegte Zusammenfassung der wichtigsten Punkte über dich und deine Arbeit. Bewusst kurz gehalten, weil sie in jede einzelne Unterhaltung geladen wird |
| **Strukturierte Erinnerungen** | `memory/facts/<name>.md`, eine Datei pro Fakt | Ein dauerhafter Fakt pro Datei: eine Entscheidung, eine Korrektur, eine Vorliebe, ein Preis, ein Kunde, ein Tool, das du nutzt. Ersetzte Fakten wandern nach `memory/facts/archived/` |
| **Zeitverlauf** | `memory/journal/<year-month>.md`, plus `memory/today.md` | Ein Protokoll, das nur ergänzt wird, Monat für Monat, plus eine kurze Zusammenfassung deiner heutigen Arbeit. Nichts wird weggeworfen |

Es gibt noch eine weitere Datei: `memory/recall.mjs`, das kleine Suchprogramm, das Taibu über deine strukturierten Erinnerungen laufen lässt, wenn du nach etwas Älterem fragst.

## Wie Erinnerungen geschrieben werden

Drei Wege. Alle drei landen in denselben Dateien:

1. **Automatisch, nach jedem Austausch.** Die App schaut auf das, was gerade passiert ist, und speichert alles, was wie ein dauerhafter Fakt klingt.
2. **Durch Taibu, während du arbeitest.** Wenn du eine Entscheidung triffst, etwas korrigierst, eine Vorliebe nennst oder etwas über dein Setup erwähnst, schreibt es den Fakt sofort auf, statt auf den automatischen Durchlauf zu warten.
3. **Durch dich.** Alles im Speicherbereich ist bearbeitbar, und "Edit as text" öffnet die rohe `memory.md` zum Umschreiben.

Eine strukturierte Erinnerung ist nicht nur ein Satz. Jede hält fest, **wann sie gelernt wurde, welcher Agent sie gelernt hat, aus welcher Unterhaltung sie stammt, wer sie gesagt hat, deine genauen Worte, die Dateien, die man prüfen sollte, wie wichtig sie ist und ob sie noch aktuell ist**. Genau das macht eine Antwort Monate später prüfbar statt geraten.

## Was Taibu liest, und wann

Dieser Teil ist wichtig, weil er erklärt, warum Taibu manches sofort weiß und manches erst nachschlagen muss.

**Immer in jede Nachricht geladen:**

- `memory.md`, die zusammengefasste Wahrheit
- eine Übersicht deiner neuesten und wichtigsten strukturierten Erinnerungen
- `memory/today.md`

**Nur bei Bedarf geöffnet:** die vollständigen Fakt-Dateien, das Monatsprotokoll und alles andere in deinem Projekt. Älterer oder speziellerer Kontext wird über Recall geholt, nicht ständig mitgetragen.

Darum bleibt die zusammengefasste Wahrheit kurz. Das ist der Teil, den Taibu nie nachschlagen muss. Dort sollte stehen, was grundsätzlich über dich stimmt, nicht jedes Detail, das du je erwähnt hast.

## Recall

Frag nach etwas von vor Monaten, in den Worten, die dir gerade einfallen. Taibu durchsucht seine strukturierten Erinnerungen und antwortet **mit Belegen**: welche Datei, welches Datum, wer es gesagt hat und die genauen Worte, die du benutzt hast.

Wenn es nichts findet, sagt es dir das, statt zu raten. Du kannst auf dieselbe Weise auch selbst suchen, oben im Feld im Speicherbereich.

Recall liest die Fakt-Dateien. Wenn dein Wissen nur in `memory.md` gelandet ist, kann es dort nichts durchsuchen, und Taibu sagt dir das.

## Deinen Verlauf importieren

Beim ersten Mal drückst du **"Import past conversations"**. Taibu wandelt deinen vorhandenen Chatverlauf in durchsuchbare Erinnerungen um. So startest du mit allem, was du ihm schon gesagt hast.

## Ordnung halten

Füge die Routine **"Memory tidy-up"** hinzu, und Taibu konsolidiert jede Woche: doppelte Einträge zusammenführen, veraltete Fakten archivieren, wiederkehrende Themen in die zusammengefasste Wahrheit übernehmen. Wichtige und bestätigte Fakten werden nie automatisch entfernt.

## Datenschutz

Memory ist lokal. Es sind normale Dateien in deinem Projektordner. Nichts geht an einen Taibu-Server.

Eine Erinnerung **ohne Geltungsbereich ist privat** und verlässt nie deinen Computer. Das ist der Standard. Nur Erinnerungen mit ausdrücklich gesetztem Team-Geltungsbereich werden überhaupt geteilt, und selbst dann werden sie verschlüsselt, bevor sie deinen Computer verlassen. Unter **Im Team arbeiten** steht, wie Geltungsbereiche funktionieren.

Zwei Dateien werden nie mit einem Team geteilt, egal wie das Teilen eingestellt ist: deine Antworten beim Onboarding (`intake.md`) und dein persönliches Profil (`context/persona.md`). Unter **Deine Daten** steht der Rest von dem, was Taibu über dich schreibt.
