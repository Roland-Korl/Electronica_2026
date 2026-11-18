# Porovnanie požiadaviek na batériu: EPS-BAT-LP vs. VLD2 FullMonitor

Dva podklady z rôznych pracovných relácií pre tie isté zariadenia:
- [EPS-BAT-LP, profily záťaže](2026-11_EPS-BAT-LP_profily-zataze_en_v1-0.pdf) (angl., [preklad](EPS-BAT-LP_profily-zataze_sk.md)): profil BAT-01 a BAT-02
- [VLD2 FullMonitor, batéria pre dodávateľa](2026-11-18_VLD2-FullMonitor_bateria-pre-dodavatela_sk.pdf) (slovensky, 18. 11. 2026)

Výpočty a závery nižšie sú moje, nie od výrobcu ani z podkladov.

## Pravdepodobné priradenie

| Zariadenie (podľa Rolanda) | Batéria | Životnosť | Najbližší podklad |
|---|---|---|---|
| Zariadenie 1 | 8,5 Ah + SPC | 10 rokov (6,7 Ah využiteľných) | EPS-BAT-LP, profil BAT-01 (≈ 34 µA) |
| Zariadenie 2 (VLD2 FullMonitor?) | 19 Ah + SPC | asi 3 roky | VLD2 (≈ 302 µA); profil BAT-02 v LP (≈ 161 µA) vyzerá ako staršia verzia toho istého |

Dôvod: VLD2 má rovnaké meranie napätia ako BAT-02 (≈ 29 mA, ≈ 2–3 ms, 1× za sekundu) a podobnú reláciu (≈ 130 mA, 56 s vs. 80 s), ale navyše meranie prúdu 10× za sekundu a dlhšiu reláciu. **Treba potvrdiť.**

## Rozdiely

| Parameter | EPS-BAT-LP (BAT-01 / BAT-02) | VLD2 FullMonitor | Čo sme už povedali Anne |
|---|---|---|---|
| Priemerný odber | 34 µA / 161 µA | **302 µA** | – |
| Impulz | do 0,6 A / 10 ms | do 0,5 A / 1–10 ms (zapnutie modemu 0,55 A < 1 ms) | 0,6 A / 10 ms |
| Min. napätie pri impulze | 3,0 V | **3,2 V** pri 0,5 A; **3,3 V** počas relácie LTE-M | – |
| Teplota prevádzky | −30 … +70 °C | **−40 … +70 °C**, správanie do +85 °C (kovová krabica na slnku) | „bežné európske počasie", −30 °C |
| Skladovanie | −40 … +85 °C | do 1 roka pred montážou, odporúčanie od dodávateľa | +85 °C (EPC1520 udáva len +60 °C) |
| Životnosť | 10 rokov / 3 roky | **≥ 2 roky (8,5 Ah), ≥ 4 roky (19 Ah)** pri 60 % využiteľnej kapacity | zar. 1: 10 rokov na 8,5 Ah; zar. 2: asi 3 roky na 19 Ah |
| Využiteľná kapacita v kalkulácii | – | 60 % | 6,7 Ah z 8,5 Ah (79 %) |
| Vodiče | 100 mm | **asi 150 mm**, izolácia do +85 °C | 100 mm (je v ponukách aj na výkresoch) |
| Konektor | – | JST XHP-2, pin 1 = + červený, pin 2 = − čierny | XH-2P, červený pin 1 (sedí) |
| Priestor | pôvodný (zaliaty / šachta) | **65 × 50 × 38 mm**, hmotnosť do 120 g | štandardné packy, rúrka aj vedľa seba |
| Prostredie | vonku | železnica, kovová krabica, vibrácie podľa EN 61373, možná kondenzácia | vonku, vodotesná krabička |
| Konkurencia v texte | – | spomína **EVE ES-261520/W** ako kandidáta | – |

## Ktoré packy Sunj sa zmestia do VLD2 (65 × 50 × 38 mm, do 120 g)

| Pack Sunj | Rozmery | Zmestí sa? |
|---|---|---|
| ER26500H + EPC1520, vedľa seba | 52 × 40 × 26 mm, ≈ 65 g | áno |
| ER34615H + EPC1520, vedľa seba | 63 × 48 mm, hrúbka nezakótovaná (článok Ø34,2), ≈ 120 g | pravdepodobne áno, **ak je hrúbka ≤ 38 mm**; hmotnosť na hranici |
| ER26500H + EPC1520, rúrka | 68 × Ø26 mm | nie (68 > 65 mm) |
| ER34615H + EPC1520, rúrka | 78 × Ø34 mm | nie (78 > 65 mm) |

Pre VLD2 teda pripadá do úvahy len verzia **vedľa seba**.

## Kontrola výpočtov vo VLD2

- **Meranie prúdu:** 5 mA × 2 ms × 10× za sekundu = **100 µA**, v tabuľke je **62 µA**. Ak platí 100 µA, celkový priemer je ≈ 340 µA namiesto 302 µA.
- Meranie napätia: 28,5 mA × 3 ms × 1× za sekundu = 85,5 µA, v tabuľke 91 µA (malý rozdiel, asi zaokrúhlenie alebo rezerva).
- Relácia LTE-M: 130 mA × 80 s raz denne = 120 µA, sedí. Udalosti ≈ 3,5 µA, sedí. Zápis údajov 6–10 µA, v tabuľke 13 µA (rezerva).
- **Dopad na životnosť pri 60 % využiteľnej kapacity:** pri 302 µA (2,65 Ah/rok) 1,9 roka (8,5 Ah) a 4,3 roka (19 Ah), ako je v PDF. Pri ≈ 340 µA (2,98 Ah/rok) **1,7 roka a 3,8 roka**, čiže pod cieľom 2 a 4 roky.
- Pri využiteľnej kapacite 79 % (ako pri zariadení 1) by to pri 302 µA bolo asi 2,5 a 5,7 roka.

## Odporúčanie pred odoslaním Anne

1. Potvrdiť priradenie: zariadenie 1 = profil BAT-01, zariadenie 2 = VLD2.
2. Opraviť alebo potvrdiť meranie prúdu (62 vs. 100 µA).
3. Pre Anne pripraviť **anglickú verziu VLD2 bez zmienky o EVE** a bez kapitoly 7 (externá batéria 12 V LiFePO4; Sunj také batérie podľa katalógu nevyrába).
4. Upozorniť Anne na zmeny oproti tomu, čo už vie: teplota −40 °C (a správanie do +85 °C), min. 3,2 V pri 0,5 A, vodiče asi 150 mm (ponuky sú na 100 mm), priestor 65 × 50 × 38 mm, hrúbka ER34615H packu vedľa seba ≤ 38 mm.
5. EPS-BAT-LP poslať len s profilom BAT-01 (pre zariadenie 1) a s poznámkou, že časti o priestore, zaliatí a kontaktoch neplatia.
