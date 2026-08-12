# AI mootorid

Taibu AI OS saab töötada kolme eri AI mootoriga. Vali sobiv mootor menüüst **Seaded → AI Engine**. Sinu projektid, failid ja oskused jäävad samaks, muutub ainult töö tegev AI.

## Kolm mootorit

| | Claude Code | OpenAI Codex | Local model (Ollama) |
|---|---|---|---|
| **Sul on vaja** | Claude tellimust, Pro või Max | ChatGPT tellimust, Plus, Pro või Team | Korralikku arvutit, muud mitte |
| **Maksumus** | Sinu olemasolev tellimus | Sinu olemasolev tellimus | Tasuta, töötab sinu arvutis |
| **Internet** | Vajalik | Vajalik | **Pole vajalik**, töötab täielikult võrguühenduseta |
| **Kvaliteet** | Parim, täisfunktsionaalne kasutus | Väga hea | Sõltub mudelist ja sinu riistvarast, keeruka mitme sammuga töö puhul on tuntavalt nõrgem |
| **Oskused (/onboard, /audit…)** | Algupärane tugi | Jah, Taibu kopeerib need kohta, kust Codex neid otsib | Jah, aga vaata allolevat hoiatust |
| **Rutiinid** | Jah | Jah | Ei ole soovitatav |
| **Tööriistade ühendamine (MCP)** | Jah | Jah, oma registriga | Jah, sama nagu Codexil |
| **Gmail / Drive / Calendar** | Jah | **Ei**, need on Claude konto ühendused | **Ei** |

**Soovitus:** kasuta täielikuks kasutuseks Claude Code'i. Vali Codex, kui maksad juba ChatGPT eest, aga mitte Claude'i eest. Kohalik mudel sobib siis, kui privaatsus või võrguühenduseta töö on tähtsam kui viimistletud tulemus.

## Claude Code, vaikimisi

1. Paigalda: `winget install Anthropic.Claude` , rakendus pakub seda ka esimesel käivitamisel
2. Logi sisse oma Claude tellimusega, rakendus juhendab sind.

## OpenAI Codex

1. Paigalda: `npm install -g @openai/codex`
2. Seaded → AI Engine → **OpenAI Codex** , rakendus avab `codex login`, logi brauseris sisse oma ChatGPT kontoga.
3. Valmis. Sinu projektijuhised toimivad automaatselt, tööruum sisaldab faili `AGENTS.md`, mida Codex loeb.

## Local model (Ollama)

Töötab täielikult sinu arvutis, sinu arvutist ei lahku midagi. Sobib tundlike andmete ja võrguühenduseta töö jaoks.

1. Paigalda [Ollama](https://ollama.com) ja tõmba koodimudel, näiteks: `ollama pull gpt-oss:20b`
2. Paigalda Codex CLI, see juhib kohalikku mudelit: `npm install -g @openai/codex`
3. Seaded → AI Engine → **Local model (Ollama)**. Mudelivalija näitab kõiki mudeleid, mis Ollamal olemas on.

**Aus ootus:** kohalik mudel ei ole Claude ja vahe on suurem, kui esmapilgul paistab. Taibu annab kohalikule mudelile samad juhised, mälu ja oskused nagu igale teisele mootorile, seega piirang ei ole ühendustes, vaid mudelis endas. Väike mudel, umbes 4B, võib pikalt arutleda ja siis jätta tööriista üldse kasutamata, see tähendab, et ta ei saa muuta faile, käivitada käske ega kasutada ühendatud tööriista. Kasuta 20B või suuremat mudelit, kui tahad, et see päriselt tööd teeks, mitte ainult teksti kirjutaks, ja proovi enne päris töövoogu, kui sellele lõplikult kindlaks jääd.

Ajastatud rutiinid kohaliku mudeliga ei ole samal põhjusel soovitatavad. Järelevalveta töö, mis ei suuda tööriistu kasutada, ei anna midagi kasulikku.

## Mis muutub, kui mootorit vahetad

Taibu hoiab kasutuskogemuse kõigi mootorite puhul võimalikult samana ja teeb vajalikud teisendused sinu eest:

- **Sinu juhised** lähevad Claude'ile otse ja teistele faili `AGENTS.md` kaudu, mida need automaatselt loevad.
- **Sinu oskused** kopeeritakse kausta, kust iga mootor neid otsib. Claude loeb kausta `.claude/skills`, Codex ja kohalikud mudelid loevad kausta `.agents/skills`. Sina ei pea selle peale mõtlema.
- **Kaldkriipskäsud** nagu `/onboard` töötavad kõikjal. Ainult Claude tunneb need ise ära, teistel mootoritel avab Taibu käsu enne saatmist lahti.
- **Rutiinid** töötavad sinu valitud mootoriga. Rutiinide leht näitab, milline mootor on kasutusel, ja hoiatab, kui see pole valmis.
- **Ühendatud tööriistad** on mootoripõhised. Claude ja Codex hoiavad kumbki oma loendit, seega ühes ühendatud tööriist ei ole teises automaatselt olemas.

Kaks asja jäävad ausalt ainult Claude'ile: **Gmail, Google Drive ja Google Calendar**, sest need on sinu Anthropicu konto ühendused, mitte midagi, mida Taibu ise paigaldab, ja **lubade alampiir**, mis blokeerib ohtlikud käsud igas režiimis. Teiste mootorite puhul töötab ajastatud töö liivakastis, mis hoiab selle sinu projekti piires.

## Mootorite vahetamine

Mootori vahetamine on kohe toimiv ja turvaline, see muudab ainult seda, milline AI vastab, mitte sinu andmeid. Iga vestlusseanss kuulub ühele mootorile. Pärast vahetamist alusta uut sõnumit ja uus mootor võtab projekti üle selle failidest, `CLAUDE.md` / `AGENTS.md`, `memory.md`, `context/`.
