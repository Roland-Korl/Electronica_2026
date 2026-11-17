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
