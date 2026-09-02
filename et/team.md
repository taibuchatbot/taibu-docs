# Tiimina töötamine

**Inimeste ikoon → "Tiim"**

Tiimis jagamine laseb grupil töötada sama ettevõtte teadmise pealt. Kõik jagatu on **krüpteeritud sinu enda arvutis** enne, kui see kuhugi liigub, ja see sünkroonib läbi taristu, **mida sina omad**. Mitte miski ei liigu läbi Taibu serveri.

## Kuidas see töötab

Tiimi juht loob **skoobid** ehk sihtrühmad, näiteks müük, turundus või üks iga kliendi jaoks, otsustab, kes millisesse kuulub, ja valib, mida jagada. Kui tiimikaaslasel ei ole skoobi võtit, siis ta päriselt ei saa selle skoobi sisu lugeda, isegi kui ta näeb sünkroonimiskausta.

![Skoobid, ligipääsumaatriks ja jagatud kausta lülitid](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/23-team-admin.png)

## Kuhu see sünkroonib

| Valik | Sobib hästi |
|---|---|
| **Jagatud kaust** | Kõige lihtsam ja kiirem. Suuna see kausta, mida hoiab sünkroonis Syncthing, NAS või pilveketas |
| **Git-hoidla** | Sinu enda privaatne hoidla koos täieliku ajalooga. Kõik peavad enne giti sisse logima |

Git-hoidla puhul peab igal inimesel olema oma masinas git sisse logitud, enne kui see töötab. Käivita `gh auth login` või klooni hoidla üks kord käsitsi, et sisselogimine jääks meelde. Taibu ei salvesta sinu tokenit, seega kasutab ta sinu süsteemi git-sisselogimist. Kui see puudub, ütleb Tiimi leht seda sulle.

## Seadistamine juhina

1. Vajuta **"Loo tiim"**, pane nimi ja vali kaust või git
2. Lisa **skoob**, näiteks `company`
3. Lülita sisse see, mida tahad jagada
4. Kopeeri **tiimikood** ja saada see kolleegidele

## Liitumine liikmena

1. Kleebi tiimikood jaotisesse **"Liitu tiimiga"**
2. Vajuta **"Sünkrooni kohe"**. Näed teadet "Ootan administraatori kinnitust"
3. Tiimi juht kinnitab sind ühe vajutusega ja sinu ligipääs jõuab kohale järgmise sünkroonimisega

![Mida liige näeb kinnituse ootel](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/24-team-pending.png)

Sina saadad koodi ainult ühe korra.

## Mida saad jagada

Ettevõtte käsiraamat, ettevõtte reeglid, mälu, ettevõtte kontekst, oskused, viited, otsused, tööriistad ja ükskõik milline kaust, mille valid.

Kui lülitad kausta välja, siis jagamine peatub sellest hetkest alates. See ei kustuta midagi: kõigile jääb alles koopia, mis neil juba on, ja sinu enda failid jäävad täpselt sinna, kus nad on.

## Ühes suunas või mõlemas

Igal üksusel on seadistus **"Kes võib seda muuta"**:

- **Ainult mina**. Juhi koopia on tõde. Liikmed loevad seda, nende muudatused edasi ei levi. Kasuta seda ettevõtte põhiteadmiseks
- **Igaüks skoobis**. Kahesuunaline. Kõik panustavad ja kõik saavad. Kasuta seda jagatud mälu jaoks

Kui muudatused lähevad konflikti, jätab süsteem alles uuema versiooni ja salvestab teise selle kõrvale, nii et midagi ei lähe kaotsi.

## Ettevõtte reeglid ilma kellegi oma üle kirjutamata

Sinu juhiste fail segab ettevõtte põhimõtteid isiklike asjadega, nagu sinu nimi, keel ja prioriteedid, seega Taibu ei sünkrooni seda faili kunagi.

Selle asemel kirjutab juht ettevõtte reeglid ühte kohta ja iga liikme Taibu lisab need tema enda juhistesse eraldi märgitud plokina. Isiklikud seaded jäävad puutumata. Muudad reeglit ja kõik saavad selle kätte.

## Mida ei jagata kunagi

**Sinu isiklik profiil ja sinu hääl ei lahku kunagi sinu arvutist**, ükskõik mida seaded ütlevad. Igaüks hoiab alles oma kirjutamisviisi. Mälu ilma skoobita on privaatne ja see on vaikimisi nii.

## Tiimi ülevaated

Juht saab tegevusaruanded sisse lülitada. Iga liige otsustab ise, kas osaleda, ja näeb täpselt, mida saadetaks.

**Saadetakse:** mitu vestlust ja milliste agentidega, kuidas mälu kasvas, teemade ja oskuste nimed, tegevus päevade kaupa ja kohad, kus töö paistab takerduvat.

**Mitte kunagi ei saadeta:** mida sina kirjutasid või millele AI vastas, sinu mustandid, sinu privaatne mälu, sinu võtmed, mitte midagi isiklikku.

![Nõusolekukaart, mida liige näeb](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/25-team-consent.png)

Midagi ei saadeta enne, kui oled nõus, ja sa saad selle igal ajal peatada.

## Piirangud, mida tasub teada

- Kellegi eemaldamine vaatab ettepoole. Tema võtmed vahetatakse välja, nii et ta ei saa enam midagi uut, aga juba sünkroonitud koopiad jäävad tema masinasse alles
- Tiimi põhivõti on juhi seadmes. Varunda seda nagu parooli
- Jagamine on teadmise jaoks, mitte meedia jaoks. Igal skoobil on suuruspiirang
- Tiimi liikmesus käib projekti kaupa. Kui ühendad ühe projekti, siis teised jäävad puutumata
