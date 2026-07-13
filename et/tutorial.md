# Kuidas Taibu AI OS-i kasutada

Tere. See ei ole juturobot. See on sinu isiklik AI-töösüsteem.
See tunneb su äri, mäletab su otsuseid ja teeb päriselt tööd sinu
eest. Siit lehelt näed, kuidas seda kasutada. Lugemiseks kulub 5 minutit.

## 1. Mida sa siin näed

- **Vasakul**: sinu projektifailid. Kõik, mida AI sinu kohta teab,
  on nendes failides. Saad neid kõiki avada ja muuta.
- **Keskel**: vestlus. Siin sa töötad. Räägi sellega nii, nagu
  räägiksid targa abilisega, kes oskab ka asju ÄRA teha, mitte ainult vastata.
- Sa ei pea olema tehniline. Tavaline keel sobib. Oma sõnadega,
  omas keeles.

## 2. Esimene päev: tee onboarding ära

Kirjuta vestlusse `/onboard` või vajuta nuppu.

AI küsib sinult 7 küsimust: kes sa oled, mida sa müüd, mis on su
prioriteedid, milliseid tööriistu kasutad ja kuidas sa kirjutad.
Siis paneb ta kõik ise paika.

Üks reegel: kui ta küsib kirjutamisnäiteid, siis **kleebi päris e-kirju või postitusi,
mida oled varem kirjutanud**. Ära kirjuta vestlusse uusi. Tal on vaja sinu päris
häält, mitte seda häält, millega sa "püüad hästi kõlada".

Pärast onboardingut proovi seda: küsi *"Millele ma peaksin sel nädalal keskenduma?"*
Näed vahet kohe. Ta vastab sinu PRIORITEETIDE järgi.

## 3. Igapäevane kasutus: lihtsalt küsi

Asjad, mida inimesed tavalisel päeval küsivad:

- *"Koosta sellele e-kirjale vastus"* (kleebi e-kiri sisse)
- *"Tee sellest dokumendist kokkuvõte ja anna mulle 3 tegevuspunkti"*
- *"Mida me eelmisel kuul hinnastamise kohta otsustasime?"*
- *"Tee mulle pakkumine kliendile, kes tahab X-i"*
- *"Pane mulle kokku lihtne ülevaade mu nädalast"*

AI saab lugeda ja muuta sinu projektifaile, otsida veebist ning töötada
kõigi tööriistadega, mille oled ühendanud. Kui sa pole kindel, kas ta
midagi teha saab, siis küsi. Halvimal juhul ütleb ta "ei, aga siin on, mida mul selleks vaja oleks".

## 4. Ühenda oma tööriistad

AI muutub päriselt kasulikuks siis, kui ta pääseb ligi sinu päris andmetele:
e-post, kalender, failid, raamatupidamine, CRM.

Kui tahad midagi ühendada, ütle seda lihtsalt vestluses:

- *"Ühenda mu Gmail"*
- *"Ühenda Google Calendar"*
- *"Ma tahan, et sa näeksid mu Pipedrive'i"*

Ta seletab sammud lahti ja teeb seadistuse koos sinuga ära. Mõned tööriistad
saavad ühendatud paari klikiga. Mõne jaoks on vaja API-võtit. AI ütleb sulle
täpselt, kust selle saad ja millisele reale see `.env` failis panna.

**Tähtis: ära kleebi API-võtmeid kunagi vestlusesse.** Võtmed lähevad otse
`.env` faili. AI teab seda reeglit ja peatab sind, kui selle unustad.

## 5. Iganädalased harjumused: siin hakkab mõju kasvama

Kaks sisse ehitatud harjumust hoiavad su süsteemi kasvamas. Need, kes need vahele jätavad,
lõpetavad kalli juturobotiga. Need, kes neist kinni peavad, saavad endale
töösüsteemi.

**`/audit` on sinu iganädalane kontroll (alates 7. päevast).**
See hindab su seisu 4 samba järgi: Kontekst, Ühendused, Võimed,
Harjumus. Saad skoori 100 punktist ja 3 kõige mõjusamat asja, mida
parandada. Tee seda kord nädalas. Mõte ongi selles, et näed skoori tõusmas.

**`/level-up` on reede rituaal (alates 14. päevast).**
Lühike vestlus, mis leiab ÜHE asja, mida sa sel nädalal käsitsi tegid ja
mille AI võiks üle võtta, ning siis ehitab selle valmis. Üks nädal, üks
automaatika. Mõne kuu pärast töötab sul masin sinu eest.

Rakendus tuletab meelde, kui on aeg need teha. Ära jäta vahele.

## 6. Kasvata seda: uued oskused

"Oskus" on võime, mille sinu AI on ära õppinud. Korduv viis, kuidas mingi
ülesanne hästi ära teha. Su OS-is on mitu sellist juba olemas. Sa saad neid juurde lisada:

**Leia valmis oskusi.** Kirjuta `/find-skills` ja kirjelda, mida sul vaja
on: *"leia oskus arvete kirjutamiseks"*. Ta otsib oskuste ökosüsteemist
ja paigaldab sobiva.

**Muuda äsja tehtud töö oskuseks.** See on kogu selle rakenduse kõige võimsam
harjumus. Alati kui AI just tegi midagi hästi, ütle:

> *"Väga hea. Salvesta see oskusena, et teeksime seda järgmine kord samamoodi."*

Ta paneb meetodi kirja ja edaspidi on see ülesanne ühe käsu kaugusel.
Kas ta tegi hea pakkumise? Hea nädalaraporti? Hea vastuse
kaebusele? Tee neist igaühest oskus. Nii muutub su OS iga nädal targemaks.
Ja see jääb sinu omaks.

## 7. Väikesed nõuanded

- **Uus vestlus iga teema jaoks.** Kasuta vestluse vahekaardi kõrval olevat + märki. Nii püsib fookus paigas.
- **Lisa faile** kirjaklambri kaudu: ekraanipildid, PDF-id, tabelid.
- **Ta jätab meelde.** Otsused lähevad otsuste logisse, kontekst failidesse.
  Kui juhtus midagi tähtsat, ütle *"pane see kirja."*
- **Küsi dashboardi.** *"Tee mulle mu reklaamitulemuste dashboard"* ja
  see ilmub siia paneeli, Dashboards alla.
- **Jäid hätta?** Küsi AI enda käest: *"Kuidas ma peaksin sind X jaoks kasutama?"* Ta tunneb
  kogu seda süsteemi ja juhatab sind õigesse suunda.
