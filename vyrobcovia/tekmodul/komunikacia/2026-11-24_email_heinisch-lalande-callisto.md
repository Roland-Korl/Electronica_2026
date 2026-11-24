# 2026-11-24 – e-mail od Petra Heinischa (tekmodul): Taoglas nie, alternatívy LALANDE, CALLISTO, TARVOS

- **Typ:** email
- **Smer:** prijaté
- **Od:** Peter Heinisch, tekmodul GmbH (p.heinisch@tekmodul.de)

## Pôvodný text (originál, nemčina)

> Hallo Herr Korl,
>
> Da wir keine taoglas Antennen führen, kann ich Ihnen kein Angebot zu der angesprochenen Antenne unterbreiten.
> Durch die Konkretisierung der Frequenzbänder können wir auch auf andere Antennen ausweichen, die sich auch preislic attraktiver gestalten, wie zB die LALANDE (https://synzen.com.tw/products/lalande1).
> 1. Gibt es eine definierte Dimension, also Länge und Breite der FPC Antenne, die eingehalten werden muss bzw zur Verfügung steht, dann kann ich die möglichen Treffer eingrenzen. Welchen Konnektor muss die Antenne haben? Ich vermute einen MHF1?
> 2. Eine externe Antennen können wir ebenfalls beschaffen bze Sie mit Muster zum Testen versorgen. Genauso haben wir pigtails in definierter Größe im Angebot, um die Schnittstelle aus dem Gheäuse nach draußen zu führen. Gibt es bei der externen Antenne Vorstellungen, welche Größe es sein darf/muss? Mogliche Alternativen mit SMA wäre die CALLISTO1 (https://synzen.com.tw/products/callisto1) oder TARVOS (https://synzen.com.tw/products/tarvos).
>
> Lalande (MHF1) und Callisto (SMA) können wir Ihnen die Muster umgehend zusenden, wenn die Anschlüsse passen (MHF1?)
> Elnath müsste ich wie Tarvos bei synzen beziehen, was aber kein Problem darstellt.
>
> beste Grüße
> Peter Heinisch, Technischer Vertrieb Nord, tekmodul GmbH (konateľ: Tassilo Halt, obchodný register München HRB 158866)

## Preklad do slovenčiny

> Dobrý deň, pán Korl,
>
> keďže antény Taoglas nepredávame, nemôžem vám na spomínanú anténu poslať ponuku.
> Keďže ste upresnili frekvenčné pásma, môžeme použiť aj iné antény, ktoré sú aj cenovo výhodnejšie, napríklad **LALANDE**.
> 1. Je daný rozmer, teda dĺžka a šírka FPC antény, ktorý treba dodržať alebo ktorý je k dispozícii? Potom viem zúžiť výber. Aký konektor musí anténa mať? Predpokladám MHF1?
> 2. Vonkajšiu anténu vieme tiež zaobstarať a poslať vám vzorky na testovanie. Rovnako ponúkame **pigtaily** (prepojovacie káble) v danej dĺžke, ktorými sa rozhranie vyvedie z krabice von. Máte predstavu, aký veľká môže alebo musí byť vonkajšia anténa? Možné alternatívy s konektorom SMA sú **CALLISTO1** alebo **TARVOS**.
>
> Vzorky LALANDE (MHF1) a CALLISTO (SMA) vám vieme poslať hneď, ak konektory sedia (MHF1?).
> ELNATH a TARVOS by som musel objednať u Synzenu, čo nie je problém.

## Vysvetlenie

- **Taoglas FXUB63 nepredávajú**, ponúkajú len antény Synzen.
- **LALANDE** (FPC, vnútorná, konektor MHF1 = U.FL) a **CALLISTO1** (vonkajšia, SMA) majú hneď skladom na vzorky. **ELNATH** (FPC) a **TARVOS** (vonkajšia, SMA) objednajú zo Synzenu.
- **Pigtail** je krátky kábel, ktorý z konektora U.FL na doske vedie k priechodke so SMA na stene krabice; zvonka sa naň naskrutkuje vonkajšia anténa. To je riešenie pre kovovú krabicu.
- **MHF1 = I-PEX MHF I = U.FL**, rovnaký konektor, aký mala FXUB63.

## Čo potrebujeme upresniť (Roland)

- Max. rozmer FPC antény v plastovej krabici (dĺžka × šírka).
- Konektor na doske: MHF1 / U.FL? (FXUB63 ho mala, takže pravdepodobne áno.)
- Max. rozmer vonkajšej antény a spôsob montáže (na stenu krabice, na stožiar).
- Dĺžka pigtailu z dosky k stene krabice.

## Upresnenie od Rolanda (2026-11-24)

1. FPC anténa: čím menšia, tým lepšia; max. priestor ako pre súčasnú Taoglas FXUB63.
2. Konektor na doske: MHF1 (U.FL), potvrdené.
3. Vonkajšia anténa: montáž na **hliníkovú krabicu**, čím menšia, tým lepšia, ideálne veľkosti mince 2 € (Ø asi 26 mm).
4. Pigtail: do 150 mm.

Poznámka (môj odhad): anténa veľkosti mince bude pri 800/900 MHz (pásma B20, B8) mať nízku účinnosť, lebo vlnová dĺžka je tam asi 35 cm. Hliníková krabica môže poslúžiť ako uzemňovacia plocha a pomôcť. Treba nechať odporučiť dodávateľa a overiť testom signálu.

## Odpoveď (nemčina)

Hallo Herr Heinisch,

vielen Dank für die schnelle Antwort und die Vorschläge. Hier die Angaben:

1. FPC-Antenne: je kleiner, desto besser. Maximal steht der Platz der aktuellen Taoglas FXUB63 zur Verfügung.
2. Anschluss: ja, auf der Platine ist MHF1 (U.FL).
3. Externe Antenne: Montage auf einem Aluminiumgehäuse im Außenbereich, also wetterfest. Auch hier gilt: je kleiner, desto besser, ideal wäre etwa die Größe einer 2-Euro-Münze. Uns ist klar, dass das bei 800/900 MHz schwierig ist. Welche ist die kleinste externe Antenne, die Sie für LTE-M (Band 20, 8 und 3) auf einem Metallgehäuse empfehlen können?
4. Pigtail: maximal 150 mm, von MHF1 (U.FL) auf SMA-Buchse zur Gehäusedurchführung.

Bitte senden Sie uns gern schon Muster: je 5 Stück LALANDE (MHF1), CALLISTO1 (SMA) und 5 passende Pigtails, sowie Ihre Empfehlung für eine kleinere externe Antenne. Bitte schicken Sie uns auch die Preise für 100 / 1.000 / 5.000 Stück.

Vielen Dank und beste Grüße
Roland Korl
Leiter IT-Abteilung
E.P.S. Germany GmbH
