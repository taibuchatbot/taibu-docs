# Einstellungen und Engines

**Zahnrad-Symbol → "Einstellungen"**, mit den Tabs Allgemein, Meine Daten und Ziele, Schlüssel und Woran sich Taibu erinnert.

**Meine Daten und Ziele** ist dein Profil: wer du bist, was du verkaufst, deine Prioritäten für das Quartal, deine Schreibbeispiele. Früher lag es hinter einem eigenen Symbol in der linken Leiste. Wenn du speicherst, übergibt Taibu das an die KI. Sie liest alles neu und baut deine Kontextdateien neu auf.

![Einstellungen, der Tab Allgemein](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/26-settings.png)

| Einstellung | Was es macht |
|---|---|
| **Beim Start öffnen** | Öffnet Start oder Chats |
| **Technische Details im Chat anzeigen** | Zeigt die Befehle und Dateizugriffe, die die KI ausführt |
| **KI-Modell / Freigabemodus / Aufwand** | Einstellungen für den aktuellen Agenten |
| **SPRACHE** | App-Sprache und die Sprache neuer Projekte. Startet die App neu |
| **KI-ENGINE** | Claude Code, OpenAI Codex oder ein lokales Modell |
| **CLAUDE-STATUS** | Ob es installiert ist und du angemeldet bist |
| **GITHUB** | Verbindet GitHub, damit Taibu mit deinen Repositories arbeiten kann |
| **LIZENZ** | Dein Plan, die Anzahl erlaubter Computer und die Projektanzahl |
| **VERSION** | Welche Build du nutzt |

Den Theme-Schalter findest du nicht in den Einstellungen. Er ist oben rechts, neben den Fensterknöpfen.

Die Erweitert-Steuerungen ändern den **aktuellen Agenten**. Das sind dieselben Werte wie in der Einstellungs-Pille des Composers. Sie sind keine globalen Standardwerte.

## Engines

| Engine | Braucht | Hinweise |
|---|---|---|
| **Claude Code** | Claude Pro, Max oder Team, oder Anthropic API billing | Das volle Erlebnis |
| **OpenAI Codex** | ChatGPT Plus, Pro oder Team, plus die Codex CLI | Funktioniert, mit etwas weniger interaktiven Details |
| **Lokales Modell (Ollama)** | Laufendes Ollama mit einem geladenen Modell, plus die Codex CLI | Vollständig offline und privat. Langsamer und schwächer bei Arbeit in mehreren Schritten |

Wenn du die Engine eines Agenten wechselst, startet ein neues Gespräch. Sitzungen lassen sich nicht zwischen Engines verschieben. Deine Dateien und Erinnerungen bleiben unverändert.

Routinen laufen immer auf Claude, egal welche Engine du für Chats gewählt hast.

**Modelle:** Sonnet ist ausgewogen und der Standard, Opus für die schwersten Aufgaben, Haiku am schnellsten für einfache Aufgaben.

## Updates

Skills, Anweisungen und Vorlagen aktualisieren sich leise und sicher selbst. Alles ist signiert, und alles, was du selbst bearbeitet hast, wird nie überschrieben.

Die App selbst aktualisiert sich nicht automatisch. Wenn es eine neue Version gibt, zeigt ein lila Balken oben auf Start: "Version X ist da", mit einem Download-Button. In den Einstellungen siehst du dasselbe neben deiner Versionsnummer. Beides lädt den Installer für dich herunter.
