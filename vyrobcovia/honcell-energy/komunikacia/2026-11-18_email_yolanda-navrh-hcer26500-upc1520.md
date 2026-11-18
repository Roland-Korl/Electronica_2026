# 2026-11-18 – e-mail od Yolandy Zou (Honcell): návrh HCER26500 + UPC1520

- **Typ:** email
- **Smer:** prijaté
- **Od:** Yolanda Zou, Sales Representative, Shenzhen Honcell Energy Co., Ltd (honcell802@honcell.com)
- **Komu:** Roland Korl

## Zhrnutie

Honcell podľa našej doterajšej špecifikácie (zrejme pôvodný dopyt EPS-BAT-02: pack max. Ø28 × 80 mm) navrhuje **HCER26500 + UPC1520**, 3,6 V, 8 500 mAh. Pýta sa, či si článok a kondenzátor budeme skladať sami, alebo chceme hotový pack, a ako pripojíme výstup packu.

## Pôvodný text (originál)

> Hi Roland,
>
> This is Yolanda. Based on current spec. we received, we suggest model HCER26500+UPC1520.
>
> HCER26500+UPC1520  3.6V  8500mAh
> Bare raw cell (D*H): 25.6±0.2*50.0±0.5mm
> Battery pack (D*H): Max.28.0*80.0mm
> Standard discharge rate: 2.0mA
> Continuous discharge rate: 150.0mA
> Pulse rate: 2000.0mA/3S
> Working temperature: -55~85℃
> Pack: 26500 single cell+UPC1520 capacitor, wrapped with blue PVC heat shrink tubing, with text marking.
>
> For further evaluation, we need to confirm how the end device is assembled. Are you going to assemble it by yourself, or do you need us to pre-assemble the cell and capacitor together? Also, could you advise how you will connect the output of the battery pack?
>
> Best Regards,
> Yolanda Zou, Sales Representative, Shenzhen Honcell Energy Co., Ltd.

## Preklad do slovenčiny

> Dobrý deň, Roland,
>
> tu Yolanda. Na základe aktuálnej špecifikácie, ktorú sme dostali, navrhujeme model HCER26500+UPC1520.
>
> HCER26500+UPC1520, 3,6 V, 8 500 mAh
> Holý článok (priemer × výška): 25,6 ± 0,2 × 50,0 ± 0,5 mm
> Batériový pack (priemer × výška): max. 28,0 × 80,0 mm
> Štandardný vybíjací prúd: 2,0 mA
> Trvalý vybíjací prúd: 150,0 mA
> Impulzný prúd: 2 000,0 mA / 3 s
> Pracovná teplota: −55 až +85 °C
> Pack: jeden článok 26500 + kondenzátor UPC1520, obalený modrou PVC zmršťovacou fóliou, s textovým označením.
>
> Na ďalšie posúdenie potrebujeme vedieť, ako sa koncové zariadenie montuje. Budete si ho skladať sami, alebo potrebujete, aby sme článok a kondenzátor zmontovali dokopy my? A môžete nám povedať, ako pripojíte výstup batériového packu?

## Poznámky

- Návrh vychádza z **pôvodného dopytu** (rozmer Ø28 × 80 mm = šachta z EPS-BAT-02). Teraz už platí [EPS-BAT-SPEC v2.0](../../../podklady/EPS-BAT-SPEC_v2-0_sk.md).
- **Trvalý prúd 150 mA** je presne na hranici našej rádiovej relácie (≈ 130–150 mA až 7 min). Sunj udáva 500 mA. Treba overiť napätie pri tejto záťaži.
- Impulz 2 000 mA / 3 s je s rezervou voči našim 0,6 A / 10 ms.
- Ponúkajú len 8,5 Ah; pack 19 Ah (D) treba vypýtať.

## Návrh odpovede (e-mail, po anglicky)

Subject: Battery packs – updated requirements EPS-BAT-SPEC v2.0

Hi Yolanda,

Thank you very much for your proposal of the HCER26500+UPC1520.

In the meantime we have updated our requirements. Please find attached our new document EPS-BAT-SPEC v2.0, which replaces our earlier requests. The main points are:

1. We need two packs: Pack A, about 8.5 Ah (for example your HCER26500+UPC1520), and Pack B, about 19 Ah (D size cell with a capacitor).
2. We would like you to pre-assemble the cell and the capacitor into one ready pack, with a heat-shrink sleeve and no exposed contacts.
3. Output connection: two wires, 150 ± 10 mm, AWG 24–26, insulation rated at least +85 °C, with a JST XHP-2 connector (pin 1 = plus, red; pin 2 = minus, black). It mates with JST B2B-XH-A on our board.
4. The pack is placed in foam in a sealed box and is replaceable in the field. It is not potted.
5. The load profiles (worst case) are in sections 3 and 4. Please note that the radio session draws about 130–150 mA for up to 7 minutes. Your datasheet says 150 mA maximum continuous current. Could you please confirm that the voltage stays above 3.3 V at this load, also at -40 °C?

Could you please send us your proposal for both packs with a drawing (dimensions, weight), the datasheets, the usable capacity at our profiles, and prices for 5 / 100 / 1,000 / 5,000 pcs with the delivery terms and the lead time of the samples?

Best regards,
Roland Korl

**Po slovensky (význam):** Ďakujem za návrh HCER26500+UPC1520. Medzitým sme aktualizovali požiadavky, v prílohe posielam nový dokument EPS-BAT-SPEC v2.0, ktorý nahrádza pôvodné dopyty. Hlavné body: 1. potrebujeme dva packy, A asi 8,5 Ah (napr. váš HCER26500+UPC1520) a B asi 19 Ah (článok D s kondenzátorom); 2. chceme, aby ste článok a kondenzátor zmontovali do hotového packu so zmršťovacou fóliou a bez odhalených kontaktov; 3. výstup: dva vodiče 150 ± 10 mm, AWG 24–26, izolácia min. +85 °C, konektor JST XHP-2 (pin 1 plus červený, pin 2 mínus čierny), protikus JST B2B-XH-A na našej doske; 4. pack je v pene v uzavretej krabici, vymeniteľný na mieste, nezaliaty; 5. profily záťaže sú v častiach 3 a 4; rádiové spojenie odoberá asi 130–150 mA až 7 minút a váš dátový list udáva max. trvalý prúd 150 mA, potvrďte, prosím, že napätie zostane nad 3,3 V aj pri −40 °C. Pošlite nám návrh pre oba packy s výkresom, dátové listy, využiteľnú kapacitu pri našich profiloch a ceny pre 5 / 100 / 1 000 / 5 000 ks s dodacími podmienkami a lehotou vzoriek.
