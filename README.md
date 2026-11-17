# Electronica 2026

Archív komunikácie a obchodných rokovaní s výrobcami, s ktorými sme sa stretli na veltrhu Electronica 2026.
Každý výrobca má vlastnú zložku s komunikáciou, obrázkami, návrhmi a dokumentmi.

> Repo je súkromné: obsahuje kontakty a ceny.

## Štruktúra

```
PREHLAD.md              tabuľka všetkých výrobcov a ich stavu (aktualizovať ručne)
_sablona/               vzor zložky, ktorý kopírujeme pre každého nového výrobcu
vyrobcovia/<nazov>/     zložka jedného výrobcu
├── README.md           karta výrobcu: kontakty, záujem, stav, ďalší krok
├── komunikacia/        jeden súbor na jednu udalosť (e-mail, hovor, stretnutie)
├── obrazky/            fotky z veltrhu, produktov, vizitky
├── navrhy/             cenové ponuky, naše návrhy, špecifikácie (verzie _v1, _v2)
└── dokumenty/          katalógy, cenníky, zmluvy, certifikáty v pôvodnej podobe
```

## Pravidlá pomenovania

- **Zložka výrobcu:** malé písmená, bez diakritiky, pomlčky: `acme-electronics`.
- **Súbory:** začínajú dátumom `RRRR-MM-DD_`, aby sa radili chronologicky.
  - `komunikacia/2026-11-17_email_cenova-ponuka.md`
  - `komunikacia/2026-11-12_stretnutie-veltrh.md`
  - `obrazky/2026-11-12_vizitka-jan-novak.jpg`
  - `navrhy/2026-11-20_ponuka_v2.pdf`
- **Typ udalosti** v názve komunikácie: `email`, `hovor`, `stretnutie`, `chat`.

## Stavy výrobcu

`kontakt` → `rokovanie` → `ponuka` → `objednavka` → `uzavrete`
(mimo hlavnej cesty: `pozastavene`, `zrusene`)

## Postup

### Nový výrobca
1. Skopíruj `_sablona/` do `vyrobcovia/<nazov>/`.
2. Vyplň `README.md` (karta výrobcu).
3. Pridaj riadok do `PREHLAD.md`.
4. Vymaž vzorový súbor `komunikacia/_vzor.md`.

### Nová komunikácia
1. Vytvor súbor v `komunikacia/` podľa vzoru (`_vzor.md` v šablóne).
2. Vlož text e-mailu. Prílohy ulož do `dokumenty/` alebo `navrhy/`, odkaz na ne daj do záznamu.
3. Napíš dve-tri vety zhrnutia a dohodnuté kroky.
4. Aktualizuj stav a „ďalší krok“ v karte výrobcu a v `PREHLAD.md`.

### Commity
Malé a zrozumiteľné, s názvom výrobcu na začiatku: `acme: ponuka v2 + odpoveď na cenu`.

## Veľké súbory

Fotky a PDF ukladáme priamo do repa. Ak ich bude veľa (repo nad ~500 MB), presunieme originály na Google Drive a v kartách necháme odkazy.
