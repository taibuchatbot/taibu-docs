# Seaded ja mootorid

**Hammasratta ikoon → "Seaded"**, seal on vahekaardid Üldine, Minu andmed ja eesmärgid, Võtmed ja Mälu.

**Minu andmed ja eesmärgid** on koht, kus on sinu profiil: kes sa oled, mida sa müüd, mis on su kvartali prioriteedid, sinu kirjutamisnäited. Varem oli see vasakul ribal omaette ikooni taga. Kui salvestad, annab süsteem selle AI-le üle. AI loeb selle uuesti läbi ja ehitab su kontekstifailid uuesti üles.

![Seaded, vahekaart Üldine](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/26-settings.png)

| Seade | Mida see teeb |
|---|---|
| **Ava käivitamisel** | Avab Kodu või Vestlused |
| **Näita vestluses tehnilisi detaile** | Näitab käske ja faililugemisi, mida AI käivitab |
| **AI mudel / Loarežiim / Pingutus** | Praeguse agendi seaded |
| **KEEL** | Äpi keel ja uute projektide keel. Taaskäivitab äpi |
| **AI MOOTOR** | Claude Code, OpenAI Codex või kohalik mudel |
| **CLAUDE'I OLEK** | Kas see on paigaldatud ja sisse logitud |
| **GITHUB** | Ühenda GitHub, et Taibu saaks su hoidlatega töötada |
| **LITSENTS** | Sinu pakett, arvutite limiit ja projektide arv |
| **VERSIOON** | Millist versiooni sa kasutad |

Teema lüliti ei ole Seadetes. See on üleval paremas nurgas, akna nuppude kõrval.

Edasijõudnute seaded muudavad **praegust agenti**, samu väärtusi, mis on koostaja seadete kapslis. Need ei ole globaalsed vaikeseaded.

## Mootorid

| Mootor | Vajab | Märkused |
|---|---|---|
| **Claude Code** | Claude Pro, Max või Team, või Anthropic API arveldus | Täielik kasutuskogemus |
| **OpenAI Codex** | ChatGPT Plus, Pro või Team, lisaks Codex CLI | Töötab, aga interaktiivseid nüansse on veidi vähem |
| **Kohalik mudel (Ollama)** | Töötav Ollama koos allalaaditud mudeliga, lisaks Codex CLI | Täielikult võrguvaba ja privaatne. Aeglasem ja nõrgem mitme sammuga töö puhul |

Kui vahetad agendi mootorit, algab uus vestlus, sest seansse ei saa mootorite vahel liigutada. Sinu failid ja mälu jäävad samaks.

Rutiinid töötavad alati Claude'i peal, ükskõik millise mootori sa vestluste jaoks valisid.

**Mudelid:** Sonnet on tasakaalus ja vaikimisi valik, Opus kõige raskema töö jaoks, Haiku kõige kiirem lihtsate ülesannete jaoks.

## Uuendused

Oskused, juhised ja mallid uuendavad end ise vaikselt ja turvaliselt. Kõik on allkirjastatud ja midagi, mida sa ise muutsid, ei kirjutata kunagi üle.

Äpp ise ei uuenda ennast automaatselt. Kui uus versioon on olemas, näitab Kodu ülaservas lilla riba teksti "Versioon X on väljas" koos nupuga Laadi alla. Seaded näitavad sama su versiooninumbri kõrval. Mõlemast kohast saad paigaldaja alla laadida.
