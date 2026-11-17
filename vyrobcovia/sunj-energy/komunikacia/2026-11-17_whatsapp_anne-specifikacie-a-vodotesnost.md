# 2026-11-17 – Anne (Sunj Energy): špecifikácie ER26500H a ER34615H, otázka na vodotesnosť

- **Typ:** chat (WhatsApp)
- **Smer:** prijaté
- **S kým:** Anne, Sunj Energy
- **Prílohy:**
  - [ER26500H + EPC1520, špecifikácia (PDF)](../dokumenty/2026-11-17_SUNJ_ER26500H-EPC1520_specifikacia_en.pdf) · [preklad](../dokumenty/SUNJ_ER26500H-EPC1520_specifikacia_sk.md)
  - [ER34615H + EPC1520, špecifikácia (PDF)](../dokumenty/2026-11-17_SUNJ_ER34615H-EPC1520_specifikacia_en.pdf) · [preklad](../dokumenty/SUNJ_ER34615H-EPC1520_specifikacia_sk.md)
  - fotka oboch packov (v repe nie je uložená, len opis nižšie)

## Zhrnutie

Anne poslala špecifikácie dvoch packov, ktoré zodpovedajú našim dvom aplikáciám:
- **ER26500H + EPC1520**: 8 500 mAh (aplikácia 1)
- **ER34615H + EPC1520**: 19 000 mAh (aplikácia 2)

Pýta sa, či náš pack vyžaduje vodotesnú úpravu, a ponúka, že ju vyrobia podľa našich požiadaviek. Konektor na ich schéme je **PH-2P 2,0 mm** (sedí s naším JST PH 2.0), kábel **100 mm**.

## Pôvodný text (originál)

> This is an integrated, waterproof battery pack consisting of an ER26500H battery and an EPC1520 capacitor, with the capacitor positioned above the battery's positive terminal. Does your battery pack require any waterproofing treatment?
>
> If your battery pack has a water-resistance requirement, we can manufacture it according to your specifications.

## Preklad do slovenčiny

> Toto je integrovaný, vodotesný batériový pack zložený z článku ER26500H a kondenzátora EPC1520, pričom kondenzátor je umiestnený nad kladným pólom článku. Vyžaduje váš batériový pack nejakú vodotesnú úpravu?
>
> Ak má váš batériový pack požiadavku na odolnosť proti vode, vieme ho vyrobiť podľa vašich špecifikácií.

## Fotka

Dva packy vedľa seba na drevenom stole: **ER34615H** (väčší, s dvomi vodičmi červený/čierny, ktoré vychádzajú z čierneho plastového krytu na vrchu) a **ER26500H** (menší, tiež s čiernym plastovým krytom na vrchu). Štítky „SUNJ, LITHIUM BATTERY 3.6V", značka + hore a − dolu. Čierny kryt na vrchu je podľa špecifikácie asi miesto s kondenzátorom (EPC1520) a vyvedením vodičov.

## Čo z dokumentov vyplýva pre nás

| | ER26500H + EPC1520 | ER34615H + EPC1520 |
|---|---|---|
| Kapacita (2 mA, 25 °C) | 8 500 mAh | 19 000 mAh |
| Hmotnosť | max. 65 g | max. 120 g |
| Rozmery packu | Ø27 × 67 mm (výkres) | **v dokumente nie sú** |
| Max. impulz | 2 000 mA | 2 000 mA |
| Prevádzková teplota | −40 až +85 °C | −40 až +85 °C |
| Kábel / konektor | 100 mm, PH-2P 2,0 mm | 100 mm, PH-2P 2,0 mm |

Naše požiadavky (z pôvodných dopytov, ak platia): −30 až +70 °C, impulzy do 0,6 A po dobu 10 ms aj pri −30 °C. Špecifikácia deklaruje max. 2 A impulz a prevádzku od −40 °C, ale **napätie počas impulzov pri −30 °C** pre naše parametre v dokumente nie je (grafy sú pre 350 mA pri −20 / −40 °C), takže to treba od Anne vypýtať.

Vyriešené z našich otázok: dátový list, typ konektora (PH-2P 2,0 mm), dĺžka kábla (100 mm), hmotnosť.
Stále otvorené: cena, dodacia lehota vzoriek, rozmery ER34615H packu, polarita na pinoch (+ na pine 1, − na pine 2), napätie pri impulzoch −30 °C, rozdiel medzi verziami 65 / 67 / 68 mm, **odpoveď na vodotesnosť**.

## Dohodnuté kroky

- [ ] Rozhodnúť o vodotesnosti (pozri návrh odpovede v správe; po rozhodnutí doplniť sem).
- [ ] Odpovedať Anne.

## Ďalšia fotka (vzorka ER26500H s káblom a konektorom)

Pack ER26500H zblízka: z čierneho plastového krytu na vrchu vychádza červený a čierny vodič, ktorý končí **malým bielym dvojpólovým konektorom** (plastové puzdro, na konci vodičov čierna zmršťovacia bužírka). Vzhľad zodpovedá káblovému puzdru typu JST PH, ale z fotky to nedokážem potvrdiť; polarita pinov sa na fotke nedá určiť (vodiče sú červený a čierny, pravdepodobne červený +, čierny −). Fotka nie je uložená v repe.

## Ďalšia správa: konektory

> There are many types of connectors, and they generally need to be compatible with your equipment.

Preklad:

> Existuje veľa typov konektorov a zvyčajne musia byť kompatibilné s vaším zariadením.

Poznámka: Anne tým naznačuje, že musíme jasne povedať, aký konektor máme my. Ich špecifikácia uvádza **PH-2P 2,0 mm** a my používame **JST PH 2.0**, takže typ sedí; treba už len potvrdiť, že ich puzdro je správny protikus (káblová strana) k nášmu a že **pin 1 = +, pin 2 = −**.

Návrh odpovede (po anglicky):

> Yes, I understand. Our device uses a JST PH 2.0 connector (2 pins, 2.0 mm pitch). Your specification shows PH-2P 2.0 mm, so this is what we need. Please use the matching cable-side housing for it, with plus on pin 1 and minus on pin 2. Could you please confirm this?

Po slovensky: Áno, rozumiem. Naše zariadenie používa konektor JST PH 2.0 (2 piny, rozstup 2,0 mm). Vaša špecifikácia uvádza PH-2P 2,0 mm, takže presne toto potrebujeme. Použite, prosím, zodpovedajúce káblové puzdro s plusom na pine 1 a mínusom na pine 2. Môžete to, prosím, potvrdiť?

## Katalóg konektorov od Anne

Anne poslala obrázok s prehľadom 2-pólových konektorov, ktoré vedia pripojiť: [katalóg konektorov](../dokumenty/2026-11-17_sunj_katalog-konektorov-2p.jpg). Sú v ňom napríklad SM-2P, 5264-2P, **PH-2P**, EH-2P, 51021-2P, XH-2P, JST-2P, VA-2P, 2510-2P, 43645-0200 (Molex), EDG-3P 5,08 a ďalšie. Pri každom sú číslované piny (2 1) a farby vodičov.

Pri **PH-2P** (náš typ) je na obrázku červený vodič pri pine 1 a čierny pri pine 2. To by sedelo s naším požiadavkou (+ na pine 1, − na pine 2), ak je červený +. Z obrázka to neviem potvrdiť s istotou, treba, aby to Anne písomne potvrdila.

## Nová otázka: pack 8,5 Ah s článkom a kondenzátorom vedľa seba

Roland chce zistiť, či majú batériu 8,5 Ah, ktorá **nie je jeden dlhý valec**, ale **dva valce vedľa seba**: hlavný veľký a tučný (článok) a vedľa neho malý pomocný (impulzný kondenzátor). Pack by bol kratší, ale širší.

Návrh odpovede (po anglicky):

> Thank you for the connector overview. We use PH-2P (JST PH 2.0), with red wire (plus) on pin 1 and black wire (minus) on pin 2. Please confirm.
>
> One more question: do you also have an 8.5 Ah pack where the cell and the capacitor are not stacked in one long tube, but placed side by side? That means the big cell (ER26500H) and the small capacitor (EPC1520) next to each other. We would like a shorter pack. If yes, please send the drawing with dimensions, the price and the delivery time.

Po slovensky: Ďakujem za prehľad konektorov. Používame PH-2P (JST PH 2.0), s červeným vodičom (plus) na pine 1 a čiernym vodičom (mínus) na pine 2. Potvrďte, prosím. Ešte jedna otázka: máte aj pack 8,5 Ah, kde nie sú článok a kondenzátor naskladané v jednej dlhej rúrke, ale uložené vedľa seba? Teda veľký článok (ER26500H) a malý kondenzátor (EPC1520) vedľa seba. Chceli by sme kratší pack. Ak áno, pošlite výkres s rozmermi, cenu a dodaciu lehotu.

## Nápad: vypýtať kompletný zoznam packov

Roland chce, aby Anne poslala **všetky batérie Li-SOCl2 + SPC, ktoré majú** (článok s impulzným kondenzátorom); Roland si vyberie vhodné a až potom sa pýtame na ceny.

Návrh odpovede (po anglicky):

> Could you please send me a list of all your Li-SOCl2 batteries with an SPC capacitor, in all sizes and capacities (cell and capacitor stacked, and side by side if you have it)? For each type, please send the datasheet or at least the capacity, the dimensions and the weight. I will choose the ones that fit our device, and then I will ask you for the prices.

Po slovensky: Môžete mi, prosím, poslať zoznam všetkých vašich Li-SOCl2 batérií s kondenzátorom SPC vo všetkých veľkostiach a kapacitách (článok a kondenzátor na sebe a ak máte, aj vedľa seba)? Pri každom type pošlite dátový list alebo aspoň kapacitu, rozmery a hmotnosť. Vyberiem tie, ktoré sa hodia do nášho zariadenia, a potom sa vás opýtam na ceny.

## Rozhodnutie a finálna správa pre Anne

**Rozhodnutie (Roland):** vodotesná úprava packu **nie je potrebná**, zariadenie bude vo vodotesnej krabičke.

Správa na odoslanie je v texte bez odrážok, aby sa dala skopírovať do WhatsAppu.

**Po anglicky (na odoslanie):**

Hello Anne, thank you for the specifications, the photos and the connector overview. I received your email as well, thank you.

About waterproofing: we do not need any extra waterproof treatment of the pack, because our device will be in a waterproof box. So your standard pack is fine as it is.

About the connector: we use PH-2P (JST PH 2.0). Please make it with the red wire (plus) on pin 1 and the black wire (minus) on pin 2. Could you please confirm this?

We need two sizes: about 8.5 Ah (like your ER26500H + EPC1520) and at least 19 Ah (like your ER34615H + EPC1520). The ER34615H specification has no dimensions. Could you please send them?

Could you also send me a list of all your Li-SOCl2 batteries with an SPC capacitor, in all sizes and capacities? For each type, please send the capacity, the dimensions, the weight and the pulse performance at -30 C if you have it. It is also interesting for us if you have a version where the cell and the capacitor are side by side and not stacked, because that pack would be shorter. We will choose the ones that fit our device, and then I will ask you for the prices.

Thank you very much!

**Po slovensky (význam):**

Dobrý deň, Anne, ďakujem za špecifikácie, fotky a prehľad konektorov. E-mail som dostal tiež, ďakujem.

K vodotesnosti: nepotrebujeme žiadnu extra vodotesnú úpravu packu, lebo naše zariadenie bude vo vodotesnej krabičke. Váš štandardný pack je teda v poriadku tak, ako je.

K konektoru: používame PH-2P (JST PH 2.0). Prosím, urobte ho s červeným vodičom (plus) na pine 1 a čiernym vodičom (mínus) na pine 2. Môžete to, prosím, potvrdiť?

Potrebujeme dve veľkosti: asi 8,5 Ah (ako váš ER26500H + EPC1520) a aspoň 19 Ah (ako váš ER34615H + EPC1520). V špecifikácii ER34615H nie sú rozmery. Môžete ich, prosím, poslať?

Môžete mi tiež poslať zoznam všetkých vašich Li-SOCl2 batérií s kondenzátorom SPC vo všetkých veľkostiach a kapacitách? Pri každom type pošlite kapacitu, rozmery, hmotnosť a impulzný výkon pri −30 °C, ak ho máte. Zaujíma nás aj verzia, kde sú článok a kondenzátor vedľa seba a nie na sebe, lebo taký pack by bol kratší. Vyberieme tie, ktoré sa hodia do nášho zariadenia, a potom sa opýtam na ceny.

Veľmi pekne ďakujem!


## OPRAVA konektora: nie PH, ale XH (2026-11-17, 09:53–09:59)

Roland si overil konektor na vlastnej doske (PCB): je to **JST B2B-XH-A(LF)(SN)**, teda séria **XH s rozstupom 2,5 mm**, nie PH 2.0. Všetky predchádzajúce zmienky o „JST PH 2.0" a „PH-2P" ako našom konektore v tomto súbore a v návrhoch odpovedí sú **zastarané**. Potrebný protikus (káblová strana) je **XH-2P** (puzdro XHP-2), ktorý je aj v katalógu konektorov od Anne. PH (2,0 mm) a XH (2,5 mm) nie sú vzájomne zameniteľné.

Zdroj správ: [snímka obrazovky](../obrazky/2026-11-17_whatsapp-anne-konektor-a-pulzy.png)

### Správy od Anne (originál)

> [Obrázok: katalóg konektorov s označeným PH-2P] (09:53)
> Is the connector the same as the one in the picture? (09:54)
> The capacitor can be placed on the side of the battery; I will provide you with the drawings shortly. (09:56)
> Does your equipment operate at 0.6 A pulses (10 ms) -30°C all the time? (09:59)
> Could you provide more details regarding the operating status of your equipment? Additionally, for the 20 sets of samples, could you please provide your full address and postal code? (09:59)

### Preklad

> Je konektor rovnaký ako ten na obrázku?
> Kondenzátor sa dá umiestniť vedľa batérie; čoskoro vám pošlem výkresy.
> Pracuje vaše zariadenie neustále s impulzmi 0,6 A (10 ms) pri −30 °C?
> Môžete poskytnúť viac podrobností o prevádzkovom stave vášho zariadenia? A pre 20 súprav vzoriek, prosím, uveďte vašu úplnú adresu a PSČ.

### Čo z toho vyplýva

- **Konektor:** nie je rovnaký, treba opraviť na XH-2P.
- **Kondenzátor vedľa článku:** Anne potvrdila, že sa to dá; pošle výkresy.
- **Impulzy:** pýta sa, či je zariadenie neustále pri −30 °C s impulzmi 0,6 A. Z pôvodných dopytov: impulzy 0,6 A po dobu 10 ms sa vyskytujú len pri rádiovej komunikácii (BAT-02: raz denne asi 1 min; BAT-01: raz za 48 h asi 20 s), medzitým malá záťaž (BAT-02: priemer ≈ 160 µA s impulzmi ≈ 30 mA po dobu ≈ 2 ms každú sekundu). −30 °C je spodná hranica prevádzkovej teploty, nie trvalý stav. **Pred odoslaním treba overiť, že tieto údaje platia aj pre nový model.**
- **Adresa pre 20 vzoriek:** zatiaľ nepripraviť; adresu poslať až po výbere packu a dohode o cene.
