# 2026-11-17 – Anne (Sunj Energy): ER26500H + EPC1520, kabeláž a konektor

- **Typ:** chat (WhatsApp)
- **Smer:** prijaté
- **S kým:** Anne, Sunj Energy (+86 133 3379 5798)
- **Čas správ:** 09:05–09:08 (druhá konverzácia toho istého dňa, nadväzuje na [rannú](2026-11-17_whatsapp_anne-vyhodnocuje-pack.md))
- **Zdroj:** prekopírovaný text správ (bez snímky)

## Zhrnutie

Anne napísala, že nám práve poslala aj e-mail, a pýta sa, či sme ho dostali. Zároveň sa pýta, či chceme len batériový pack zložený z článku **ER26500H** a hybridného kondenzátora **EPC1520**, a upozorňuje, že takéto packy sa bežne dodávajú **s káblami a konektormi** na pripojenie k zariadeniu zákazníka. Teda reaguje na našu správu o prechode na štandardné batérie.

## Dohodnuté kroky

- [x] Firemný e-mail od Anne prečítaný, v poriadku (Roland). Obsah do repa zatiaľ nezapísaný.
- [ ] Odpovedať Anne (návrh nižšie).
- [x] Rozhodnuté (Roland): nová verzia zariadenia je **krabica namiesto rúrky**, navrhnutá na štandardný pack s káblom a konektorom. Dopyty BAT-01 a BAT-02 už neplatia.

## Pôvodný text (originál)

> Hello Roland, good morning😊 (09:05)
> I just sent you an email as well—did you receive it? (09:06)
> Do you mean that you only require the battery pack consisting of an ER26500H and an EPC1520? Typically, such battery packs need to be equipped with cables and connectors to connect to the customer's equipment. (09:08)

## Preklad do slovenčiny

> Dobrý deň, Roland, pekné ráno 😊
> Práve som vám poslala aj e-mail, dostali ste ho?
> Myslíte tým, že potrebujete len batériový pack zložený z ER26500H a EPC1520? Takéto batériové packy sa zvyčajne dodávajú s káblami a konektormi na pripojenie k zariadeniu zákazníka.

## Výkres od Sunj Energy

Prišiel ešte ten istý deň (kanál neuvedený, text hore na výkrese je orezaný). Súbor: [výkres packu](../navrhy/2026-11-17_sunj_vykres-pack-kabel-konektor.jpg).

Na výkrese je štandardný pack s dvoma vodičmi (červený +, čierny −) zakončenými konektorom, vo dvoch variantoch:
- ľavá strana: max. Ø27 mm, dĺžka max. **68 mm**
- pravá strana: max. Ø27 mm, dĺžka max. **65 mm**
- na hornom konci packu je plastové zakončenie s vyvedenými vodičmi; zospodu je vidieť kontaktnú dosku

Z tohto výkresu neviem prečítať: dĺžku kábla (je prerušená značkou), typ konektora, kapacitu ani rozdiel medzi oboma variantmi.

**Druhý výkres** (Anne poslala medzitým): [výkres packu 67 mm, kábel 100 mm](../navrhy/2026-11-17_sunj_vykres-pack-67mm-kabel-100mm.jpg).
- max. **Ø27 mm × max. 67 mm**
- dĺžka kábla **100 ± 5 mm** (čiže na prvú otázku o dĺžke kábla je odpoveď)
- červený + čierny vodič, na konci konektor (položka 9)
- jednotlivé časti sú očíslované 1–11, ale **zoznam položiek (legenda) na výkrese nie je**. Z tvaru odhadujem: 1 = článok, 9 = konektor, 7 a 8 = vodiče, 6 = nejaký prvok na vodiči (možno poistka alebo PTC). Ostatné nepoznám. Treba vypýtať legendu.

Anne teda poslala výkresy v troch dĺžkach: **65, 67 a 68 mm**. Treba zistiť, ktorá je štandardná a prečo sú tri.

**Porovnanie s našou šachtou (EPS-BAT-02):** šachta Ø30 mm, pack max. Ø28 × 80 mm. Pack Ø27 × 65–68 mm sa rozmerovo zmestí. Prekáža len kábel a konektor: v pôvodnom návrhu sú pružinové kontakty na dne šachty a pack žiadne vodiče nemá.

**E-mail:** Roland potvrdil, že e-mail od Anne dostal a je v poriadku; v komunikácii môžeme pokračovať na WhatsAppe.

## Poznámky

- **ER26500H** je pravdepodobne vysokovýkonná verzia článku ER26500 (veľkosť C, Li-SOCl2); význam „H" nepoznám s istotou, treba overiť v dátovom liste.
- **EPC1520** používa Anne; v našom dopyte (EPS-BAT-02) sme písali „SPC1520". Pravdepodobne ide o ten istý typ pod iným označením výrobcu, treba potvrdiť.
- **Káble a konektor:** náš dopyt EPS-BAT-02 výslovne žiadal pack **bez káblov a bez konektora** (ploché kontakty na čele, výmena v šachte). Štandardný pack sa dodáva s káblom a konektorom, takže by sme museli prispôsobiť upevnenie a pripojenie v zariadení. Ak sa pack zalieva (BAT-01), káble sú naopak v poriadku.

## Návrh odpovede

**Po anglicky (na odoslanie):**

> Hello Anne, yes, I received your email, thank you. We can continue here on WhatsApp.
>
> To clarify: yes, we only need your standard battery pack with an ER26500H cell and an EPC1520 capacitor. We now have a new version of our device. It is a box instead of a tube, designed so that your standard pack, with cable and connector, fits inside. So we do not need any custom pack anymore, and our earlier requests EPS-BAT-01 and EPS-BAT-02 are no longer valid.
>
> Thank you for the drawings. To finish our design, could you please send me:
> 1. the datasheet of the pack
> 2. the connector type (and the mating connector)
> 3. you sent drawings with 65, 67 and 68 mm length: what is the difference, and which one is your standard?
> 4. the parts list for the numbers 1–11 on the 67 mm drawing
> 5. the price for 100 / 1,000 / 5,000 pieces
> 6. the delivery time for 20 samples
> 7. the capacity, and the voltage during 0.6 A pulses (10 ms) at −30 °C
>
> Thank you very much!

**Po slovensky (význam):**

> Dobrý deň, Anne, áno, e-mail som dostal, ďakujem. Môžeme pokračovať tu na WhatsAppe.
>
> Upresnenie: áno, potrebujeme len váš štandardný batériový pack s článkom ER26500H a kondenzátorom EPC1520. Máme novú verziu zariadenia. Je to krabica namiesto rúrky, navrhnutá tak, aby sa do nej zmestil váš štandardný pack s káblom a konektorom. Vlastný pack na mieru už teda nepotrebujeme a naše predchádzajúce dopyty EPS-BAT-01 a EPS-BAT-02 už neplatia.
>
> Ďakujem za výkresy. Aby sme dokončili návrh, pošlite mi, prosím:
> 1. dátový list packu
> 2. typ konektora (aj protikus)
> 3. poslali ste výkresy s dĺžkou 65, 67 a 68 mm: aký je rozdiel a ktorý je váš štandard?
> 4. zoznam položiek k číslam 1–11 na výkrese so 67 mm
> 5. cenu pre 100 / 1 000 / 5 000 ks
> 6. dodaciu lehotu pre 20 vzoriek
> 7. kapacitu a napätie počas impulzov 0,6 A (10 ms) pri −30 °C
>
> Veľmi pekne ďakujem!
