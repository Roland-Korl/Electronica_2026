# tekmodul (antény)

| | |
|---|---|
| **Stav** | ponuka |
| **Web** | www.tekmodul.de |
| **Krajina / mesto** | Nemecko, München |
| **Stretli sme sa** | Electronica 2026, Mníchov, stánok tekmodul (rozhovor kolegu p. Antala s p. Mosandlom) |
| **Ďalší krok** | odpovedať (preberá Roland), upresniť pásma LTE-M a vypýtať vzorky a ponuku |
| **Termín** | doplniť |

Typ firmy: distribútor (nie výrobca), technický predaj.

## Kontaktné osoby

| Meno | Rola | E-mail | Telefón | Poznámka |
|---|---|---|---|---|
| Peter Heinisch | Technischer Vertrieb Nord (technický predaj Sever) | p.heinisch@tekmodul.de | +49 89 90411829-16, mobil +49 160 4065225 | tekmodul GmbH, Lindwurmstr. 97a, 80337 München |
| p. Mosandl | kolega p. Heinischa (stánok na veľtrhu) | neznámy | neznámy | |

Na strane EPS: pôvodne kolega p. Antal, teraz preberá **Roland Korl (vedúci IT oddelenia)**.

## Čo nás zaujíma

- **Antény pre modem LTE-M** (Cat-M1) vo vonkajších zariadeniach.
- Diskutovaná anténa: **Taoglas FXUB63** 5G/4G Flex, kábel 150 mm, Ø1,37 mm, konektor I-PEX MHF I (U.FL).
- Navrhnutá alternatíva: **Synzen (SP Technologies) ELNATH SZK-C-5L36**, FPC anténa 42,5 × 15 mm, rovnaký frekvenčný rozsah ([produkt](https://synzen.com.tw/products/elnath)).
- Pozor: zariadenie s packom B (VLD2) je v **kovovej** krabici; vnútorná anténa tam nebude fungovať, treba vonkajšiu.

## Obchodné podmienky

- Cena / cenník ([ponuka TM105075](navrhy/2026-11-25_tekmodul_ponuka_TM105075.pdf), USD bez DPH, platí do 24. 12. 2026): ELNATH 2,22 / 2,00 / 1,26; LALANDE 2,57 / 2,07 / 1,36; TARVOS 5,65 / 3,22 / 2,42; pigtail SMA–MHF1 100 mm 1,90 / 1,60 / 1,14 (100 / 1 000 / 5 000 ks). Vzorky po 5 ks ELNATH, LALANDE, TARVOS.
- MOQ (min. množstvo): zatiaľ nie
- Dodacia lehota: zatiaľ nie
- Platobné podmienky: splatnosť 30 dní; poštovné 17,80 USD (Európa) / 11,50 USD (Nemecko) za dodávku
- Exkluzivita / distribúcia: zatiaľ nie

## Zhrnutie rokovania

- 2026-11-26: vzor NDA Synzen (taiwanské právo), dátový list TARVOS (195 × Ø13 mm, −30 až +65 °C), podklady na testy: krabica, osadená doska, typ batérie; vzorky v 1. januárovom týždni ([záznam](komunikacia/2026-11-26_email_heinisch-nda-tarvos.md)).
- 2026-11-25: ponuka TM105075; Synzen odporúča ELNATH a TARVOS a ponúka bezplatné testy antén v našom dizajne ([záznam](komunikacia/2026-11-25_email_heinisch-ponuka-TM105075.md)).
- 2026-11-24: Taoglas nepredávajú; navrhujú Synzen LALANDE (FPC, MHF1) a CALLISTO1 / TARVOS (vonkajšie, SMA) plus pigtaily; vzorky LALANDE a CALLISTO hneď ([záznam](komunikacia/2026-11-24_email_heinisch-lalande-callisto.md)).
- 2026-11-23: p. Heinisch ďakuje za návštevu, navrhuje ELNATH ako alternatívu k FXUB63, ponúka vzorky a ponuku, pýta sa na frekvenčný rozsah ([záznam](komunikacia/2026-11-23_email_heinisch-anteny.md)).

## Otvorené otázky

- [ ] Aký modem LTE-M použijeme a aké pásma (podľa mojej znalosti v Nemecku hlavne B20, B8, prípadne B3)?
- [ ] Riešenie antény pre kovovú krabicu: vonkajšia anténa so SMA (CALLISTO1 / TARVOS) + pigtail z U.FL na stenu krabice; upresniť rozmer antény a dĺžku pigtailu.
- [x] Konektor MHF1 (U.FL); FPC max. ako FXUB63; vonkajšia anténa čo najmenšia (ideálne ako minca 2 €) na hliníkovú krabicu; pigtail do 150 mm.
- [x] Ponuka pre 100 / 1 000 / 5 000 ks (TM105075).
- [ ] Potvrdiť vzorky (ELNATH, LALANDE, TARVOS po 5 ks) a doplniť 5 pigtailov.
- [x] Rozmer TARVOS: 195 × Ø13 mm, prevádzka len −30 až +65 °C (nevyhovuje); vypýtať menšiu vonkajšiu anténu do −40 °C.
- [ ] Konektor ELNATH (MHFa1 alebo MHF1 / U.FL?).
- [ ] NDA: rozhodnúť (vzor Synzen s taiwanským právom alebo vlastná NDA), zahrnúť tekmodul, podpis konateľom.
- [ ] Pripraviť na testy krabicu, osadenú dosku, typ a umiestnenie batérie.
- [ ] Prijať bezplatné testy Synzen; zistiť, čo potrebujú (krabica, doska), zvážiť NDA.
