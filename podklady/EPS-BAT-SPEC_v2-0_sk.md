# EPS-BAT-SPEC v2.0 – požiadavky na batériové packy pre výrobcov (slovenská verzia)

Spoločný dokument pre **všetkých výrobcov batérií**. Na odoslanie: [EPS-BAT-SPEC_v2-0_en.pdf](EPS-BAT-SPEC_v2-0_en.pdf) (angličtina, 3 strany). Zdroj PDF: [EPS-BAT-SPEC_v2-0_en.html](EPS-BAT-SPEC_v2-0_en.html).
Nahrádza pôvodné dopyty EPS-BAT-01 a EPS-BAT-02. Vznikol spojením [EPS-BAT-LP](../vyrobcovia/sunj-energy/navrhy/EPS-BAT-LP_profily-zataze_sk.md) a [VLD2 FullMonitor](../vyrobcovia/sunj-energy/navrhy/2026-11-18_VLD2-FullMonitor_bateria-pre-dodavatela_sk.pdf), vždy s **horšou hodnotou** z oboch a s rezervou ([porovnanie](../vyrobcovia/sunj-energy/navrhy/porovnanie_poziadaviek_EPS-BAT-LP_VLD2.md)).

Zámerne vynechané oproti podkladom: zmienka o konkurenčnom type (EVE), externá batéria 12 V LiFePO4, priestor a zaliatie podľa BAT-01/02, konkrétne použitie VLD2 (obmedzovač napätia), objem 50 000 ks ročne (len „potenciál výrazne vyšších objemov").

## Zhrnutie

Dva primárne packy Li-SOCl2 3,6 V (bobbin) s paralelným hybridným impulzným kondenzátorom (HLC / SPC) pre dve vonkajšie zariadenia s rádiovým modulom:
- **Pack A** asi 8,5 Ah (trieda C) pre úsporné zariadenie so životnosťou **10 rokov**,
- **Pack B** asi 19 Ah (trieda D) pre monitorovacie zariadenie so životnosťou **aspoň 3 roky**.

Oba sú hotové packy (článok + kondenzátor) s vodičmi a konektorom JST XHP-2, vymeniteľné na mieste, nezaliate. Hodnoty odberu sú **najhorší prípad s rezervou**.

## 1 Prehľad

| | Pack A – úsporné zariadenie | Pack B – monitorovacie zariadenie |
|---|---|---|
| Kapacita | asi 8,5 Ah (napr. 26500 / C + 1520) | asi 19 Ah (napr. 34615 / D + 1520) |
| Napätie | 3,6 V; naprázdno max. 3,9 V | rovnako |
| Návrhový priemerný prúd (s rezervou) | **50 µA** (1,2 mAh/deň, 0,44 Ah/rok) | **450 µA** (10,8 mAh/deň, 3,9 Ah/rok) |
| Životnosť | min. 10 rokov | min. 3 roky, potom výmena |
| Rádiové spojenie | ≈ 144 mA, ≈ 17 s, každých 48 h | ≈ 130 mA, ≈ 80 s (max. 7 min), 1× denne |
| Impulzy | do **0,6 A / 10 ms**, stovky až tisíce za spojenie; zapnutie modemu ≈ 0,55 A < 1 ms | rovnako |
| Priestor | zatiaľ neurčený: ponúknuť rúrku aj vedľa seba | **max. 65 × 50 × 38 mm**, max. 120 g, verzia vedľa seba |

## 2 Elektrické požiadavky

- Napätie pri impulze 0,6 A / 10 ms: **min. 3,2 V** v celom rozsahu teplôt a životnosti, aj po dlhom pokoji (pasivácia). Pod 3,0 V sa zariadenie môže reštartovať.
- Počas rádiového spojenia: **min. 3,3 V** priemerne pri ≈ 150 mA až 7 min.
- Trvalý prúd: min. 150 mA až 7 min.
- Samovybíjanie: max. 1 % ročne pri +25 °C.
- Nabíjanie: nikdy (dva nezávislé blokovacie prvky, spätný prúd < 1 µA).
- Ochrana: v zariadení poistka 2 A a ochrana proti prepólovaniu; poistka/PTC v packu vítaná, ak úbytok pri 0,6 A je max. 0,1 V.

## 3 Profil záťaže A

| Fáza | Prúd | Trvanie | Opakovanie | mAh/deň |
|---|---|---|---|---|
| Spánok | 13,7 µA | trvalo | – | 0,329 |
| Meranie | ≈ 5 mA (16 × ≈ 2 ms) | 35 ms | každých 60 s | 0,070 |
| Zápis dát | ≈ 40 mA | ≈ 0,25 s | 6× denne | 0,018 |
| Rádiové spojenie | ≈ 144 mA, impulzy do 0,6 A / 10 ms | ≈ 17 s | každých 48 h | 0,340 |
| Spojenie bez siete (zriedka) | ≈ 37 mA, impulzy do 0,6 A | do 300 s | ≈ 1× za 2 mesiace | 0,051 |
| **Spolu (výpočet)** | **≈ 33,7 µA** | | | **0,808** |
| **Návrhová hodnota** | **50 µA** (≈ 50 % rezerva) | | | **1,200** |

Kontrola: 10 rokov × 0,44 Ah + samovybíjanie ≈ 5,2 Ah; predpoklad ≈ 6,7 Ah využiteľných z 8,5 Ah.

## 4 Profil záťaže B

| Fáza | Prúd | Trvanie | Opakovanie | mAh/deň |
|---|---|---|---|---|
| Spánok | 12,5 µA | trvalo | – | 0,300 |
| Meranie prúdu | ≈ 5 mA | ≈ 2 ms | 10× za sekundu | 2,400 |
| Meranie napätia | 28,5 mA typ., **41 mA max.** (počítané so 41 mA) | ≈ 3 ms | 1× za sekundu | 2,952 |
| Prebudenie, zápis dát | 25 … 40 mA | 50 … 110 ms | ≈ 200× denne | 0,312 |
| Udalosti | ≈ 1 mA | do 30 s | ≈ 10× denne | 0,083 |
| Rádiové spojenie LTE-M | ≈ 130 mA; impulzy do 0,6 A / 1 … 10 ms; zapnutie 0,55 A < 1 ms | ≈ 80 s (max. 7 min) | 1× denne | 2,889 |
| **Spolu (najhorší prípad)** | **≈ 372 µA** | | | **8,936** |
| **Návrhová hodnota** | **450 µA** (≈ 20 % rezerva) | | | **10,800** |

Najhorší deň: neúspešné spojenie sa opakuje o 1 h a o 4 h, každé až 7 min pri ≈ 130 mA, spolu až ≈ 46 mAh za deň (zriedka). Kontrola: pri ≈ 15 Ah využiteľných z 19 Ah a 3,9 Ah ročne ≈ 3,6 roka.

**Oproti VLD2 opravené / zhoršené:** meranie prúdu 100 µA (vo VLD2 chybne 62 µA), meranie napätia počítané s maximom 41 mA (123 µA namiesto 91 µA), impulz 0,6 A (z LP) namiesto 0,5 A.

## 5 Vstup zariadenia

3,3 V znižovací menič (60 nA) a rádiový modul priamo z batérie; 3 × 100 µF keramika pri rádiu; funguje od 3,0 V, max. 4,2 V; zariadenie meria napätie batérie pod záťažou a posiela ho s dátami.

## 6 Teplota a prostredie

- Prevádzka **−40 … +70 °C**, impulzy aj pri −40 °C; správanie do **+85 °C** (krabica na slnku).
- Skladovanie pred montážou až 1 rok: odporúčané podmienky a skladovateľnosť náhradných packov.
- Vonku v uzavretej krabici (pack B: kovová s odvzdušňovacím ventilom), možná vlhkosť a kondenzácia.
- Vibrácie a otrasy; pack B pri železničnej trati (rámec EN 61373); pack v pene, poloha ľubovoľná.

## 7 Rozmery a pripojenie

- Pack A: priestor zatiaľ neurčený, ponúknuť rúrku aj vedľa seba s rozmermi a hmotnosťou.
- Pack B: max. 65 × 50 × 38 mm, max. 120 g.
- Balenie: zmršťovacia fólia, žiadne odhalené kontakty, vodiče na jednom konci, značenie podľa nariadenia EÚ o batériách.
- Vodiče: 2 ks, **150 ± 10 mm**, AWG 24 … 26, izolácia min. **+85 °C** (napr. UL1569 alebo UL1015, 105 °C).
- Konektor: **JST XHP-2** (rozstup 2,5 mm) s kontaktmi SXH, protikus JST B2B-XH-A na doske: **pin 1 = + (červený), pin 2 = − (čierny)**.

## 8 Zhoda a preprava

UN 38.3 (súhrn skúšok), IEC 60086-4, nariadenie EÚ 2023/1542 (prenosná batéria vymeniteľná na mieste: CE, značenie, vyhlásenie o zhode); karta bezpečnostných údajov; preprava samostatne (UN 3090) a v zariadení (UN 3091).

## 9 Množstvá

Prototypy 5 ks z každého packu; vzorky 20 ks z každého (Q1 2027); séria na začiatku 1 000 … 3 000 ks ročne z každého, s potenciálom výrazne vyšších objemov.

## 10 Čo od výrobcu potrebujeme

Odporúčaný pack pre profil A a B s dátovým listom a výkresom; využiteľnú kapacitu pri −40, +25 a +70 °C (do 3,2 V pri 0,6 A); napätie pri impulze a na konci spojenia pri −40, +20 a +70 °C (nový pack a koniec životnosti); pasiváciu po skladovaní a dlhom spánku pri −40 °C; samovybíjanie pri +25 a +70 °C, skladovanie, správanie do +85 °C; UN 38.3, SDS a podmienky prepravy; ceny pre 5 / 100 / 1 000 / 5 000 ks, Incoterms, dopravu a dodaciu lehotu vzoriek.

## Poznámky k zmenám (pre nás)

- **Vodiče 150 mm** namiesto 100 mm (podľa VLD2). Ponuky a výkresy Sunj sú na 100 mm, treba ich upraviť.
- **Izolácia vodičov:** Sunj na výkresoch používa UL1007, ktorá je podľa mojej znalosti dimenzovaná len na 80 °C. Pri požiadavke +85 °C treba iný vodič (napr. UL1569 alebo UL1015, 105 °C). Overiť.
- **Trvalý prúd 150 mA:** Honcell udáva pri svojom článku max. trvalý prúd 150 mA, čo je presne na hranici rádiového spojenia.
