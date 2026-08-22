# Sinu andmed, mida Taibu sinu kohta kirjutab

Taibu hoiab seda, mida ta teab, tavalistes failides sinu projekti kaustas. Midagi ei ole peidetud andmebaasi ja midagi ei ole Taibu serveris. See leht on kaart, mis näitab, mida iga fail sisaldab, kuidas see kirjutatakse ja millised failid võivad üldse kolleegini jõuda.

Ava vasakul failipuust ükskõik milline neist.

## Sina ise

| File | How it gets written | What is in it |
|---|---|---|
| `intake.md` | Seadistusviisard ja hiljem **Seaded → "Minu andmed ja eesmärgid"** | Sinu seitse vastust: kes sa oled ja mida sa müüd, üks või kaks näidet sinu kirjutamisest, sinu kvartali prioriteedid, kuhu tulu jõuab, kus sa inimestega suhtled, kus su dokumendid asuvad ja mis su nädala ära sööb |
| `context/persona.md` | Ainult oskus `/learn-me`, ja ainult pärast seda, kui oled iga muudatuse heaks kiitnud | Sinu digitaalne kaksik: sinu hääl ja stiilireeglid, mida sa püüad teha ja miks, kuidas sa otsustad, mis sulle meeldib ja mis sind ärritab, sind ümbritsevad inimesed |

**Neid kumbagi ei jagata kunagi tiimiga.** Need on sünkroonimiskihis blokeeritud, seega jäävad need sinu arvutisse ka siis, kui keegi jagab kausta, kus need asuvad. Need on ka põhjus, miks Taibu kõlab nagu sina, mitte nagu tavaline assistent, seega tasub neid hoida täpsena.

`persona.md` ei kirjutata kunagi sinu selja taga ümber. `/learn-me` pakub muudatusi päris tõendite põhjal, sinu tegelike mustandite ja paranduste põhjal, ning sina kinnitad need ükshaaval.

## Sinu ettevõte

| File | What belongs in it |
|---|---|
| `company/offer.md` | Mida sa müüd, sinu hinnad, mis teeb sind erinevaks |
| `company/icp.md` | Kellele sa müüd, mis probleem neil on, kust neid leida |
| `company/strategy.md` | Kuhu äri liigub ja mis on praegu tähtis |
| `company/sops/<process>.md` | Üks fail iga korduva protsessi kohta: kuidas me teeme X |

Need täituvad töö käigus. Kui kirjeldad, kuidas midagi tehakse, määrad hinna, defineerid kliendi või paned paika suuna, kirjutab Taibu selle õigesse faili ja ütleb sulle ühe lausega, mida ta salvestas.

See jaotus on oluline: **`company/` on see, mida ettevõte teab, ja seda saab tiimiga jagada. `context/persona.md` ja `intake.md` on see, kes sina oled, ja neid ei saa jagada.** See ongi kogu põhjus, miks need on eraldi kaustades.

## Otsused, viited, ühendused

| File or folder | What it is |
|---|---|
| `decisions/log.md` | Kuupäevaga otsused koos põhjusega iga otsuse taga. Kui sa midagi otsustad, pakub Taibu selle logisse lisamist |
| `references/` | Raamistikud, häälenäited ja juhend iga tööriista kohta, mille ühendad. `references/voice.md` on register, kuhu Taibu kirjutab |
| `connections.md` | Register kõigi süsteemide kohta, millest Taibu teab, olenemata sellest, kas need on ühendatud või mitte. **Käivita `/audit`, et näha tegelikku olekut** |
| `.env` | Sinu API võtmed. Neid ei jagata kunagi, neid ei näidata vestluses ja need täidetakse käsitsi kirjutamise asemel kaudu **Seaded → "Võtmed"** |

## Sinu juhised

`CLAUDE.md` projekti juurkaustas on püsijuhiste fail, kuidas Taibu peaks sinuga töötama, kus asjad asuvad ja milliseid reegleid ta peab järgima. See laaditakse iga vestluse alguses. `AGENTS.md` on sama asi OpenAI Codexi mootori jaoks.

Sa saad seda muuta. Kui avastad, et kordad vestluses sama juhist, pane see sinna ja siis kehtib see edaspidi.

Kui töötad tiimis, ilmuvad sinu administraatori jagatud reeglid sellesse faili märgitud ploki sisse. Kõik väljaspool seda plokki jääb sinu omaks.

## Mälu

Kolmel mälukihil, `memory.md`, `memory/facts/` ja `memory/journal/`, on oma eraldi leht. Vaata **Mida Taibu mäletab**.

## Tegevuslogi

Taibu peab arvestust selle üle, mis rakenduses toimub: mida sa palusid, iga tööriist, mida agent käivitas ja millega, ning failid, mida rakendus kirjutas, ümber nimetas või kustutas. See on olemas selleks, et kui keegi kunagi küsib, mis juhtus, oleks olemas sirge vastus, mitte mälestus.

Kolm asja teevad selle väärtuslikuks:

* **See on alati sees.** Sina ei saa seda välja lülitada ja Taibu ka mitte. Kirje, mida saab enne millegi tegemist välja lülitada, ei ole päris kirje.
* **Seda ei saa muuta.** Iga kirje on seotud eelmisega, seega iga kirje muutmine või eemaldamine rikub kõik selle järel. **Seaded → Activity log** näitab, kas see on terve, ja nimetab esimese vigase kirje, kui midagi on puututud.
* **Seda kinnitab sõltumatu osapool.** Aeg ajalt saadab Taibu logi kontrollsumma, ja mitte midagi muud, sõltumatule ajatembeldamise teenusele. See tõestab, et logi eksisteeris täpselt sellises olekus just sel ajal. Sinu päringud, failid ja teed ei lahku kunagi masinast, ainult 32 märgiga kontrollsumma.

Paroolid ja API võtmed eemaldatakse enne, kui midagi kirja pannakse.

**Kus see asub:** Taibu enda kaustas sinu arvutis, mitte sinu projektis, seega tiimiga jagamine ei puuduta seda kunagi ja tehisaru ei saa sinna kirjutada.

**Kes saab seda lugeda:** sina. Seda ei laadita kunagi üles ja MGR Tech Solutions ei saa seda kunagi kätte. Kui sul on kunagi vaja tõestada, mis juhtus, näitad selle ette sina ja igaüks saab seda kontrollida Taibuga kaasas oleva kontrollijaga.

**Mida see ei tee:** see salvestab, mida küsiti ja mida tehti, mitte kõike seda, mida tehisaru vastu ütles. Ja miski sinu enda arvutis ei saa takistada administraatori õigustega inimest kogu kausta kustutamast. See tagab, et kirjet, mis on alles, ei ole vaikselt muudetud.

## Töö, mida rakendus haldab

Kaust `.taibu/` on rakenduse enda arvestus: sinu vestlused, mustandid, mis ootavad väljundkaustas, aruanded, mille sinu rutiinid lõid, ning sinu tiimi võtmed ja sünkroonimise olek. Sul ei ole vaja seda avada ja kõige parem on see rahule jätta.

## Mis võib sinu arvutist lahkuda

| Data | Leaves? |
|---|---|
| `intake.md`, `context/persona.md`, `.env` | **Mitte kunagi** |
| Mälu ilma ulatuseta | **Mitte kunagi**, ja ulatuseta on vaikimisi |
| `company/`, `references/`, `decisions/`, oskused, ulatusega mälu | Ainult siis, kui sinu administraator on selle kausta jaganud ulatusega, kuhu sina kuulud, ja ainult krüpteeritult |
| Sinu töö, MGR Tech Solutionsile | **Mitte kunagi.** Ühtegi faili, päringut ega vastust ei laadita kunagi üles |
| Sinu litsentsivõti, anonüümne masina ID ja sinu e post | Saadetakse aktiveerimisel ja iga kord, kui rakendus käivitub, et kontrollida litsentsi kehtivust |
| Tegevuslogi kontrollsumma | Saadetakse sõltumatule ajatembeldamise teenusele. 32 märki, ilma sisuta |
| Päringud sinu tehisaru mootorile | Need lähevad sellele teenusepakkujale, kelle sa valisid, Anthropicule või OpenAIle, sinu enda konto ja nende tingimuste alusel |

Kõik ülaltoodu on lihttekstifail. Sa saad selle avada suvalises redaktoris, teha varukoopia, panna giti või kustutada. Kui lõpetad Taibu kasutamise, jäävad sinu teadmised täpselt sinna, kus need on.
