# KI-Engines

Taibu AI OS kann mit drei verschiedenen KI-Engines laufen. Wähle deine in **Einstellungen → AI Engine**. Deine Projekte, Dateien und Skills bleiben gleich. Nur die KI, die die Arbeit macht, wechselt.

## Die drei Engines

| | Claude Code | OpenAI Codex | Lokales Modell (Ollama) |
|---|---|---|---|
| **Du brauchst** | Claude-Abo (Pro/Max) | ChatGPT-Abo (Plus/Pro/Team) | Einen ordentlichen Computer, sonst nichts |
| **Kosten** | Dein bestehendes Abo | Dein bestehendes Abo | Kostenlos. Läuft auf deinem Rechner |
| **Internet** | Erforderlich | Erforderlich | **Nicht erforderlich**. Vollständig offline |
| **Qualität** | Am besten. Volles Erlebnis | Sehr gut | Hängt vom Modell und deiner Hardware ab. Bei komplexer Arbeit mit mehreren Schritten merklich schwächer |
| **Skills (/onboard, /audit…)** | Nativ | Ja. Taibu kopiert sie dorthin, wo Codex sucht | Ja, aber beachte die Warnung unten |
| **Routinen** | Ja | Ja | Nicht empfohlen |
| **Tools verbinden (MCP)** | Ja | Ja, eigenes Registry | Ja, wie bei Codex |
| **Gmail / Drive / Calendar** | Ja | **Nein**. Das sind Claude-Konto-Connectoren | **Nein** |

**Unsere Empfehlung:** Claude Code für das volle Erlebnis. Codex, wenn du schon für ChatGPT zahlst und nicht für Claude. Lokale Modelle, wenn Datenschutz oder Offline-Arbeit wichtiger sind als Feinschliff.

## Claude Code (Standard)

1. Installieren: `winget install Anthropic.Claude` (die App bietet das auch beim ersten Start an)
2. Melde dich mit deinem Claude-Abo an. Die App führt dich durch den Prozess.

## OpenAI Codex

1. Installieren: `npm install -g @openai/codex`
2. Einstellungen → AI Engine → **OpenAI Codex**. Die App öffnet `codex login`. Melde dich im Browser mit deinem ChatGPT-Konto an.
3. Das war's. Deine Projektanweisungen funktionieren automatisch. Der Workspace enthält ein `AGENTS.md`, das Codex liest.

## Lokales Modell (Ollama)

Läuft komplett auf deinem Rechner. Nichts verlässt deinen Computer. Gut für sensible Daten und Offline-Arbeit.

1. Installiere [Ollama](https://ollama.com) und lade ein Coding-Modell, zum Beispiel: `ollama pull gpt-oss:20b`
2. Installiere die Codex CLI, sie steuert das lokale Modell: `npm install -g @openai/codex`
3. Einstellungen → AI Engine → **Lokales Modell (Ollama)**. Die Modellauswahl zeigt alle Modelle an, die Ollama hat.

**Ehrliche Erwartungen:** Ein lokales Modell ist nicht Claude, und der Abstand ist größer, als es aussieht. Taibu gibt einem lokalen Modell dieselben Anweisungen, denselben Speicher und dieselben Skills wie jeder anderen Engine. Die Anbindung ist also nicht das Limit, sondern das Modell. Ein kleines Modell, etwa 4B, denkt lange nach und schafft es dann nicht, überhaupt ein Tool aufzurufen. Das heißt, es kann keine Dateien bearbeiten, keine Befehle ausführen und kein verbundenes Tool nutzen. Nimm 20B oder größer, wenn es wirklich Arbeit erledigen soll und nicht nur Text schreiben. Teste deinen echten Ablauf, bevor du dich festlegst.

Geplante Routinen mit einem lokalen Modell sind aus demselben Grund nicht empfohlen. Ein unbeaufsichtigter Lauf, der keine Tools nutzen kann, liefert nichts Brauchbares.

## Was sich beim Wechsel ändert

Taibu hält das Erlebnis auf jeder Engine gleich und übernimmt die Übersetzung für dich:

- **Deine Anweisungen** gehen direkt an Claude und an die anderen über `AGENTS.md`, das sie automatisch lesen.
- **Deine Skills** werden in den Ordner kopiert, den jede Engine nutzt. Claude liest `.claude/skills`, Codex und lokale Modelle lesen `.agents/skills`. Du musst nicht daran denken.
- **Slash-Befehle** wie `/onboard` funktionieren überall. Nur Claude erkennt sie selbst. Bei anderen Engines erweitert Taibu den Befehl vor dem Senden.
- **Routinen** laufen auf der Engine, die du gewählt hast. Die Seite Routinen zeigt dir welche und warnt dich, wenn sie nicht bereit ist.
- **Verbundene Tools** gelten pro Engine. Claude und Codex führen jeweils ihre eigene Liste. Ein Tool, das du bei der einen Engine verbunden hast, ist bei der anderen nicht automatisch da.

Zwei Dinge bleiben ehrlich gesagt nur bei Claude: **Gmail, Google Drive und Google Calendar**, weil das Connectoren in deinem Anthropic-Konto sind und nichts, was Taibu installiert, und die **untere Berechtigungsgrenze**, die gefährliche Befehle in jedem Modus blockiert. Bei anderen Engines läuft geplante Arbeit stattdessen in einer Sandbox, die sie in deinem Projekt hält.

## Engines wechseln

Der Wechsel ist sofort und sicher. Er ändert nur, welche KI antwortet, nicht deine Daten. Jede Chat-Sitzung gehört zu einer Engine. Nach dem Wechsel startest du eine neue Nachricht, und die neue Engine übernimmt das Projekt aus seinen Dateien (CLAUDE.md / AGENTS.md, memory.md, context/).
