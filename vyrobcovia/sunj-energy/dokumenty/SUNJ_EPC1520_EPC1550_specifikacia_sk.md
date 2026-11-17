# SUNJ EPC1520 a EPC1550: špecifikácia kondenzátorov (preklad)

Originály (angličtina, 4 strany každý):
- [2026-11-17_SUNJ_EPC1520_specifikacia_en.pdf](2026-11-17_SUNJ_EPC1520_specifikacia_en.pdf)
- [2026-11-17_SUNJ_EPC1550_specifikacia_en.pdf](2026-11-17_SUNJ_EPC1550_specifikacia_en.pdf)

Produkt: **super impulzný kompozitný kondenzátor** (Super pulse composite capacitance). Vydal SUNJ Energy (Luoyang) Co., Ltd.

## Porovnanie

| Parameter | EPC1520 | EPC1550 |
|---|---|---|
| Max. rozmer | Ø15,1 × 21,0 mm | Ø15,1 × 50,5 mm |
| Hmotnosť | asi 10,0 g | asi 21,0 g |
| Napätie naprázdno | ≥ 3,64 V | ≥ 3,64 V |
| Vnútorný odpor (RT, 1 kHz) | ≤ 200 mΩ | ≤ 100 mΩ |
| Kapacita | 140 As pri 3,67 V; 210 As pri 3,90 V | 560 As pri 3,67 V; 850 As pri 3,90 V |
| Koncové napätie vybíjania | 2,5 V | 2,5 V |
| Max. trvalý vybíjací prúd | 0,5 A | 2,0 A |
| Max. impulz (1 s) | 2,0 A | 5,0 A |
| Max. nabíjacie napätie | 3,95 V | 3,95 V |
| Max. nabíjací prúd | 100 mA | 500 mA |
| **Zvodový prúd pri izbovej teplote** (spolu so článkom ER) | **0,1 µA** | **3,0 µA** |
| **Zvodový prúd pri +80 °C** | 5,0 µA | 15,0 µA |
| Prevádzková teplota | −40 až +85 °C | −40 až +85 °C |
| Skladovacia teplota | −40 až +60 °C | −40 až +60 °C |

Poznámka k vybíjaniu: pri vybíjaní na 2,5 V pri izbovej teplote alebo na 2,0 V pri −40 °C môže vzrásť vnútorný odpor kondenzátora.

## Skladovateľnosť

| Teplota | Kondenzátor samostatne | Kombinácia ER + EPC |
|---|---|---|
| izbová | 3 roky | **10 rokov** |
| +60 °C | 4 týždne | 7 rokov |
| +80 °C | 1 týždeň | viac než 1 rok |

## Životnosť pri cyklovaní (do 80 % pôvodnej reverzibilnej kapacity)

Pri nabíjaní na 3,67 V: 1 000 cyklov pri 100 % hĺbke vybitia (DOD), 10 000 cyklov pri 10 % DOD, 100 000 cyklov pri 1 % DOD.

## Bezpečnostné skúšky a súlad

Skrat (pri izbovej teplote a +55 °C), tepelná záťaž 130 °C, prebíjanie (200 %, 0,2 A) a hlboké vybitie, stlačenie, prepichnutie, tepelný šok, voľný pád, mechanický šok a vibrácie. Zodpovedá **UL1642 a IEC 60086**, obsah lítia je **menej než 0,1 g**.

## Grafy

Krivky vybíjania pri rôznych teplotách (EPC1520: 200 mA a 350 mA; EPC1550: 500 mA a 1 000 mA) a závislosť kapacity od napätia sú v PDF (strany 2 a 3). V preklade ich neuvádzam, lebo hodnoty z obrázka nedokážem presne prečítať.

## Čo to znamená pre nás (môj záver, nie údaj výrobcu)

- Naše impulzy sú pri komunikácii 0,6 A po dobu 10 ms. **EPC1520 má povolených 2 A impulz (1 s) pri odpore ≤ 200 mΩ**, čo by malo stačiť s rezervou. Úbytok napätia pri 0,6 A je pri izbovej teplote asi 0,12 V (0,6 A × 0,2 Ω); pri −30 °C bude odpor vyšší, preto treba údaj od Sunj.
- **EPC1550 má 30× väčší zvodový prúd** (3,0 µA oproti 0,1 µA). Pri 3,0 µA je to za 10 rokov asi 0,26 Ah (3 µA × 24 × 365 × 10 h), čo je pri 8,5 Ah asi 3 % kapacity. Samotné číslo nie je veľké, ale zbytočne ju berie; EPC1550 sa oplatí len ak by sme potrebovali väčšie impulzy než 2 A.
- Skladovacia teplota je tu −40 až +60 °C, náš pôvodný dopyt chcel −40 až +85 °C. Ak je to dôležité, treba sa opýtať.
