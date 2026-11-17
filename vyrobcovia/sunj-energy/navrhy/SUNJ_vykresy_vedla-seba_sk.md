# SUNJ: výkresy packov s kondenzátorom vedľa článku (preklad)

Originály (verzia A/0, kreslil WangBingle, Sunj Energy):
- [ER26500H + EPC1520](2026-11-17_sunj_vykres_ER26500H-EPC1520-vedla-seba.pdf)
- [ER34615H + EPC1520](2026-11-17_sunj_vykres_ER34615H-EPC1520-vedla-seba.pdf)

Obe riešenia majú **článok a kondenzátor EPC1520 položené vedľa seba**, takže sú podstatne kratšie než varianty z katalógu, kde je kondenzátor na článku.

## Rozmery

| | ER26500H + EPC1520 (8,5 Ah) | ER34615H + EPC1520 (19 Ah) |
|---|---|---|
| Dĺžka (výška článku) | max. **52 ± 1 mm** | max. **63 mm** |
| Šírka (článok + kondenzátor vedľa seba) | max. **40 ± 1 mm** | max. **48 mm** |
| Hrúbka (priemer článku) | max. **26 ± 1 mm** | **nie je na výkrese zakótovaná** (článok má podľa katalógu Ø34,2 mm) |
| Kábel | **100 ± 5 mm** | **100 ± 5 mm** |
| Porovnanie s katalógom (kondenzátor na článku) | Ø29 × 67 mm | Ø34 × 78 mm |

Pack s kondenzátorom vedľa článku je teda o 15 mm kratší pri 8,5 Ah (52 oproti 67 mm) a o 15 mm kratší pri 19 Ah (63 oproti 78 mm), ale širší (40 oproti Ø29 a 48 oproti Ø34).

## Zoznam súčiastok (preklad)

**ER26500H + EPC1520**

| Č. | Položka | Špecifikácia | ks |
|---|---|---|---|
| 1 | Batéria | ER26500H | 1 |
| 2 | Zvislá modrá fólia | OD 55 × 60 mm | 1 |
| 3 | Kondenzátor | EPC1520 | 1 |
| 4 | Vodorovná modrá fólia | sploštený priemer 75 × 49 mm (z čínskeho popisu „折径") | 1 |
| 5 | Izolačná podložka | kombinácia ER26 + 14 | 1 |
| 6 | Zmršťovacia bužírka | Ø2,5 × 0,1 × (8–10) mm | 1 |
| 7 | Červený izolovaný vodič | UL1007 24 AWG × 140 mm | 1 |
| 8 | Čierny izolovaný vodič | UL1007 24 AWG × 105 mm | 1 |
| 9 | Silikónová hadička | Ø2 × 0,5 × 10 mm | 2 |
| 10 | Kladná elektróda, paralelný niklovaný oceľový pásik | 3 × 0,08 × 25 mm | 1 |
| 11 | Záporná elektróda, paralelný niklovaný oceľový pásik | 3 × 0,08 × 50 mm | 1 |

**ER34615H + EPC1520**

| Č. | Položka | Špecifikácia | ks |
|---|---|---|---|
| 1 | Batéria | ER34615H | 1 |
| 2 | Záporná elektróda, paralelný niklovaný oceľový pásik | 3 × 0,1 × 62 mm | 1 |
| 3 | Zvislá modrá fólia | OD 65 × 70 mm | 1 |
| 4 | Vodorovná modrá fólia | OD 93 × 57 mm | 1 |
| 5 | Izolačná podložka | Ø34 + Ø14 | 1 |
| 6 | Kondenzátor | EPC1520 | 1 |
| 7 | Kladná elektróda, paralelný niklovaný oceľový pásik | 3 × 0,1 × 30 mm | 1 |
| 8 | Izolačná podložka | ER14 | 1 |
| 9 | Zmršťovacia bužírka | φ2,5 × 0,1 × (8–10) mm | 1 |
| 10 | Červený izolovaný vodič | UL1007 24 AWG × 140 mm | 1 |
| 11 | Čierny izolovaný vodič | UL1007 24 AWG × 105 mm | 1 |
| 12 | Silikónová hadička | Φ2 × 0,5 × 10 mm | 2 |

## Čo si na výkresoch všimnúť

- **Konektor nie je určený.** Pri ER26500H končia vodiče holými plochými koncovkami (bez puzdra konektora), pri ER34615H je na konci nakreslený malý konektor bez označenia typu. Treba výslovne požiadať o **puzdro XH-2P** (JST XH, rozstup 2,5 mm) s červeným vodičom (+) na pine 1 a čiernym (−) na pine 2.
- **Vodiče:** UL1007 24 AWG, červený 140 mm a čierny 105 mm v zozname, výsledná dĺžka kábla 100 ± 5 mm. Pri ER26500H sú vodiče skrútené.
- **Hrúbka ER34615H packu** na výkrese chýba; treba si ju vypýtať, kým navrhneš krabicu.
- Kondenzátor je pripojený paralelne k článku cez niklované pásiky; izolácia modrou fóliou a podložkami.
- Typy výkresov sú „Version A/0", teda prvá verzia.
