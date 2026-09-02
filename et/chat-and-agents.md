# Vestlus ja agendid

**Agent** on üks vestluse sakk ühe eesmärgi jaoks. Hoia eri eesmärgid eri agentides ja igaüks püsib oma teema juures.

- Sakaribal olev **+** käivitab uue agendi
- Tee sakil **topeltklõps või paremklõps**, et see ümber nimetada
- Võid mujale liikuda ja agent töötab edasi, vastus ootab sind
- Kui sulged päris sisuga agendi, liigub see Kodu vaatesse jaotisse "Hiljuti suletud", kust saad selle uuesti avada

Paneel **Agendid** näitab kõiki agente, mille oled käivitanud, jaotistes **Aktiivsed** ja **Suletud**. Avatud agendi juures näed valikut **Sulge**, mis jätab agendi ja selle vestluse alles. Suletud agendi juures näed valikuid **Ava** ja kustuta.

![Neli agenti, üks iga eesmärgi jaoks](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/11-agents.png)

## Sisestuskast

Kirjuta ja vajuta Enter. Shift+Enter teeb uue rea.

| Juhtelement | Mida see teeb |
|---|---|
| **+** | Ühenda tööriist |
| **Tegevused** | Käivita oskus omaette uues agendis |
| **Seadete kapsel** | Selle agendi mootor, mudel, pingutus ja õigused |
| **Kirjaklamber** | Lisa fail kontekstiks |
| **Saada / Peata** | Saada või katkesta käimasolev tegevus |

Kui kirjutad **/**, avaneb käskude menüü: /clear, /compact, /help, /model, /status. Ka oskused on kaldkriipskäsklused, näiteks /roast.

![Kaldkriipskäskluste menüü](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/12b-slash.png)

## Kuidas vastuseid lugeda

Vastused tulevad tavalise tekstina koos klõpsatavate linkidega. Vahepeal võid näha järgmist:

- **Pakutud plaan** kaardid plaanide jaoks, nuppudega "Kinnita plaan" ja "Muuda"
- **Tööriistakaardid**, mis näitavad, mida agent tegi: muutis faili, käivitas käsu. Failinimed on klõpsatavad
- **Pildid ja videod** otse vastuses, dokumendid klõpsatavate siltidena
- **"{n} taustasammu"** silt, mis peidab rutiinse töö kokku. Klõpsa silti, et avada selle vastuse sammud. Kui tahad neid alati näha, tee Seaded all linnuke **"Näita vestluses tehnilisi detaile"**

![Vastus plaani ja tööriistakaartidega](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/13-answer.png)

## Õigused

Määra need iga agendi jaoks eraldi seadete kapslis.

| Režiim | Mida see teeb |
|---|---|
| **Täisautomaatne** | Muudab faile ja käivitab käske küsimata. See on vaikimisi valik |
| **Ainult failimuudatused** | Muudab faile, käske ei käivita |
| **Kõigepealt plaan** | Ainult loeb ja teeb plaani. Midagi ei muuda |

Turvapiirang kehtib igas režiimis, ka täisautomaatses. Taibu keeldub kustutamast sinu ketast või kodukausta, kasutamast sudo-t, masinat välja lülitamast, git ajaloo peale force-push'i tegemast või pakette avaldamast. AI ei saa neid piiranguid jutuga kõrvale nihutada.

**Pingutus** määrab, kui põhjalikult see mõtleb: Auto, Fast, Balanced, Deep.

![Selle agendi mootor, mudel, pingutus ja õigused](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/14-agent-settings.png)

## Plaanid

Kui Taibu pakub mitme sammuga plaani, näed kaarti "Pakutud plaan". "Kinnita plaan" ütleb sellele, et jätka. "Muuda" lubab sul öelda, mida muuta.

Režiimis "Kõigepealt plaan" ilmub pärast planeerimisvooru ka nupp "Käivita plaan".

Plaani kinnitamine lülitab selle agendi üle täisautomaatseks ülejäänud seansi ajaks. Ka iga sinu kirjutatud sõnum ajal, kui plaan ootab kinnitust, läheb arvesse kinnitusena. Kui tahad tagasi ainult planeerimise juurde, vali uuesti "Kõigepealt plaan".

## Peatamine

**Peata** katkestab käigu ja jätab alles kõik, mis selleks hetkeks juba kirja sai. **/clear** tühjendab vestluse ja alustab puhtalt lehelt. Sinu failid jäävad puutumata.
