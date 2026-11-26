# 2026-11-26 – e-mail od Jerryho Zhu (Raicky): výkresy konektora M12 X a kábla M12 X – RJ45

- **Typ:** email
- **Smer:** prijaté
- **Od:** Jerry Zhu (szzrk@raicky.com)
- **Prílohy:** [zásuvka M12 X do dosky, 120708-04-049 rev. S2](../navrhy/2026-11-26_raicky_vykres_120708-04-049_M12-X-zasuvka-PCB_S2.pdf) (2 strany), [kábel M12 X – RJ45, 2607021-X-2433](../navrhy/2026-11-26_raicky_vykres_2607021-X-2433_kabel-M12-X-RJ45.pdf)

## Pôvodný text (originál)

> Dear Mr. Korl
> Hello! It's great to receive your reply!
> Both items are M12 connectors: the first one is an M12 X-coded connector, and the second is an M12 X-coded male to RJ45 CAT6A cable. I have attached the specification drawings for both products we are currently working on. Please review them to see if they meet your requirements. Let's confirm the relevant dimensions on the drawings first before we discuss the pricing. Thank you

## Preklad do slovenčiny

> Vážený pán Korl, dobrý deň! Teším sa z vašej odpovede!
> Obe položky sú konektory M12: prvá je konektor M12 s kódovaním X, druhá je kábel M12 X (vidlica) na RJ45 CAT6A. Prikladám výkresy oboch produktov, na ktorých práve pracujeme. Pozrite si, prosím, či spĺňajú vaše požiadavky. Najprv si potvrďme rozmery na výkresoch a potom sa budeme baviť o cene. Ďakujem.

## Výkres 1: zásuvka M12 X do dosky (Raicky 120708-04-049, rev. S2 z 29. 10. 2025)

**M12 X-coding 8pin female PCB connector**: 8-pinová zásuvka M12 s kódovaním X do dosky plošných spojov, **zahnutá o 90°**, montáž do panelu maticou.

| | |
|---|---|
| Závit | M12 × 1,0 |
| Rozmery | čelo Ø16,5 mm, kľúč SW15 (matica SW14), výška 19,2 mm, hĺbka 30 mm, šírka 15 mm, vzdialenosť osi od dosky 8,5 mm |
| Výrez v paneli (odporúčaný) | Ø12,1 ± 0,05 mm so zrezanou stranou 10,6 ± 0,05 mm (tvar D) |
| Doska (odporúčané) | 8 otvorov Ø0,9 mm pre piny, 2 otvory Ø2,05 mm a 2 Ø2,8 mm; blokovaná plocha 16 × 15 mm |
| Diely | konektor M12 X 8-pin, O-krúžok HNBR Ø8 × 1,3 mm, plášť zo zinkovej zliatiny poniklovaný (M12 × 1), O-krúžok HNBR Ø11,5 × 1,6 mm, kovová matica Ø15 × 2 mm (SW14), poniklovaná mosadzná krytka proti prachu |
| Elektrické | menovité napätie 50 V AC / 60 V DC, izolačný odpor > 100 MΩ, menovitý prúd 0,5 A, prechodový odpor ≤ 5 mΩ |
| Mechanické | > 100 zasunutí |
| Ukončenie | v texte „SMT", ale podľa výkresu má **piny do otvorov (THT)** |
| Teplota | **−25 až +85 °C** |
| Ostatné | všetky materiály RoHS |

**Neuvedené:** krytie IP, kategória Cat6A / rýchlosť 10 Gbit/s.

## Výkres 2: kábel M12 X (vidlica) – RJ45 (Raicky 120708-57-39x, projekt RKY2607021, z 25. 7. 2026)

| | |
|---|---|
| Strana P1 | **M12 X-kódovaná vidlica, 8 pinov, tienená**, Ø14,5 mm, dĺžka 47,5 mm (orientačne) |
| Strana P2 | **RJ45 8P8C vidlica, Cat7, tienená**, dĺžka 46,6 mm (orientačne) |
| Kábel | **SFTP Cat6A 26 AWG, 4 páry + oplet**, plášť **PU tmavozelený**, Ø6,2 mm |
| Dĺžky | 120708-57-391: **2 000 ± 20 mm**; 120708-57-392: **5 000 ± 50 mm** |
| Elektrické | 30 V, 0,5 A |
| Krytie | **IP67** (na strane M12) |
| Teplota | **−25 až +80 °C** (závisí od kvality kábla) |
| Mechanické | > 100 zasunutí, utahovací moment 0,4–1,6 Nm, odolnosť spoja konektor–zálievka 5,0 kgf, stupeň znečistenia 3 |

Zapojenie (M12 → RJ45): 1→1 (biely), 2→2 (oranžový), 3→3 (biely), 4→6 (zelený), 5→7 (biely), 6→8 (hnedý), 7→5 (biely), 8→4 (modrý), plášť → oplet → plášť. Páry zodpovedajú zapojeniu RJ45 podľa T568B (môj záver, overiť s vaším zapojením).

## Poznámky (môj záver)

- **Výkresy sú z inej firmy:** v rohoch výkresov je web sz-signal.com a text „majetok SIGNAL COMPANY". Raicky je teda zrejme sprostredkovateľ, nie výrobca.
- **Nie je to originál Amphenol LTW MSXS-08PFFR-SF7003**, ale čínska náhrada. Treba porovnať rozmery, výrez v paneli a rozloženie pinov na doske s Amphenolom (dátový list Amphenolu tu nemám, stránky nie sú dostupné).
- **Rozpor pri zásuvke:** text „Termination: SMT" vs. výkres s pinmi do otvorov.
- **Chýba** krytie IP a údaj o Cat6A / 10 Gbit pri zásuvke; pri kábli je Cat6A len pri samotnom kábli, konektor RJ45 je Cat7.
- **Teplota −25 °C:** ak je prepäťová ochrana vonku, môže to byť málo (naše batériové zariadenia počítajú s −40 °C).
- Ceny zatiaľ nie sú; Jerry chce najprv potvrdiť rozmery.
