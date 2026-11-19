# Sunmoon ER26500 + HPC1520 a ER34615 + HPC1520: špecifikácie (preklad)

Výrobca článkov a kondenzátorov: **Wuhan Sunmoon Battery Co., Ltd.**, No. 231, Xingsan Road, Hannan District, Wuhan, Hubei, Čína, tel. +86-27-84732116 / 84730089, web www.voltec-sunmoon.com. Dodáva cez Unitek (distribútor).
Originály (angličtina): [ER26500 + HPC1520](2026-11-19_Sunmoon_ER26500-HPC1520_specifikacia_en.pdf) (1 strana), [ER34615 + HPC1520](2026-11-19_Sunmoon_ER34615-HPC1520_specifikacia_en.pdf) (2 strany).

## ER26500 + HPC1520 (pack A, 8,5 Ah)

Bobbin článok Li-SOCl2 ER26500 zapojený paralelne s hybridným impulzným kondenzátorom HPC1520.

| Parameter | Hodnota |
|---|---|
| Menovitá kapacita (3 mA, do 2 V) | 8,5 Ah |
| Menovité napätie | 3,6 V |
| Max. trvalý vybíjací prúd (článok) | **100 mA** |
| Max. pracovný impulzný prúd (článok) | 200 mA |
| Kapacita kondenzátora HPC1520 | 144 As (40 mAh) pri 3,67 V |
| Max. vybíjací prúd (pack) | 700 mA |
| Max. impulzný prúd | 2 000 mA |
| Pasivácia (oneskorenie napätia) | nie |
| Hmotnosť | ≤ 64 g |
| Prevádzková teplota | −40 až +85 °C |
| Rozmery (výkres) | **max. 51,5 × 41,2 mm** (článok a kondenzátor vedľa seba), kábel 100 ± 5 mm; hrúbka nezakótovaná (článok ≈ Ø26) |

Kapacita podľa prúdu pri +23 °C: 50 mA → 6,5 Ah; 10 mA → 7,0 Ah; 3 mA → 8,5 Ah; 1 mA → 8,3 Ah.

Grafy (odčítané približne z obrázka, nie presné):
- Napätie pri 1 s impulze v závislosti od teploty: pri **−40 °C** asi 3,0 V pri 100 mA, 2,9 V pri 200 mA a **2,4–2,5 V pri 500 mA**; nad 0 °C asi 3,4–3,5 V.
- Napätie kondenzátora pri impulze pri izbovej teplote: pri 500 mA asi 3,5 V na 10 ms.
- Obnoviteľná kapacita pri −30 °C výrazne klesá so stúpajúcim prúdom (asi 5–6 Ah pri 1 mA, asi 2 Ah pri 30 mA).

Výhody podľa výrobcu: vysoká hustota energie, stabilné vysoké napätie, široký rozsah teplôt, dlhá skladovateľnosť. Upozornenia: nevystavovať ohňu, nenabíjať, neskratovať, nerozoberať, nespaľovať, nezahrievať nad 100 °C, nepoužívať mimo povoleného rozsahu teplôt.

## ER34615 + HPC1520 (pack B, 19 Ah)

| Parameter | Hodnota |
|---|---|
| Kapacita do 2,5 V (250 mA, 1 % strieda) | 19 Ah |
| Menovité napätie | 3,6 V |
| Max. 1 s impulz do 2,5 V | **1 000 mA** |
| Max. dĺžka impulzu pri 125 mA do 2,5 V | 1 000 s |
| Oneskorenie do 3,0 V pri 125 mA | bez oneskorenia |
| Typická hmotnosť | **138 g** |
| Prevádzková teplota | −40 až +85 °C |
| Zachovanie kapacity po 10 rokoch | 95 % |
| Certifikácia | UL Component Recognition MH 29130; ISO 9001, UL, CE, RoHS |
| Rozmery | **v špecifikácii nie sú** |

Kapacita podľa prúdu pri +23 °C: 20 mA → 13,5 Ah; 5 mA → 18,0 Ah; 2 mA → 19,0 Ah; 0,3 mA → 18,2 Ah; 0,2 mA → 17,0 Ah.

Grafy (približne): pri 1 s impulze pri −40 °C asi 3,1 V pri 100 mA a **asi 2,5–2,6 V pri 500 mA**. Samovybíjanie rastie s teplotou (graf do 80 °C, typické a maximálne hodnoty).

## Porovnanie s našou špecifikáciou EPS-BAT-SPEC v2.0 (môj záver)

| Požiadavka | ER26500 + HPC1520 | ER34615 + HPC1520 |
|---|---|---|
| Trvalý prúd 150 mA až 7 min (rádiové spojenie) | článok len **100 mA**; zvyšok musí dodať kondenzátor (144 As); treba potvrdenie | max. impulz 125 mA na 1 000 s; **150 mA nie je potvrdené** |
| Impulz 0,6 A / 10 ms, min. 3,2 V pri −40 °C | pri 1 s a 500 mA pri −40 °C len asi 2,4–2,5 V; údaj pre 10 ms chýba | max. 1 s impulz 1 000 mA (Sunj udáva 2 000 mA); pri −40 °C a 500 mA asi 2,5 V pri 1 s |
| Priestor pack B 65 × 50 × 38 mm, max. 120 g | – | **138 g, nad limitom 120 g**; rozmery chýbajú |
| Pasivácia | „nie" | „bez oneskorenia" |
| Samovybíjanie max. 1 % ročne | neuvedené | 95 % po 10 rokoch, teda asi 0,5 % ročne |

Údaje pri 1 s impulze nie sú priamo porovnateľné s našimi 10 ms impulzmi (pri 10 ms bude napätie vyššie), ale ukazujú, že **nízka teplota je kritický bod**. Treba vypýtať údaje pre 10 ms pri −40 °C.
