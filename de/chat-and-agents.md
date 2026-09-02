# Chats und Agenten

Ein **Agent** ist ein Chat-Tab für genau ein Ziel. Trenne Ziele auf mehrere Agenten auf. So bleibt jeder fokussiert.

- **+** in der Tab-Leiste startet einen neuen Agenten
- **Doppelklick oder Rechtsklick** auf einen Tab benennt ihn um
- Wenn du wegwechselst, arbeitet er weiter. Die Antwort wartet auf dich
- Wenn du einen Agenten mit echtem Inhalt schließt, landet er auf Start unter „Zuletzt geschlossen“. Dort kannst du ihn wieder öffnen

Im Bereich **Agenten** siehst du alle Agenten, die du gestartet hast, unter **Aktiv** und **Geschlossen**. Ein geöffneter Agent bietet **Schließen**. Das behält den Agenten und seinen Verlauf. Ein geschlossener Agent bietet **Öffnen** und **Löschen**.

![Vier Agenten, einer pro Ziel](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/11-agents.png)

## Der Composer

Tippe und drücke Enter. Mit Shift+Enter fügst du eine neue Zeile ein.

| Steuerung | Was es macht |
|---|---|
| **+** | Verbindet ein Tool |
| **Aktionen** | Führt einen Skill aus, in einem eigenen neuen Agenten |
| **Einstellungs-Pill** | Engine, Modell, Aufwand und Berechtigungen für diesen Agenten |
| **Büroklammer** | Hängt eine Datei als Kontext an |
| **Senden / Stoppen** | Sendet oder unterbricht, was gerade läuft |

Wenn du **/** tippst, öffnet sich die Befehlsliste: /clear, /compact, /help, /model, /status. Skills sind auch Slash-Befehle, zum Beispiel /roast.

![Das Slash-Befehlsmenü](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/12b-slash.png)

## Antworten lesen

Antworten kommen als normaler Text mit anklickbaren Links. Dabei kannst du Folgendes sehen:

- **Vorgeschlagene Route**-Karten für Pläne, mit „Route freigeben“ und „Anpassen“
- **Tool-Karten**, die zeigen, was es gemacht hat: eine Datei bearbeitet, einen Befehl ausgeführt. Dateinamen sind anklickbar
- **Bilder und Videos** direkt im Chat, Dokumente als anklickbare Chips
- Einen **„{n} Hintergrundschritte“**-Chip, der Routinearbeit einklappt. Klicke auf den Chip, um diese eine Antwort aufzuklappen. Wenn du sie immer sehen willst, aktiviere **„Technische Details im Chat anzeigen“** in den Einstellungen

![Eine Antwort mit einem Plan und Tool-Karten](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/13-answer.png)

## Berechtigungen

Du stellst sie pro Agent über die Einstellungs-Pill ein:

| Modus | Was es macht |
|---|---|
| **Vollautomatisch** | Bearbeitet Dateien und führt Befehle ohne Rückfrage aus. Das ist die Standardeinstellung |
| **Nur Dateibearbeitungen** | Ändert Dateien, führt keine Befehle aus |
| **Erst planen** | Liest und plant nur. Ändert nichts |

Eine Sicherheitsgrenze gilt in jedem Modus, auch in Vollautomatisch. Taibu weigert sich, dein Laufwerk oder Home-Verzeichnis zu löschen, `sudo` zu verwenden, den Rechner herunterzufahren, die Git-Historie mit Force-Push zu überschreiben oder Pakete zu veröffentlichen. Die KI kann diese Regeln nicht umgehen.

**Aufwand** steuert, wie intensiv sie nachdenkt: Auto, Schnell, Ausgewogen, Tief.

![Engine, Modell, Aufwand und Berechtigungen für diesen Agenten](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/14-agent-settings.png)

## Pläne

Wenn Taibu einen Plan mit mehreren Schritten vorschlägt, bekommst du eine Karte „Vorgeschlagene Route“. Mit „Route freigeben“ macht es weiter. Mit „Anpassen“ sagst du, was geändert werden soll.

Im Modus „Erst planen“ erscheint nach einem Planungsdurchgang zusätzlich die Schaltfläche „Plan ausführen“.

Wenn du einen Plan freigibst, wechselt dieser Agent für den Rest der Sitzung auf Vollautomatisch. Jede Nachricht, die du tippst, während ein Plan noch offen ist, zählt auch als Freigabe. Wähle wieder „Erst planen“, um zum Planen zurückzugehen.

## Stoppen

**Stoppen** unterbricht den Durchgang und behält alles, was schon geschrieben wurde. **/clear** löscht den Verlauf und startet neu. Deine Dateien bleiben unberührt.
