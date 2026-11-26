# Porovnanie: zásuvka M12 X Raicky 120708-04-049 vs. Amphenol LTW MSXS-08PFFR-SF7003

Podklady:
- Amphenol LTW: [výkres MSXS-XXPFFR-SF7003, rev. K z 5. 11. 2025](../dokumenty/Amphenol-LTW_MSXS-XXPFFR-SF7003_vykres_revK.pdf) („N SEN, M12 X-SHLD, SCREW RECEPTACLE, F, F, PCB R" = zásuvka M12 X, tienená, so závitom, do dosky, zahnutá)
- Raicky: [výkres 120708-04-049, rev. S2 z 29. 10. 2025](2026-11-26_raicky_vykres_120708-04-049_M12-X-zasuvka-PCB_S2.pdf) (výkres firmy Signal)

Porovnanie som robil z výkresov (obrázkov); je to môj záver, nie potvrdenie výrobcu.

## Rozmery a montáž

| Parameter | Amphenol MSXS-08PFFR-SF7003 | Raicky 120708-04-049 | Zhoda |
|---|---|---|---|
| Typ | M12 X, 8 pinov, zásuvka, tienená, do dosky 90°, montáž do panelu maticou | M12 X, 8 pinov, zásuvka, do dosky 90°, montáž do panelu maticou | áno |
| Závit | M12 × 1,0 | M12 × 1,0 | áno |
| Výrez v paneli | Ø12,10 (+0,10) so zrezanou stranou 10,60 (+0,10) | Ø12,1 ± 0,05 so zrezanou stranou 10,6 ± 0,05 | áno |
| Šesťhran / čelo | 15,0 / Ø16,5 | SW15 / Ø16,5 | áno |
| Výška osi nad doskou | 8,5 | 8,5 | áno |
| Celková dĺžka | 28,7 (orientačne) | 30,0 | Raicky o 1,3 mm dlhší |
| Hrúbka panelu | 1,0–4,0 mm | neuvedená | **overiť** |
| Hrúbka dosky | 1,6–2,4 mm | neuvedená | **overiť** |
| Panel – prvý rad otvorov / hrana dosky | 4,30 / hrana dosky max. 3,80 od panelu | v rozložení dosky nezakótované presne | **overiť** |

## Rozloženie na doske (footprint)

| Parameter | Amphenol | Raicky | Zhoda |
|---|---|---|---|
| Rastrové rozmery | 12,00 / 5,60 / 2,80 / 3,65 | 12,0 / 5,6 / 2,8 / 3,65 | áno |
| Otvory pre piny | 9 × Ø1,10 (8 pinov + stred) | 8 × Ø0,9 + stred Ø1,10; piny Ø0,78 | Raicky piny sa zmestia do otvorov Ø1,10 (väčšia vôľa) |
| Otvory pre kolíky | 2 × Ø2,10 | 2 × Ø2,05; kolíky Ø2,0 | áno, kolíky sa zmestia |
| Veľké otvory | 2 × Ø2,80 | 2 × Ø2,8 | áno |
| Číslovanie pinov | v „Pin Definition", panel vľavo | v rozložení dosky, panel dole, v čelnom pohľade bez čísel | **overiť**, orientácia výkresov je iná |

## Vlastnosti

| Parameter | Amphenol | Raicky |
|---|---|---|
| Krytie | **IP67 po zasunutí** | neuvedené |
| Telo | termoplast čierny | plášť zo zinkovej zliatiny, poniklovaný |
| Piny | zliatina medi, **pozlátené** | materiál a pokovenie neuvedené |
| Tienenie | kovové | (plášť kovový) |
| O-krúžky | guma sivá | HNBR čierne |
| Elektrické údaje | na výkrese neuvedené | 50 V AC / 60 V DC, 0,5 A, > 100 MΩ, ≤ 5 mΩ |
| Teplota | na výkrese neuvedená | −25 až +85 °C |
| Cat6A / 10 Gbit | na výkrese neuvedené (séria X je na to určená) | neuvedené |
| Ukončenie | piny do otvorov (THT) | text „SMT", výkres THT |
| Ostatné | RoHS; matica balená zvlášť | RoHS; mosadzná krytka proti prachu |

## Záver

- **Mechanicky je Raicky veľmi blízka náhrada:** rovnaký výrez v paneli, rovnaký raster otvorov na doske a rovnaká výška osi. Na existujúcu dosku navrhnutú pre Amphenol by sa mala dať osadiť (piny Ø0,78 do otvorov Ø1,10).
- **Treba overiť pred objednávkou série:** číslovanie pinov (rovnaké zapojenie), vzdialenosť panel – doska a hrúbku panelu, krytie IP67, pokovenie pinov (zlato), vhodnosť pre 10 Gbit (merania Cat6A).
- **Odporúčanie:** objednať 10 ks vzoriek a skúsiť ich osadiť na vašu dosku a do krabice, otestovať 10 Gbit prenos a tesnosť.
