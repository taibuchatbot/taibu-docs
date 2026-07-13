# AI-mootorid

Taibu AI OS töötab kolme erineva AI-mootoriga. Vali oma **Seaded → AI-mootor** alt. Projektid, failid ja oskused jäävad samaks — vahetub ainult AI, kes töö ära teeb.

## Kolm mootorit

| | Claude Code | OpenAI Codex | Lokaalmudel (Ollama) |
|---|---|---|---|
| **Vajad** | Claude'i tellimust (Pro/Max) | ChatGPT tellimust (Plus/Pro/Team) | Korralikku arvutit, muud ei midagi |
| **Hind** | Su olemasolev tellimus | Su olemasolev tellimus | Tasuta — jookseb su masinas |
| **Internet** | Vajalik | Vajalik | **Pole vaja** — täielikult offline |
| **Kvaliteet** | Parim — täiskogemus | Väga hea | Sõltub mudelist ja riistvarast — keerukatel mitmesammulistel töödel märgatavalt nõrgem |
| **Oskused (/onboard, /audit…)** | Natiivne | Töötab AGENTS.md silla kaudu | Töötab AGENTS.md silla kaudu, vähem kindlalt |

**Meie soovitus:** Claude Code täiskogemuseks. Codex, kui maksad juba ChatGPT eest ja mitte Claude'i eest. Lokaalmudelid siis, kui privaatsus või offline-töö on olulisem kui lihv.

## Claude Code (vaikimisi)

1. Paigalda: `winget install Anthropic.Claude` (app pakub seda ka esmakäivitusel)
2. Logi sisse oma Claude'i tellimusega — app juhendab.

## OpenAI Codex

1. Paigalda: `npm install -g @openai/codex`
2. Seaded → AI-mootor → **OpenAI Codex** — app avab `codex login`; logi brauseris sisse oma ChatGPT kontoga.
3. Ongi kõik. Projekti juhised toimivad automaatselt (tööruumis on `AGENTS.md`, mida Codex loeb).

## Lokaalmudel (Ollama)

Jookseb täielikult sinu masinas — midagi ei lahku su arvutist. Hea tundlike andmete ja offline-töö jaoks.

1. Paigalda [Ollama](https://ollama.com) ja tõmba kodeerimismudel, nt: `ollama pull gpt-oss:20b`
2. Paigalda Codex CLI (see juhib lokaalmudelit): `npm install -g @openai/codex`
3. Seaded → AI-mootor → **Lokaalmudel (Ollama)**. Mudelivalik näitab kõiki Ollama mudeleid.

**Ausad ootused:** lokaalne 20B mudel ei ole Claude. Lihtsad tööd (mustandid, kokkuvõtted, failimuudatused) toimivad hästi. Pikad mitmesammulised automatiseeringud ja juhendatud oskused vajavad rohkem kättpidi juhtimist. Proovi oma päris töövoogu enne, kui selle peale lood.

## Mootori vahetamine

Vahetus on hetkeline ja ohutu — vahetub AI, mitte su andmed. Iga vestlussessioon kuulub ühele mootorile; pärast vahetust alusta uue sõnumiga ja uus mootor võtab projekti üles failidest (CLAUDE.md / AGENTS.md, memory.md, context/).
