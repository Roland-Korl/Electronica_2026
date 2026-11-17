# Sunj Energy

| | |
|---|---|
| **Stav** | kontakt |
| **Web** | neznámy |
| **Krajina / mesto** | Čína (podľa predvoľby telefónneho čísla; mesto neznáme) |
| **Stretli sme sa** | Electronica 2026, Mníchov (presný dátum a stánok doplniť) |
| **Ďalší krok** | počkať na ponuky a aktualizované výkresy od Anne (2026-11-18) |
| **Termín** | 2026-11-18 |

## Kontaktné osoby

| Meno | Rola | E-mail | Telefón | Poznámka |
|---|---|---|---|---|
| Anne | zástupkyňa Sunj Energy (rola neznáma) | neznámy | +86 133 3379 5798 (WhatsApp) | Prvá správa 2026-11-17 ráno. Číslo nie je v kontaktoch. Priezvisko neznáme. |

## Čo nás zaujíma

- Produkty: primárny batériový pack Li-SOCl2 + hybridný impulzný kondenzátor (HLC / SPC) do zaliateho vonkajšieho zariadenia s rádiovým modulom. Máme dva dopyty (nemecky, slovenský preklad vedľa):
  - **EPS-BAT-01**: zaliaty natrvalo, min. 4 Ah, životnosť 10 rokov, vodiče, [preklad](navrhy/EPS-BAT-01_dopyt_sk.md)
  - **EPS-BAT-02**: výmenný pack (trieda ER26500 + SPC1520, veľkosť C), min. 8 Ah, životnosť 3 roky, kontakty bez vodičov, [preklad](navrhy/EPS-BAT-02_dopyt_sk.md)
  - Sunj Energy má obe podklady. **Rozhodnutie 2026-11-17:** pôvodné dopyty BAT-01 a BAT-02 už neplatia. Nová verzia zariadenia je krabica namiesto rúrky a je navrhnutá na hotový štandardný pack Sunj Energy (ER26500H + EPC1520, s káblom a konektorom). Dizajn si prispôsobíme my.
- Požadované batérie (2026-11-17): dve aplikácie, **aplikácia 1: 8,5 Ah + SPC**, **aplikácia 2: aspoň 19 Ah + SPC**. Priorita: čo najväčšia kapacita v čo najmenšom púzdre. Konektor: **JST XH 2,5 mm** (na PCB B2B-XH-A(LF)(SN)); potrebný protikus **XH-2P**; **+ na pine 1, − na pine 2** (overiť podľa PCB). Pôvodne uvádzaný PH 2.0 bol omyl.
- Špecifikácie od Sunj (2026-11-17): [ER26500H + EPC1520, 8,5 Ah](dokumenty/SUNJ_ER26500H-EPC1520_specifikacia_sk.md) a [ER34615H + EPC1520, 19 Ah](dokumenty/SUNJ_ER34615H-EPC1520_specifikacia_sk.md); kábel 100 mm, konektor PH-2P 2,0 mm. Anne ponúka vodotesnú úpravu podľa našich požiadaviek ([záznam](komunikacia/2026-11-17_whatsapp_anne-specifikacie-a-vodotesnost.md)).
- Predpokladané množstvá: vzorky 20 ks (Q1 2027), séria 1 000 – 3 000 ks ročne (pri BAT-02 plus náhradné packy)
- Účel / projekt: doplniť

## Katalóg a hotové packy (2026-11-17)

Podrobnosti: [prehľad katalógu](dokumenty/SUNJ_katalog_vyber_sk.md), [kondenzátory EPC1520 / EPC1550](dokumenty/SUNJ_EPC1520_EPC1550_specifikacia_sk.md), [záznam komunikácie](komunikacia/2026-11-17_whatsapp_anne-katalog-baterii.md).

| | kondenzátor na článku | kondenzátor vedľa článku |
|---|---|---|
| 8,5 Ah | ER26500H + EPC1520, Ø29 × 67 mm | ER26500H + EPC1550, 55 × 44 × 28 mm |
| 19 Ah | ER34615H + EPC1520, Ø34 × 78 mm | ER34615H + EPC1550, 64 × 55 × 35 mm |

**Výkresy s EPC1520 vedľa článku** ([prehľad](navrhy/SUNJ_vykresy_vedla-seba_sk.md)): ER26500H + EPC1520 = 52 × 40 × 26 mm; ER34615H + EPC1520 = 63 × 48 mm (hrúbka nie je zakótovaná). Kábel 100 ± 5 mm, konektor na výkrese nie je určený (treba XH-2P).

Firma: SUNJ Energy (Luoyang) Co., Ltd, založená 2017, areál 33 300 m², ISO 9001 / 45001 / 14001, výrobky UL, CE, UN 38.3, RoHS (podľa katalógu, neoverené). Web www.sunj.com.

## Obchodné podmienky

- Cena / cenník (2026-11-17, Anne, množstvo a podmienky nepotvrdené): **ER26500H + EPC1520 = 3,5 USD/ks**, **ER34615H + EPC1520 = 5 USD/ks**; poloha kondenzátora cenu neovplyvňuje. Doprava sa ešte počíta zvlášť.
- MOQ (min. množstvo): zatiaľ nie
- Dodacia lehota: zatiaľ nie
- Platobné podmienky: zatiaľ nie
- Exkluzivita / distribúcia: zatiaľ nie

## Zhrnutie rokovania

- 2026-11-17 (neskôr): Anne sa pýta, či chceme len pack ER26500H + EPC1520, a upozorňuje, že takéto packy sa dodávajú s káblom a konektorom. Poslala aj e-mail.
- 2026-11-17 (ráno): Anne napísala cez WhatsApp. Ich vývojové oddelenie (R&D) stále vyhodnocuje špeciálny batériový pack, na ktorý sme sa pýtali. Detaily v [komunikacii](komunikacia/2026-11-17_whatsapp_anne-vyhodnocuje-pack.md).

## Otvorené otázky

- [x] **Vodotesnosť:** nie je potrebná, zariadenie bude vo vodotesnej krabičke (Roland, 2026-11-17).
- [ ] Vypýtať: cenu pre 100 / 1 000 / 5 000 ks, dodaciu lehotu 20 vzoriek, rozmery packu ER34615H, polaritu pinov (+ pin 1, − pin 2), napätie počas impulzov 0,6 A pri −30 °C.

- [ ] Vypýtať od Anne: typ konektora a protikus, dátový list, legendu položiek 1–11, rozdiel medzi verziami 65 / 67 / 68 mm. Výkresy: [65 a 68 mm](navrhy/2026-11-17_sunj_vykres-pack-kabel-konektor.jpg), [67 mm, kábel 100 ± 5 mm](navrhy/2026-11-17_sunj_vykres-pack-67mm-kabel-100mm.jpg); všetky Ø27 mm.
- [ ] Prečítaný e-mail od Anne (2026-11-17): ak v ňom bolo niečo dôležité, doplniť do `komunikacia/`.
- [ ] Potvrdiť Anne, že chceme pack ER26500H + EPC1520 a že akceptujeme kábel s konektorom (viď [záznam](komunikacia/2026-11-17_whatsapp_anne-er26500h-epc1520.md)).
- [ ] Pošlú zoznam štandardných článkov / packov (dátové listy, ceny, dodacia lehota, MOQ)?
- [ ] Ktoré štandardné batérie vyhovujú: impulzy 0,6 A pri −30 °C, životnosť, rozmery? Podľa toho upraviť zariadenie.
- [ ] Kedy budú mať výsledok vyhodnotenia?
- [ ] Získať e-mail a priezvisko Anne, prípadne vizitku.
- [ ] Zistiť web firmy a overiť ju (číslo nie je v kontaktoch, čínsky dodávateľ).
