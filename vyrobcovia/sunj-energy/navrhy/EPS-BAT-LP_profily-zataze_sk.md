# EPS-BAT-LP – profily záťaže batérie (preklad)

Preklad z angličtiny. Originál: [2026-11_EPS-BAT-LP_profily-zataze_en_v1-0.pdf](2026-11_EPS-BAT-LP_profily-zataze_en_v1-0.pdf) (verzia 1.0, 11/2026, 2 strany).
Vystavil: E.P.S. Germany GmbH · info@eps-de.com · +49 8442 639 2935

Prúdy, spotreba a teploty pre primárne batériové packy EPS-BAT-01 a EPS-BAT-02. Oba packy napájajú uzavreté, batériou napájané vonkajšie zariadenie s rádiovým modulom. Všetky hodnoty sú na svorkách packu. Pochádzajú z meraní na prototypových doskách a z nášho energetického modelu a budú potvrdené na prototypoch. Dopyty EPS-BAT-01 a EPS-BAT-02 určujú priestor a úplné požiadavky; tento list dopĺňa podrobnú záťaž.

## 1 Prehľad

| | EPS-BAT-01 – zaliaty pack | EPS-BAT-02 – výmenný pack |
|---|---|---|
| Chémia | Li-SOCl2 bobbin článok(y) + hybridný impulzný kondenzátor (HLC / SPC); veľkosť a usporiadanie na dodávateľovi | Li-SOCl2 bobbin článok + HLC / SPC, trieda ER26500 + SPC1520 (veľkosť C) |
| Použitie | úplne zaliaty v mäkkom 2K polyuretáne, nikdy sa nevymieňa | vymieňa ho technik, suchá tesná šachta, nezaliaty |
| Menovité napätie | 3,6 V | 3,6 V |
| Minimálne napätie | 3,0 V na svorkách počas všetkých impulzov, počas celej životnosti a až do −30 °C | rovnako |
| Priemerný prúd | ≈ 34 µA (0,81 mAh denne, 0,30 Ah ročne) | ≈ 161 µA (3,86 mAh denne, 1,41 Ah ročne); neskorší firmvér ≈ 115 µA |
| Najvyššia záťaž | rádiové spojenie ≈ 144 mA po dobu ≈ 17 s, s impulzmi do 0,6 A / 10 ms; každých 48 h | rádiové spojenie ≈ 56 s pri ≈ 106 … 131 mA, s impulzmi do 0,6 A / 10 ms; raz denne |
| Impulzy medzi spojeniami | ≈ 5 mA, ≈ 2 ms, 16 × za minútu | ≈ 30 mA, ≈ 2 ms, každú sekundu |
| Životnosť | min. 10 rokov v zariadení (≈ 3,4 Ah vrátane samovybíjania 1 %/rok) | jeden pack min. 3 roky, potom výmena (≈ 4,5 Ah vrátane 1 %/rok); skladovateľnosť náhradných packov min. 10 rokov |
| Kapacita | min. 4 Ah | min. 8 Ah |
| Teplota | prevádzka −30 … +70 °C (impulzy aj pri −30 °C), skladovanie −40 … +85 °C | rovnako |
| Priestor | kruhový odsek R 24,0 mm, rovná strana 47,4 mm, výška 20,3 mm, dĺžka ≤ 55 mm | Ø28 mm × 80 mm vrátane kontaktov, v šachte Ø30 mm |
| Pripojenie | 2 vodiče AWG 24–26 (bez silikónu), červený +, čierny −, skrútené, 100 mm, pocínované konce | ploché kontakty na vnútornom čele: + stred Ø ≥ 8 mm, − prstenec Ø14 … 21 mm; tlačené 2 pružinovými kontaktmi (≈ 1,5 N každý) |
| Prostredie | vonku, vibrácie a otrasy; zaliatie chráni pack | vonku, vibrácie a otrasy; pack drží veko cez penovú podložku (≈ 20 N) |
| Množstvá | vzorky 20 ks (Q1 2027), séria 1 000–3 000 ks ročne | vzorky 20 ks (Q1 2027), séria 1 000–3 000 ks ročne + náhradné packy |
| Zhoda | UN 38.3, nariadenie EÚ o batériách 2023/1542 | UN 38.3, IEC 60086-4, nariadenie EÚ 2023/1542 (vymeniteľný na mieste: CE, označenie); náhradné packy posielané samostatne (UN 3090) |

## 2 Vstup nášho zariadenia (oba packy)

| | |
|---|---|
| Elektronika | 3,3 V znižovací menič (pokojový prúd 60 nA) a rádiový modul priamo z batérie; medzi meraniami hlboký spánok |
| Ochrana vstupu | rýchla poistka 2 A, ochrana proti prepólovaniu (MOSFET) |
| Žiadne nabíjanie | dve nezávislé ideálne diódy v sérii blokujú akýkoľvek prúd do batérie (USB port sa používa len na stole, pred zaliatím) |
| Zásobník | 3 × 100 µF keramika na napájaní rádiového modulu (spolu s HLC pokryje vysielacie impulzy 10 ms) |
| Rozsah napätia | funguje od 3,0 V; max. 4,2 V na vstupe |
| Monitorovanie | zariadenie meria napätie batérie pod záťažou a posiela ho s dátami, takže správanie v teréne vieme zdieľať s dodávateľom |

## 3 Profil záťaže EPS-BAT-01 (zaliaty pack)

| Fáza | Prúd | Trvanie | Opakovanie | mAh / deň |
|---|---|---|---|---|
| Spánok (beží časovač) | 13,7 µA | trvalo | – | 0,329 |
| Meranie | ≈ 5 mA impulzy (16 × ≈ 2 ms) | spolu 35 ms | každých 60 s | 0,070 |
| Zápis dát do pamäte | ≈ 40 mA | ≈ 0,25 s | 6 × denne | 0,018 |
| Rádiové spojenie | ≈ 144 mA priemer, vysielacie impulzy do 0,6 A / ≈ 10 ms | ≈ 17 s | každých 48 h | 0,340 |
| Rádiové spojenie bez siete (zriedka, rezerva) | ≈ 37 mA priemer, impulzy do 0,6 A | až 300 s | ≈ 1 × za 2 mesiace | 0,052 |
| **Spolu** | **≈ 33,7 µA priemer** | | | **0,808** |

Meranie raz za minútu, dáta sa posielajú každých 48 h. Medzi fázami zariadenie spí.

## 4 Profil záťaže EPS-BAT-02 (výmenný pack)

| Fáza | Prúd | Trvanie | Opakovanie | mAh / deň |
|---|---|---|---|---|
| Spánok (beží časovač) | 11,4 µA | trvalo | – | 0,274 |
| Meranie | ≈ 29 mA na ≈ 1,6 ms, potom ≈ 5 mA na ≈ 1 ms | ≈ 2 ms | každú 1 s | 1,431 |
| Udalosť (zriedka): rovnaký merací impulz 10 × za sekundu | ako vyššie | ≈ 32 s | ≈ 10 × denne | 0,057 |
| Zápis dát do pamäte | ≈ 25 mA, potom ≈ 40 mA | ≈ 50 ms + 60 ms | každých 10 min | 0,149 |
| Rádiové spojenie | ≈ 106 mA na ≈ 10 s (sieť), potom ≈ 131 mA na ≈ 46 s (dáta); vysielacie impulzy do 0,6 A / ≈ 10 ms | ≈ 56 s | raz denne | 1,950 |
| Rádiové spojenie bez siete (zriedka) | ≈ 37 mA priemer, impulzy do 0,6 A | až 300 s | zriedka, nie je v priemere | – |
| **Spolu** | **≈ 160,9 µA priemer** | | | **3,861** |

Meranie každú sekundu, všetky hodnoty sa posielajú raz denne. Počas zriedkavej udalosti (predpoklad 10 × denne, ≈ 32 s) beží meranie 10 × za sekundu.

## 5 Prosíme o

- napätie na konci rádiového spojenia (najvyššia záťaž) pri −30 °C, +20 °C a +70 °C, pre nový pack a na konci životnosti;
- oneskorenie napätia (pasivácia) po skladovaní a po dlhých obdobiach spánku, a ako to rieši HLC;
- využiteľnú kapacitu pri našej záťaži a rozsahu teplôt, teda očakávanú životnosť;
- samovybíjanie za rok a skladovateľnosť náhradných packov (EPS-BAT-02);
- EPS-BAT-01: písomné potvrdenie, že úplné zaliatie v PU je prípustné, a čo potrebuje bezpečnostný ventil;
- EPS-BAT-02: výkres kontaktnej strany, ochranu proti skratu (poistka / PTC) a prepravný kryt;
- ceny pre 100 / 1 000 / 5 000 ks a dodaciu lehotu vzoriek.

Polia na vyplnenie výrobcom: „Výrobca batérií / kontakt", „Poznámky".

## Poznámky k prekladu

- *Passivation / voltage delay* = pasivácia, oneskorenie napätia: pri článkoch Li-SOCl2 po dlhom kľude chvíľu klesne napätie pri prvom zaťažení.
- *Ideal diode* = ideálna dióda (obvod s MOSFET, ktorý sa správa ako dióda s veľmi malým úbytkom napätia).
