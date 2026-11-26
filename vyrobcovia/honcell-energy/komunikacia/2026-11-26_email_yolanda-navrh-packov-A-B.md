# 2026-11-26 – e-mail od Yolandy Zou (Honcell): návrh packov A a B

- **Typ:** email
- **Smer:** prijaté
- **Od:** Yolanda Zou, Shenzhen Honcell Energy Co., Ltd (honcell802@honcell.com)
- **Reaguje na:** EPS-BAT-SPEC v2.0

## Pôvodný text (originál)

> Hi Roland,
>
> This is Yolanda from Honcell Energy. Sorry for the late reply. Our technical team just had a busy week. Here we propose two solutions for your reference.
>
> Pack A:
> HCER26500ZC+UPC1520 3.6V 8500mAh
> Bare raw cell (D*H): 25.6±0.2*50.0±0.5mm
> Battery pack (D*H): Max.28.0*80.0mm
> Standard discharge: 2.0mA
> Maximum continuous discharge: 150.0mA
> Maximum pulse discharge: 2000.0mA/3S
> Working temperature: -55~85℃
> Wires & connector: JST XHP-02/Reversed polarity/UL3302-AWG24/Wire outlet on right, L=150mm
> Pack composition: 26500 cell+UPC1520 capacitor+connector&wires+blue PVC heat shrink tube+marking
>
> Pack B:
> HCER34615ZC+UPC1520 3.6V 19000mAh
> Bare raw cell (D*H): 32.7±0.2*60.4±0.8mm
> Battery pack (D*H): Max.35.0*80.0mm
> Standard discharge: 2.0mA
> Maximum continuous discharge: 250.0mA
> Maximum pulse discharge: 2000.0mA/1S
> Working temperature: -40~85℃
> Wires & connector: JST XHP-02/Reversed polarity/UL3302-AWG24/Wire outlet on right, L=150mm
> Pack composition: 34615 cell+UPC1520 capacitor+connector&wires+blue PVC heat shrink tube+marking
>
> Please kindly check the basic spec. including the working temperature. These two models are both wide-temperature range batteries. We will send the datasheet if there are no problems. Please feel free to let us know if there is any change in specifications.
>
> Best Regards,
> Yolanda Zou

## Preklad do slovenčiny

> Dobrý deň, Roland,
>
> tu Yolanda z Honcell Energy. Prepáčte neskorú odpoveď, náš technický tím mal rušný týždeň. Navrhujeme dve riešenia.
>
> **Pack A:** HCER26500ZC + UPC1520, 3,6 V, 8 500 mAh. Holý článok 25,6 ± 0,2 × 50,0 ± 0,5 mm. Pack max. Ø28,0 × 80,0 mm. Štandardné vybíjanie 2,0 mA. Max. trvalý prúd 150,0 mA. Max. impulz 2 000 mA / 3 s. Pracovná teplota −55 až +85 °C. Vodiče a konektor: JST XHP-02 / obrátená polarita / UL3302 AWG24 / vývod vodičov vpravo, dĺžka 150 mm. Zloženie: článok 26500 + kondenzátor UPC1520 + konektor a vodiče + modrá PVC zmršťovacia fólia + označenie.
>
> **Pack B:** HCER34615ZC + UPC1520, 3,6 V, 19 000 mAh. Holý článok 32,7 ± 0,2 × 60,4 ± 0,8 mm. Pack max. Ø35,0 × 80,0 mm. Štandardné vybíjanie 2,0 mA. Max. trvalý prúd 250,0 mA. Max. impulz 2 000 mA / 1 s. Pracovná teplota −40 až +85 °C. Vodiče a konektor rovnako ako pri A. Zloženie: článok 34615 + kondenzátor UPC1520 + konektor a vodiče + modrá PVC fólia + označenie.
>
> Skontrolujte, prosím, základné parametre vrátane pracovnej teploty. Oba modely sú batérie so širokým rozsahom teplôt. Ak je všetko v poriadku, pošleme dátové listy. Ak sa niečo v špecifikácii zmení, dajte nám vedieť.

## Porovnanie s EPS-BAT-SPEC v2.0 (môj záver)

| Požiadavka | Pack A (HCER26500ZC) | Pack B (HCER34615ZC) |
|---|---|---|
| Kapacita | 8 500 mAh ✓ | 19 000 mAh ✓ |
| Teplota −40 … +70 °C, do +85 °C | −55 … +85 °C ✓ | −40 … +85 °C ✓ |
| Trvalý prúd 150 mA až 7 min | **150 mA**, presne na hranici | 250 mA ✓ |
| Impulz 0,6 A / 10 ms | 2 000 mA / 3 s ✓ | 2 000 mA / 1 s ✓ |
| Priestor | ponúkli rúrku Ø28 × 80 mm; chceme rúrku aj vedľa seba | **rúrka Ø35 × 80 mm sa nezmestí** do 65 × 50 × 38 mm (80 > 65); potrebná verzia vedľa seba |
| Hmotnosť (pack B max. 120 g) | neuvedená | neuvedená |
| Vodiče 150 mm, izolácia ≥ +85 °C | UL3302 AWG24, 150 mm ✓ (UL3302 je podľa mojej znalosti XLPE na 105 °C) | rovnako ✓ |
| Konektor JST XHP-2, pin 1 = + (červený) | XHP-02, „**reversed polarity**" | rovnako |

**Hlavné otázky:**
- „Reversed polarity" (obrátená polarita): treba potvrdiť, že to znamená **pin 1 = + (červený), pin 2 = − (čierny)**, ako žiadame. Inak by bol pack zapojený opačne.
- Pack B potrebuje **verziu vedľa seba** do 65 × 50 × 38 mm a do 120 g.
- Pack A: ponúknuť aj verziu vedľa seba; trvalý prúd 150 mA je na hranici, treba napätie pri 150 mA a −40 °C.
- Ceny a využiteľná kapacita pri našich profiloch zatiaľ chýbajú.
