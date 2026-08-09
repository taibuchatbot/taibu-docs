# Tiimiga jagamine

Taibu oskab jagada teadmisi üle tiimi: mälu, oskused, references, otsused, brändi kontekst. Lokaalsuse lubadus jääb kehtima: kõik krüpteeritakse **otsast otsani sinu arvutis** ja sünkroonitakse taristu kaudu, mis **kuulub teie tiimile** — jagatud kaust (NAS, Syncthing) või teie oma git-hoidla. Taibu serverit ei ole kunagi vahel.

## Kuidas see töötab

- **Admin** loob tiimi, määrab **skoobid** (näiteks sales, marketing, klient-a) ja otsustab inimese ja skoobi kaupa, kes saab **lugeda** ja kes ka **kirjutada**.
- Kõik jagatav krüpteeritakse skoobivõtmetega enne, kui see sinu masinast lahkub. Tiimikaaslane, kellel skoobi võtit pole, ei saa selle skoobi andmeid lugeda — isegi kui ta näeb sünkikausta. Sünkikohas on alati ainult šifreeritud sisu.
- Sünk on **kahesuunaline**: kui lisad oskuse või salvestad otsuse skoopi, kuhu sul on kirjutusõigus, saavad selle kõik sama skoobi liikmed. Kui nemad midagi muudavad, saad sina. Konfliktsete muudatuste puhul jääb uusim versioon ja teine salvestatakse `.conflict` failina, nii et midagi ei kao.
- Kõik, mis on märgitud **privaatseks** (või üldse märkimata), ei lahku kunagi sinu arvutist. See on vaikimisi nii.

## Alustamine

1. **Admin:** ava Tiimi leht (inimeste ikoon), vali Loo tiim, määra sünkikoht (jagatud kaust või git-URL) ja saada tiimikaaslastele **tiimikood**.
2. **Liige:** kleebi tiimikood jaotisse Liitu tiimiga ja saada oma **liikmekood** adminile.
3. **Admin:** lisa liige, määra maatriksis tema õigused ja vajuta Sünkrooni. Valmis — edaspidi sünkroonivad mõlemad pooled ühe klõpsuga (ja projekti avamisel automaatselt).

## Mälu ja kaustade jagamine

- Igal struktureeritud mälestusel (faktil) on **skoop** — määra see paneelil „Mida Taibu mäletab". Ilma skoobita fakt on privaatne.
- Kaustad nagu `references/`, `decisions/` või oskus kaustas `.claude/skills/` jagatakse, sidudes need Tiimi lehel skoobiga.

## Uue tiimiliikmena liitumine

Kui keegi uus alustab, loob ta oma uue projekti (mitte koopia sinu omast) ja seadistab selle. Taibu küsib, kas ta seadistab oma äri või liitub tiimiga. Tiimiliikmelt ei küsita kunagi, mida ettevõte müüb või kes on kliendid, sest see pole tema välja mõelda: ta seadistab ainult iseenda ja oma kirjutamisviisi. Ettevõtte teadmine tuleb sünkides.

Järjekord on seega: loo projekt, liitu koodiga tiimiga, siis lõpeta isiklik seadistus. Pärast seda on tal esimesest päevast olemas sinu ettevõtte käsiraamat, viited, otsused ja jagatud mälu.

## Isiklik jääb isiklikuks

Kaks faili ei lahku kunagi kellegi arvutist, ükskõik mida jagamisseaded ütlevad: tema isiklikud vastused ja tema häälprofiil. Igaüks säilitab oma kirjutamisviisi ja identiteedi, samal ajal kui ettevõtte teadmine on jagatud. Keegi ei päri kellegi teise isiksust.

## Millised projektid sünkroonivad

Tiimi kuulumine käib **projekti kaupa**. Ühe projekti ühendamine tiimiga ei puuduta su teisi projekte ja jagatakse ning raporteeritakse ainult ühendatud projekti. Erinevad projektid võivad kuuluda eri tiimidesse, aga sama projekt ei saa kuuluda kahte tiimi ega kaks projekti ühte ja samasse tiimi ühes arvutis.

## Tiimi ülevaade

Kui admin lülitab sisse Tiimi ülevaate, koostab iga liikme Taibu väikese **tegevusaruande** ja saadab selle adminile automaatselt: mitu vestlust ja milliste agentidega, kuidas mälu kasvas, millised teemad ja oskused esile kerkisid, aktiivsus päevade kaupa viimase kahe nädala jooksul, ja kus keegi näib takerduvat (pikk edasi-tagasi, korduvad vead, vaiksed perioodid). Lühikese kirjaliku kokkuvõtte kirjutab liikme oma Taibu tema enda arvutis.

Admin näeb **Tiimi ülevaadet**: kogu tiimi numbrid, aktiivsus päevade kaupa, enim käsitletud teemad, „vajab abi" nimekiri ja kaart iga liikme kohta.

**Mis sinna kunagi ei satu:** sõnumite sisu, mustandid, privaatne või skoobita mälu, `.env` ja saladused. Kõik, mis satub, puhastatakse enne arvutist lahkumist e-postiaadressidest, telefoninumbritest, linkidest, võtmetest ning kaardi- ja kontonumbritest, ja kokkuvõte kirjutatakse juba puhastatud andmete põhjal.

Liige saab Tiimi lehel näha täpselt, mida tema kohta raporteeritakse. Kuna tegu on ettevõtte tööandmetega, ei saa ta seda muuta ega blokeerida, ainult vaadata. Päris isiklikud märkmed kuuluvad **privaatsesse** mällu, mis ei lahku arvutist üldse.

## Ausad piirid

- Liikme eemaldamine roteerib võtmed, nii et ta ei saa enam midagi uut, aga juba sünkroonitud koopiad jäävad tema masinasse. See on iga võrguvaba süsteemi füüsikaline omadus.
- Admini seade hoiab tiimi peavõtit — varunda see nagu parool.
