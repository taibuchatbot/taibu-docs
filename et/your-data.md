# Sinu andmed, mida Taibu sinu kohta kirjutab

Taibu hoiab seda, mida ta teab, tavalistes failides sinu projekti kaustas. Midagi ei ole peidetud andmebaasi ja midagi ei asu Taibu serveris. See leht on kaart, mis näitab, mida iga fail sisaldab, kuidas see täidetakse ja millised neist võivad üldse kolleegini jõuda.

Ava neist ükskõik milline vasakul olevast failipuust.

## Sina ise

| Fail | Kuidas see kirja pannakse | Mis seal sees on |
|---|---|---|
| `intake.md` | Seadistusabiline ja hiljem **Seaded → "Minu andmed ja eesmärgid"** | Sinu seitse vastust, kes sa oled ja mida sa müüd, üks või kaks näidet sinu kirjutamisest, sinu kvartali prioriteedid, kuhu tulu jõuab, kus sa inimestega suhtled, kus su dokumendid asuvad ja mis su nädala ära sööb |
| `context/persona.md` | Ainult oskus `/learn-me`, ja ainult pärast seda, kui kiidad iga muudatuse heaks | Sinu digitaalne kaksik, sinu hääl ja stiilireeglid, mida sa püüad teha ja miks, kuidas sa otsuseid teed, mis sulle meeldib ja mis sind ärritab, inimesed sinu ümber |

**Neid kumbagi ei jagata kunagi tiimiga.** Need on sünkroonimiskihis blokeeritud, seega jäävad need sinu arvutisse ka siis, kui keegi jagab kausta, kus need asuvad. Need on ka põhjus, miks Taibu kõlab nagu sina, mitte nagu üldine assistent, seega tasub neid hoida täpsena.

`persona.md` ei kirjutata kunagi sinu teadmata ümber. `/learn-me` pakub muudatusi päris tõendite põhjal, sinu tegelike mustandite ja sinu paranduste järgi, ning sina kinnitad need ükshaaval.

## Sinu ettevõte

| Fail | Mis sinna kuulub |
|---|---|
| `company/offer.md` | Mida sa müüd, sinu hinnad, mis teeb sind teistsuguseks |
| `company/icp.md` | Kellele sa müüd, mis probleem neil on, kust neid leida |
| `company/strategy.md` | Kuhu ettevõte liigub ja mis on praegu tähtis |
| `company/sops/<process>.md` | Üks fail iga korduva protsessi kohta, kuidas me teeme asja X |

Need täituvad töö käigus. Kirjelda, kuidas midagi tehakse, määra hind, kirjelda klient või sea suund paika, ning Taibu kirjutab selle õigesse faili ja ütleb ühe lausega, mida ta salvestas.

See jaotus on oluline, **`company/` on see, mida ettevõte teab, ja seda saab tiimiga jagada. `context/persona.md` ja `intake.md` on see, kes sina oled, ja neid ei saa jagada.** See ongi kogu põhjus, miks need on eri kaustades.

## Otsused, viited, ühendused

| Fail või kaust | Mis see on |
|---|---|
| `decisions/log.md` | Kuupäevaga otsused koos põhjusega iga otsuse taga. Kui sa midagi otsustad, pakub Taibu selle logisse lisamist |
| `references/` | Raamistikud, häälenäited ja juhend iga tööriista kohta, mille ühendad. `references/voice.md` on register, kuhu Taibu kirjutab |
| `connections.md` | Register kõigist süsteemidest, millest Taibu teab, olgu need ühendatud või mitte. **Tegeliku oleku nägemiseks käivita `/audit`** |
| `.env` | Sinu API võtmed. Neid ei jagata kunagi, neid ei näidata kunagi vestluses, ja need täidetakse **Seaded → "Võtmed"** kaudu, mitte käsitsi |

## Sinu juhised

`CLAUDE.md` projekti juurkaustas on püsijuhiste fail, kuidas Taibu peaks sinuga töötama, kus asjad asuvad ja milliseid reegleid ta peab järgima. See laaditakse iga vestluse alguses. `AGENTS.md` on sama fail OpenAI Codexi mootori jaoks.

Sa võid seda muuta. Kui märkad, et kordad vestluses sama juhist, pane see hoopis sinna, siis kehtib see edaspidi.

Kui töötad tiimis, ilmuvad sinu administraatori jagatud reeglid selles failis märgitud ploki sisse. Kõik väljaspool seda plokki jääb sinu omaks.

## Mälu

Kolmel mälukihil, `memory.md`, `memory/facts/` ja `memory/journal/`, on omaette leht. Vaata **Mida Taibu mäletab**.

## Töö, mida rakendus haldab

Kaust `.taibu/` on rakenduse enda arvestus, sinu vestlused, Outboxis ootavad mustandid, aruanded, mille sinu rutiinid lõid, ning sinu tiimi võtmed ja sünkroonimise olek. Sul ei ole vaja seda avada ja kõige parem on see rahule jätta.

## Mis võib sinu arvutist lahkuda

| Andmed | Kas lahkub arvutist |
|---|---|
| `intake.md`, `context/persona.md`, `.env` | **Mitte kunagi** |
| Mälu ilma ulatuseta | **Mitte kunagi**, ja ulatuseta on vaikeseade |
| `company/`, `references/`, `decisions/`, skills, scoped memory | Ainult siis, kui sinu administraator on seda kausta jaganud ulatusega, kuhu sina kuulud, ja ainult krüpteeritult |
| Ükskõik mis, Taibule | Mitte kunagi. Sinu tööd hoidvat Taibu serverit ei ole olemas |

Kõik ülaltoodu on lihttekstifail. Sa võid selle avada ükskõik millises redaktoris, teha varukoopia, panna giti, või kustutada. Kui lõpetad Taibu kasutamise, jäävad sinu teadmised täpselt sinna, kus need on.
