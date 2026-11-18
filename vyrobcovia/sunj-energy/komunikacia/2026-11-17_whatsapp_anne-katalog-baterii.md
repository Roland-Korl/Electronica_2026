# 2026-11-17 – Anne (Sunj Energy): katalóg batérií a kondenzátorov

- **Typ:** chat (WhatsApp)
- **Smer:** prijaté
- **S kým:** Anne, Sunj Energy
- **Čas správ:** 10:02–10:03
- **Prílohy:**
  - [katalóg produktov (PDF, 24 strán)](../dokumenty/2026-11-17_SUNJ_katalog-produktov_en.pdf) · [výber a preklad](../dokumenty/SUNJ_katalog_vyber_sk.md)
  - [EPC1520, špecifikácia](../dokumenty/2026-11-17_SUNJ_EPC1520_specifikacia_en.pdf) a [EPC1550, špecifikácia](../dokumenty/2026-11-17_SUNJ_EPC1550_specifikacia_en.pdf) · [preklad](../dokumenty/SUNJ_EPC1520_EPC1550_specifikacia_sk.md)
  - [tabuľka H-rady (obrázok)](../dokumenty/2026-11-17_SUNJ_tabulka-rada-ER-H.jpg)

## Pôvodný text (originál)

> This is the information regarding our battery models. (10:02)
> They can all be combined with capacitors. (10:03)

## Preklad do slovenčiny

> Toto sú informácie o našich modeloch batérií.
> Všetky sa dajú kombinovať s kondenzátormi.

## Zhrnutie

Anne odpovedala na našu žiadosť o zoznam všetkých batérií Li-SOCl2 so SPC. Poslala katalóg, špecifikácie kondenzátorov EPC1520 a EPC1550 a tabuľku H-rady (vysoká kapacita). Z katalógu vyplýva, že majú aj **hotové kombinované packy** s rozmermi, a tie odpovedajú na naše otázky.

## Čo z toho vyplýva (podrobne v preklade katalógu)

Naše dve aplikácie, hotové kombinácie z katalógu (strana 20):

| | Kondenzátor na článku (dlhší, užší) | Kondenzátor vedľa článku (kratší, širší) |
|---|---|---|
| **8,5 Ah** | ER26500H + EPC1520: **Ø29,0 × 67,0 mm**, impulz 2 A | ER26500H + EPC1550: **55 × 44 × 28 mm**, impulz 5 A |
| **19 Ah** | ER34615H + EPC1520: **Ø34,0 × 78,0 mm**, impulz 2 A | ER34615H + EPC1550: **64 × 55 × 35 mm**, impulz 5 A |

- **Rozmery ER34615H packu**, ktoré chýbali v špecifikácii, sú v katalógu: Ø34,0 × 78,0 mm (s EPC1520).
- Verzia s kondenzátorom vedľa článku je v katalógu len s väčším EPC1550. Verziu **EPC1520 vedľa článku** Anne sľúbila ako výkres (správa 09:56).
- **EPC1550 má 30× väčší zvodový prúd** než EPC1520 (3,0 µA oproti 0,1 µA). Pri našich impulzoch 0,6 A × 10 ms stačí podľa špecifikácie EPC1520 (impulz do 2 A).
- Katalóg obsahuje aj H-radu (vysoká kapacita, vhodná pre nás) a M-radu (vysoký výkon, nižšia kapacita), ďalšie články ER14250H–ER341245H a kondenzátor EPC1530.

## Dohodnuté kroky

- [ ] Vybrať varianty (Roland) a vypýtať ceny pre 100 / 1 000 / 5 000 ks.
- [ ] Počkať na výkres EPC1520 vedľa článku.
- [ ] Odpovedať na predchádzajúce otázky Anne (konektor XH-2P, impulzy, adresa vzoriek), ak ešte neodišli.


## Ďalšie správy: výkresy s kondenzátorom vedľa článku

> Pls reference the drawings.🙏 (príloha: dva výkresy)

Preklad: „Prosím, pozrite si výkresy. 🙏"

Anne poslala dva výkresy, o ktorých písala (správa 09:56: kondenzátor sa dá umiestniť vedľa batérie):
- [ER26500H + EPC1520 vedľa seba](../navrhy/2026-11-17_sunj_vykres_ER26500H-EPC1520-vedla-seba.pdf): **52 × 40 × 26 mm**, kábel 100 ± 5 mm
- [ER34615H + EPC1520 vedľa seba](../navrhy/2026-11-17_sunj_vykres_ER34615H-EPC1520-vedla-seba.pdf): **63 × 48 mm**, hrúbka nie je zakótovaná, kábel 100 ± 5 mm

Preklad výkresov, porovnanie s katalógom a poznámky: [prehľad výkresov](../navrhy/SUNJ_vykresy_vedla-seba_sk.md). Dôležité: na výkresoch **nie je určený konektor** (XH-2P treba objednať výslovne) a pri ER34615H chýba hrúbka packu.

## Rozhodnutie (Roland): potrebujeme oba typy

Roland potrebuje **obe konštrukcie**: rovnú rúrku (kondenzátor na článku) aj verziu s kondenzátorom vedľa článku, pre obe kapacity. Ide teda o štyri packy s EPC1520:

| | rovná rúrka (kondenzátor na článku, z katalógu) | kondenzátor vedľa článku (z výkresov) |
|---|---|---|
| 8,5 Ah | ER26500H + EPC1520, Ø29 × 67 mm | ER26500H + EPC1520, 52 × 40 × 26 mm |
| 19 Ah | ER34615H + EPC1520, Ø34 × 78 mm | ER34615H + EPC1520, 63 × 48 mm (hrúbka chýba) |

Správa pre Anne (po anglicky, bez odrážok):

Thank you very much for the drawings. We need both types of the packs: the straight tube version (capacitor on top of the battery, as in your catalog) and the version with the EPC1520 capacitor beside the battery (as in your drawings). So we need four packs: ER26500H + EPC1520 for 8.5 Ah in both versions, and ER34615H + EPC1520 for 19 Ah in both versions.

Please change two things. First, at the end of the cable, please fit an XH-2P housing (JST XH, 2.5 mm pitch) with the red wire (plus) on pin 1 and the black wire (minus) on pin 2. Your ER26500H drawing shows bare terminals and the ER34615H drawing does not show the connector type. Second, please add the thickness of the ER34615H pack to the drawing, because it is not marked. Could you also send me the drawing of the straight tube version of both packs with the cable and the connector?

Could you please send me the prices of all four packs for 100 / 1,000 / 5,000 pieces, with the XH-2P connector, and the delivery time for 20 samples? We also still need the voltage of the pack during 0.6 A pulses (10 ms) at -30 C.

Thank you very much!

## Odpoveď Anne: aktualizované výkresy zajtra, adresa na dopravu

Originál:

> Hello Roland,
> Ok, we will send you update drawings tomorrow.
> Can you share me your details address and post code for shipping cost?

Preklad:

> Dobrý deň, Roland, dobre, aktualizované výkresy vám pošleme zajtra. Môžete mi poslať vašu podrobnú adresu a PSČ kvôli nákladom na dopravu?

Poznámka: aktualizované výkresy (rúrka, konektor XH-2P, hrúbka ER34615H) prídu **2026-11-18**. Adresa je na výpočet dopravy vzoriek; poslať **firemnú adresu** (nie súkromnú). Adresu do repa nezapisujem.

Návrh odpovede (po anglicky; adresu doplní Roland):

> Thank you, Anne. We will wait for the updated drawings tomorrow. Our company address for shipping is: [company name, street and number, postal code, city, country]. Could you please also tell me the price of the 20 samples (all four packs, or each type) and the shipping cost?

## Ceny od Anne (11:45–11:49)

Originál:

> ok (11:45)
> ER26500H+EPC1520  USD3.5/pcs (11:46)
> ER34615H+EPC1520  USD5/pcs (11:47)
> The position of the capacitor does not affect the price of the battery. (11:48)
> Should the samples be shipped together? (11:48)
> For the shipping cost, pls wait. (11:49)

Preklad:

> Dobre.
> ER26500H+EPC1520: 3,5 USD/ks
> ER34615H+EPC1520: 5 USD/ks
> Poloha kondenzátora neovplyvňuje cenu batérie.
> Majú sa vzorky poslať spolu?
> Na náklady dopravy, prosím, počkajte.

| Pack | Cena | Poznámka |
|---|---|---|
| ER26500H + EPC1520 (8,5 Ah) | **3,5 USD/ks** | rúrka aj vedľa seba rovnaká cena |
| ER34615H + EPC1520 (19 Ah) | **5 USD/ks** | rúrka aj vedľa seba rovnaká cena |

**Nejasné:** pre aké množstvo cena platí (vzorky, 100, 1 000, 5 000 ks)? Zahŕňa kábel 100 mm a konektor XH-2P? Za akých podmienok dodania (Incoterms: EXW, FOB, DAP)? Bez DPH a cla? Doprava sa počíta zvlášť, Anne ju pošle neskôr.

Pri 20 vzorkách (napr. po 5 ks každej zo 4 verzií) by to bolo **85 USD** bez dopravy (10 × 3,5 + 10 × 5). Počet kusov každej verzie určí Roland.

## Záver dňa

Originál:

> It's too late today; I'll send you quotations tomorrow.

Preklad:

> Dnes je už neskoro; ponuky vám pošlem zajtra.

**Čakáme na 2026-11-18:** cenové ponuky, aktualizované výkresy (rúrka, konektor XH-2P, hrúbka ER34615H), náklady na dopravu. Naše otvorené otázky (množstvo pri cene, kábel a konektor v cene, Incoterms, napätie pri −30 °C) zatiaľ bez odpovede.

## Otázka na dopravu väčších objemov

Originál:

> For bulk shipments, do you prefer sea freight or air freight?

Preklad:

> Pri väčších zásielkach, uprednostňujete námornú alebo leteckú dopravu?

Poznámky (môj odhad, overiť u špeditéra):
- Hmotnosť podľa špecifikácií: ER26500H + EPC1520 max. 65 g, ER34615H + EPC1520 max. 120 g. Pri 1 000 ks je to asi 65 kg resp. 120 kg, pri 3 000 ks asi 195 kg resp. 360 kg (bez obalu).
- Primárne lítiové batérie (UN 3090) sú nebezpečný tovar triedy 9. Letecky sa zvyčajne prepravujú len v nákladnom lietadle a s obmedzeniami, námorná doprava je možná, ale trvá približne 5–7 týždňov. Podmienky treba potvrdiť u špeditéra, ktorý vie prepravu nebezpečného tovaru.

Návrh odpovede (po anglicky), kým sa Roland nerozhodne:

> For the first orders we would prefer air freight, because the quantities are small and we need them quickly. Later, for regular larger orders, we can consider sea freight. Could you please quote both, for 1,000 and 3,000 pieces, to our address in Germany, and tell me which freight forwarder you use for lithium batteries (UN 3090)?

## Možnosti dopravy od Anne (15:09–15:11)

Originál:

> For samples, you can choose either door-to-door air freight or door-to-door delivery via DHL. Express shipping typically takes 7–10 days, while door-to-door air freight takes 15–20 days. (15:09)
> For bulk shipments, sea freight can be used; while this method involves a longer transit time, it offers lower shipping costs. (15:10)
> I can provide you with quotes for different shipping methods tomorrow. Shipping costs are calculated separately. (15:11)

Preklad:

> Pri vzorkách si môžete vybrať buď leteckú dopravu „od dverí k dverám", alebo doručenie „od dverí k dverám" cez DHL. Expresná zásielka zvyčajne trvá 7–10 dní, letecká doprava od dverí k dverám 15–20 dní.
> Pri väčších zásielkach sa dá použiť námorná doprava; trvá dlhšie, ale má nižšie náklady na dopravu.
> Zajtra vám môžem poslať ponuky pre rôzne spôsoby dopravy. Náklady na dopravu sa počítajú zvlášť.

| | Vzorky | Veľké zásielky |
|---|---|---|
| Možnosti | DHL expres (7–10 dní) alebo letecká doprava „od dverí k dverám" (15–20 dní) | námorná (dlhšie, lacnejšie) |
| Náklady | zvlášť, ponuka zajtra | zvlášť, ponuka zajtra |

**Otvorené:** „door-to-door" nemusí znamenať, že cena zahŕňa clo a dovozné DPH; treba sa opýtať (DAP alebo DDP). Cena dopravy sa počíta zvlášť od ceny batérií.

Návrh odpovede (po anglicky):

> Thank you, Anne. Please send me the quotes tomorrow for the samples (both DHL express and door-to-door air freight) and for bulk orders by sea freight (1,000 and 3,000 pieces). Please also tell me if the door-to-door price includes import duty and import VAT, or if we pay them separately in Germany.

## Rozlúčka (15:18)

> ok, my friend 😊😊 / Have a nice day ☺️

Preklad: „Dobre, priateľ môj. Pekný deň." Dnes už nič ďalšie; zajtra (2026-11-18) ponuky, výkresy a doprava.

## 2026-11-18 ráno: ponuky a výkresy poslané e-mailom, opakovaná otázka na podmienky

Originál (08:50):

> Hello Roland, good morning😊
> I have sent the quotations and drawings to your mail, pls check.
> Besides, what kind of device is your battery pack used in? Does your equipment operate at 0.6 A pulses (10 ms) -30°C all the time? Could you provide a detailed description of the conditions under which your equipment operates?

Preklad:

> Dobrý deň, Roland, pekné ráno 😊
> Poslala som ponuky a výkresy na váš e-mail, prosím, skontrolujte.
> Okrem toho, v akom zariadení sa váš batériový pack používa? Pracuje vaše zariadenie neustále s impulzmi 0,6 A (10 ms) pri −30 °C? Môžete poskytnúť podrobný opis podmienok, v ktorých vaše zariadenie pracuje?

**Poznámky:**
- Ponuky a aktualizované výkresy prišli **e-mailom** (firemná pošta Rolanda). Do repa ich treba doplniť po prečítaní (PDF do `navrhy/`, preklad).
- Anne sa už druhýkrát pýta na impulzy 0,6 A pri −30 °C a podmienky zariadenia (prvá otázka 2026-11-17 09:59). Chce zrejme overiť, či jej pack s EPC1520 postačí. Treba odpovedať podrobnejšie.
- Podklady na odpoveď z pôvodných dopytov (nutné potvrdiť, že platia): priemerná záťaž ≈ 160 µA; impulzy ≈ 30 mA po dobu ≈ 2 ms každú sekundu (zriedka až 10 za sekundu); raz denne rádiové spojenie ≈ 1 min s impulzmi do 0,6 A po dobu 10 ms; prevádzka −30 až +70 °C; zariadenie je zaliate alebo vo vodotesnej krabici, na vonkajšie použitie, s rádiovým modulom.
