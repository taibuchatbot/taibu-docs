# Alusta siit

Taibu AI OS on sinu isiklik AI operatsioonisüsteem. See juhend aitab sul esimese tunniga tulemusse jõuda.

## Mis see on?

Taibu AI OS ühendab Claude AI-d sinu projekti failide, tööriistade ja mõtteviisiga. Sa ei kasuta AI-d lihtsalt küsimuste esitamiseks — sa ehitad endale isikliku operaatori, kes tunneb sinu äri.

## Esimesed sammud

### 1. Logi Claude sisse

Esmakäivitusel avaneb sisselogimise juhend. Vali, kas kasutad Claude tellimust (Pro/Max/Team) või API-arveldust, ja järgi samme. Olek näed igal ajal **Seaded → CLAUDE OLEK**.

### 2. Loo oma esimene projekt

Klõpsa vasakul üleval **projektivalija** nupul ("Vali projekt") ja siis **"Lisa projekt…"**. Sisesta projekti nimi (nt kliendi nimi). Taibu kopeerib kogu template struktuuri automaatselt.

### 3. Käivita /onboard

Kirjuta vestlusaknasse:

```
/onboard
```

Claude küsib sinult 7 küsimust — kes sa oled, mida teed, millised tööriistad sul on. Vastused salvestatakse `context/` kausta ja muudavad iga järgmise vestluse palju täpsemaks.

### 4. Räägi Claude'iga

Vestlusaken töötab nagu Claude.ai, aga Claude näeb su projekti faile ja saab neid otse muuta. Küsi midagi konkreetset:

- *"Vaata intake.md ja ütle, mida puudu jääb"*
- *"Loo mulle e-mail uuele kliendile, kes tegeleb kinnisvara haldusega"*
- *"Mis automatiseeringuid saaks minu töövoos teha?"*

### 5. Ühenda oma tööriistad

Vestluskasti kõrval on **+** nupp. Sealt valid populaarseima ühenduse — Google Drive, Gmail, Notion, Slack jne — ja Claude juhendab sind seadistamisel. Nii saab Claude su päris andmetega töötada.

Faili saab vestlusse lisada **kirjaklambri** ikooniga (pildid, dokumendid). GitHubi ühendamiseks vaata **Seaded → GITHUB**.

### 6. Muuda faile otse

Klõpsa vasakul failipuus mõnda faili (nt `CLAUDE.md` või `intake.md`). Fail avaneb redigeeritava tekstina. **Ctrl+S** salvestab. HTML-faili saab vaadata ka eelvaatena, pildid avanevad pildina.

### 7. Käivita /audit nädala pärast

```
/audit
```

Claude vaatab läbi, mis on tehtud ja mis puudu. Hea tava: kord nädalas.

---

## Kiired viited

| Käsk | Mis teeb |
|------|----------|
| `/onboard` | Seadistab projekti (täidab context kaustad) |
| `/audit` | Lünkade aruanne — mis puudu |
| `/level-up` | Iganädalane 3M-i intervjuu |
| `/roast` | Testib idee 5 persona nõukoguga |
| `/clear` | Tühjendab vestluse (alustab uue sessiooni) |
