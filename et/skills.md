# Oskused

Taibu AI OS-i võimekust saab laiendada oskustega. Oskus on üks Markdown-fail, mis ütleb Claude'ile, kuidas mingis olukorras käituda. Süsteem kasutab Claude Code'i natiivset `/skills` mehhanismi.

## Struktuur

Oskused elavad projekti `.claude/skills/` kaustas:

```
.claude/skills/
  pipedrive-kontakt/
    SKILL.md
  meili-mustand/
    SKILL.md
```

Iga `SKILL.md` koosneb kahest osast:

```markdown
---
name: pipedrive-kontakt
description: Kasuta, kui kasutaja ütleb "lisa kontakt", "uus klient Pipedrive" või küsib Pipedrive'i kohta
---

Siia kirjuta juhendid Claude'ile täpselt selles stiilis, milles ta peab käituma.
Näiteks: milliseid välju küsida, mis järjekorras tegutseda, kuidas API-d kutsuda.
```

`description` on kõige tähtsam väli — see määrab, millal Claude oskust rakendab.

## Oskuse muutmine — markdowni pole vaja

Kui avad `SKILL.md` faili, näitab Taibu AI OS seda **vormina**, mitte toore markdownina: nimi, kirjeldus ja iga sektsioon on eraldi sisestusväljad. Kirjuta väljadesse ja vajuta **Ctrl+S** — fail jääb korrektseks, nii et sa ei saa kogemata rikkuda frontmatter'it ega pealkirju.

Vaja struktuuri muuta või sektsiooni lisada? Klõpsa redaktori paremas ülanurgas **Lähtekood**, et minna lähtekoodile, ja **Vorm**, et tagasi tulla. Uued oskused avanevad automaatselt vormivaates.

## Kust oskusi leida

**[skills.sh](https://skills.sh/)** — oskuste kataloog. Leia valmis oskusi erinevate tööriistade ja töövoogude jaoks. Kopeeri SKILL.md sisu ja pane õigesse kausta.

**GitHub** — paljud arendajad jagavad oskusi avalikes repodes. Anna Claude'ile lihtsalt link ja palu see paigaldada:

> *"Paigalda see oskus: https://github.com/kasutaja/repo"*

Claude laeb SKILL.md alla ja paneb õigesse kausta.

**Loo ise** — ütle Claude'ile, mida vaja:

> *"Tee mulle oskus, mis aitab mulle Pipedrive kontakte lisada — küsib nime, e-maili ja ettevõtte ning lisab API kaudu"*

Claude loob vajaliku faili ja järgmine kord teab täpselt, mida teha.

## /find-skills käsk

Kirjuta vestlusaknasse:

```
/find-skills
```

Claude aitab leida sobivaid oskusi vastavalt sinu töövoogudele ja ühendatud tööriistadele. Oskusi saab otsida nii skills.sh-st, GitHubist kui ka teistest allikatest.

## Näited praktikas

- **Klientide haldus** — oskus, mis teab, kuidas Pipedrive'i kontakti lisada, tehingut luua, märkust kirjutada
- **Arved** — oskus, mis genereerib Merit Aktiva arve õiges formaadis
- **Sisu** — oskus, mis kirjutab LinkedIn postitusi sinu häälregistris (K2-st)
- **Iganädalane ülevaade** — oskus, mis koostab koosolekukokkuvõtte kindlas struktuuris

Üks oskus = üks töövoog, mida enam ei pea meeles pidama.
