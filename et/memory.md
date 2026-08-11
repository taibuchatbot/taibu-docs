# Mida Taibu mäletab

Taibu mäletab sinu tööd kuude kaupa. Kõik on sinu projektis lihtfailidena, mida saad lugeda, muuta või kustutada.

**Hammasratta ikoon → Seaded → "Mälu"**

![The memory panel](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/15-memory.png)

## Kolm kihti ja failid nende taga

| Kiht | Kus see asub | Mis see on |
|---|---|---|
| **Koondatud tõde** | `memory.md` | Lühike, hoolikalt valitud kokkuvõte sellest, mis on sinu ja su töö juures kõige olulisem. See hoitakse meelega lühike, sest see laaditakse igasse vestlusesse |
| **Struktureeritud mälestused** | `memory/facts/<name>.md`, üks fail iga fakti kohta | Igas failis on üks püsiv fakt, näiteks otsus, parandus, eelistus, hind, klient või tööriist, mida kasutad. Aegunud faktid liiguvad kausta `memory/facts/archived/` |
| **Ajajoon** | `memory/journal/<year-month>.md`, lisaks `memory/today.md` | Lisanduv logi kuu kaupa ja lühike kokkuvõte tänasest tööst. Midagi ei visata ära |

On veel üks fail, `memory/recall.mjs`, see on väike otsinguprogramm, mida Taibu käivitab sinu struktureeritud mälestuste peal siis, kui küsid midagi vana kohta.

## Kuidas mälestused kirja pannakse

Selleks on kolm viisi ja kõik kolm jõuavad samadesse failidesse.

1. **Automaatselt, pärast iga vahetust.** Rakendus vaatab, mis just juhtus, ja salvestab kõik, mis tundub püsiva faktina.
2. **Taibu poolt töö käigus.** Kui teed otsuse, parandad midagi, väljendad eelistust või mainid midagi oma töökorralduse kohta, kirjutab Taibu fakti kohe üles, mitte ei oota automaatset läbivaatust.
3. **Sinu poolt.** Kõik Mälu paneelis on muudetav ja "Muuda tekstina" avab ümberkirjutamiseks toorfaili `memory.md`.

Struktureeritud mälestus ei ole lihtsalt üks lause. Iga selline kirje talletab **millal see õpiti, milline agent selle õppis, millisest vestlusest see pärineb, kes seda ütles, sinu täpsed sõnad, failid mida tasub kontrollida, kui oluline see on ja kas see kehtib endiselt**. Just see teeb kuude pärast antud vastuse kontrollitavaks, mitte oletuseks.

## Mida Taibu loeb ja millal

Seda tasub teada, sest see selgitab, miks Taibu teab mõnda asja kohe ja mõne puhul peab otsima.

**Laaditakse igasse sõnumisse, alati:**

- `memory.md`, koondatud tõde
- kokkuvõte sinu kõige uuematest ja olulisematest struktureeritud mälestustest
- `memory/today.md`

**Avatakse ainult vajaduse korral:** täielikud faktifailid, kuude kaupa peetud päevik ja kõik muu sinu projektis. Vanem või täpsem kontekst tuuakse välja meenutuse kaudu, mitte ei hoita kogu aeg kaasas.

Seepärast hoitakse koondatud tõde lühike. See on osa, mida Taibu ei pea kunagi eraldi üles otsima, seega peaks seal olema see, mis on sinu kohta üldiselt tõsi, mitte iga üksik detail, mida oled kunagi maininud.

## Meenutus

Küsi millegi kohta, mis juhtus kuid tagasi, just nende sõnadega mis pähe tulevad. Taibu otsib oma struktureeritud mälestustest ja vastab **viidetega**: milline fail, mis kuupäev, kes seda ütles ja milliseid täpseid sõnu kasutasid.

Kui ta ei leia midagi, ütleb ta seda otse ega paku. Sama moodi saad otsida ka ise Mälu paneeli ülaservas olevast kastist.

Meenutus loeb faktifaile. Kui sinu teadmine on läinud ainult faili `memory.md`, siis ei ole tal midagi otsida ja Taibu ütleb seda.

## Impordi oma ajalugu

Esimesel korral vajuta **"Impordi varasemad vestlused"**. Taibu muudab sinu olemasoleva vestlusajaloo otsitavaks mäluks, nii et alustad kõigega, mida oled talle juba rääkinud.

## Kuidas hoida kõik korras

Lisa rutiin **"Memory tidy-up"** ja Taibu korrastab kord nädalas, ühendab duplikaadid, arhiveerib aegunud faktid ja viib korduvad teemad koondatud tõe sisse. Olulisi ja kinnitatud fakte ei eemaldata kunagi automaatselt.

## Privaatsus

Mälu on lokaalne. See on sinu projektikaustas tavaliste failidena ja midagi ei saadeta Taibu serverisse.

Mälestus, millel **puudub ulatus, on privaatne** ja ei lahku kunagi sinu arvutist. See on vaikimisi seadistus. Jagatakse ainult neid mälestusi, millele on selgelt antud tiimi ulatus, ja ka siis krüptitakse need enne väljasaatmist. Vaata jaotist **Tiimina töötamine**, et mõista, kuidas ulatused töötavad.

Kahte faili ei jagata tiimiga kunagi, ükskõik kuidas jagamine on seadistatud, sinu sisseelamise vastused failis `intake.md` ja sinu isiklik profiil failis `context/persona.md`. Ülejäänu kohta, mida Taibu sinu kohta kirjutab, vaata jaotist **Sinu andmed**.
