# Äpid

Taibu ei kirjuta ainult sinu ettevõttest. Ta võib sellele ka **tarkvara ehitada**. Kirjeldad, mida tahad näha, Taibu võtab andmed sinu ühendatud tööriistadest, kirjutab lehe ja lisab selle siia. Arendajat pole vaja, igakuist SaaS-i tasu pole, kasutajapõhist hinnastust pole.

**Ruudustiku ikoon → "Äpid"**

![Äppide leht](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/22-apps.png)

## Äpi küsimine

Lehe ülaosas olev kast ongi kogu liides. Kirjuta, mida tahad näha, ja vajuta **"Build it"** või Ctrl+Enter. See avab töö jaoks **uue agendi**: ta plaanib äpi, ehitab selle valmis ja lisab selle siia lehele, kui töö tehtud saab. Sina võid samal ajal teises sakis edasi töötada.

Ei tea, mida küsida? Vaata kasti. Kui sa midagi ei tee, kirjutab see sinna päris näiteid.

![Äppide leht enne esimese äpi loomist](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/22b-apps-empty.png)

Iga paan on **äpi enda reaalajas vaade**, mitte ikoon, nii et saad neil ühe pilguga vahet teha. Paan kirjaga **"Not running"** tähendab, et tegu on töötava äpiga, mille server on praegu peatatud. Ava see ja vajuta **"Start server"**.

## Üks töölauavaade nelja brauserisaki asemel

Enamikul ettevõtetel on sama auk. Reklaamiraha on Facebook Adsis. Veel raha on Google Adsis. Vihjed tulevad kodulehe vormi kaudu. See, kas neist lõpuks raha sai, on CRM-is. Miski ei seo neid kokku, seega ei oska keegi vastata ainsale küsimusele, mis loeb: milline kanal tegelikult raha sisse toob?

Ühenda need tööriistad ja küsi siis ühe lausega:

> "Ehita mulle reaalajas töölaud: Facebooki ja Google'i reklaamikulu, vihjed veebilehe funnelist ja millised neist vihjetest me ClickUpis võitsime. Näita kulu vihje kohta ja tasuvust kanali kaupa."

![Valmis äpp Taibus avatuna](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/et/29-app-open.png)

Vaata, millele see vastab. Facebook toob 171 vihjet hinnaga 29 eurot tükk, Google toob 84 hinnaga 42. Vihje hinna järgi võidab Facebook ja enamik inimesi tõstaks eelarve sinna ümber. Aga Google sulges oma 84 vihjest 10, Facebook aga 171 vihjest 9, seega tõi Google tagasi 5.5 korda ja Facebook 2.7. Odavam kanal oligi kehvem ja kumbki reklaamiplatvorm ei saa sulle seda öelda, sest kumbki ei tea, mis lõpuks ära võideti.

## Veel asju, mida tasub ehitada

- **Raha ja runway**: pangakonto pluss väljaminevad arved, et näeksid päris seisu
- **Müügitoru etappide kaupa**: CRM-i tehingud ja kui kaua igaüks on kinni olnud
- **Kliendiaruanne**: üks leht kliendi kohta, mille saad kuu lõpus teele panna
- **Vihjete kvaliteet allika järgi**: mitte kes saadab kõige rohkem vihjeid, vaid kes saadab need, kes allkirjastavad

## Reaalajas või hetkepilt

| Tüüp | Kuidas see töötab | Kasuta siis, kui |
|---|---|---|
| **Reaalajas** | Käivitab väikese kohaliku serveri ja loeb andmed iga kord uuesti, kui selle avad | See on sulle endale ja tahad näha tänaseid numbreid |
| **Hetkepilt** | Üks HTML-fail, kuhu andmed on sisse kirjutatud, serverit pole | Tahad selle saata kliendile või raamatupidajale |

Hetkepilt on üks fail. Saadad selle ära ja see lihtsalt avaneb. Saajal pole vaja midagi paigaldada.

## Äpi ise lisamine

Vahel pole midagi ehitada vaja: sul on HTML-fail juba olemas või sinu enda server juba töötab. Lehe all olev **"Add one manually"** küsib nime, aadressi, näiteks http://localhost:8000, või HTML-faili, ja soovi korral ka käivituskäsku. Käivituskäsk jookseb äpi avamisel sisseehitatud terminalis, nii et server läheb ise käima.

## Kui äpp on tühi

Selle server ei tööta. Vajuta **"Start server"** või käivita see ise, siis vajuta **"Reload"**. Hetkepiltidega seda ei juhtu, sest seal pole serverit, mida käivitada.

## Kuhu andmed lähevad

Äpp töötab sinu arvutis ja loeb ühendatud tööriistadest. Taibusse ei laadita midagi üles. Leht on sinu projektis fail, mida saad avada, muuta või kustutada nagu iga teist faili.
