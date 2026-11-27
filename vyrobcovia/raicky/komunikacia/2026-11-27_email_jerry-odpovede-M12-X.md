# 2026-11-27 – e-mail od Jerryho Zhu (Raicky): odpovede k zásuvke M12 X, test 10 Gbit

- **Typ:** email (v nemčine)
- **Smer:** prijaté
- **Od:** Jerry Zhu (szzrk@raicky.com)
- **Prílohy:** [testovací protokol Fluke 10GBASE-T](../dokumenty/2026-11-27_raicky_test-Fluke-10GBASE-T_120708-04-049.pdf), [opravený výkres 120708-04-049 (ukončenie DIP)](../navrhy/2026-11-27_raicky_vykres_120708-04-049_M12-X-zasuvka-PCB_S2_DIP.pdf)

## Pôvodný text (originál, nemčina)

> Dear Mr. Korl,
> Antwort:
> 1. Die Entwicklung erfolgt in Übereinstimmung mit der Norm IEC 61076-2-109.
> 2. Der Abstand von der Mitte der ersten Stiftreihe zur Montagefläche beträgt ebenfalls 4,1 mm REF, maximale Plattenstärke 1,5 mm.
> 3. Bei korrekter Montage und Verriegelung wird die Schutzart IP67 erreicht.
> 4. Die Kontaktstifte sind vergoldet.
> 5. Erfüllt die Cat6A-Datenübertragungsrate von 10 Gbit/s. Siehe Bericht.
> 6. „SMT" war ein Tippfehler, es handelt sich um DIP-Lötung. Die Zeichnung muss korrigiert werden.
>
> Jerry Zhu, Shenzhen Raicky Technology Co., Ltd

## Preklad do slovenčiny

> Vážený pán Korl, odpovede:
> 1. Vývoj je v súlade s normou IEC 61076-2-109 (číslovanie pinov M12 X).
> 2. Vzdialenosť od stredu prvého radu pinov k montážnej ploche je tiež 4,1 mm (orientačne), maximálna hrúbka panelu 1,5 mm.
> 3. Pri správnej montáži a zaistení sa dosiahne krytie IP67.
> 4. Kontaktné piny sú pozlátené.
> 5. Spĺňa prenosovú rýchlosť Cat6A 10 Gbit/s, pozri protokol.
> 6. „SMT" bol preklep, ide o spájkovanie DIP (piny do otvorov). Výkres treba opraviť.

Opravený výkres (stále rev. S2) už uvádza „Termination: DIP".

## Testovací protokol (Fluke, LinkWare PC; preklad z čínštiny)

| | |
|---|---|
| Označenie | 120708-04-049, kus 1 |
| Prístroj | Fluke DSX-8000 (hlavný a vzdialený), softvér V6.7, LinkWare PC 10.8.1 |
| Limit testu | **10GBASE-T** (V7.6) |
| Dátum testu | 21. 11. 2025 |
| Celkový výsledok | **vyhovuje (PASS)** |
| Typ kábla | Cat 6A F/UTP, NVP 74 % |
| Dĺžka | **0,9 m** (limit 100 m) |
| Oneskorenie / rozdiel oneskorenia | 5 ns / 1 ns |
| Odpor | 0,21 Ω |
| Zapojenie | T568B, vyhovuje |
| Najhoršia rezerva | **19,3 dB** (NEXT, páry 3,6–4,5) |
| Vložný útlm | rezerva 50,0 dB pri 477 MHz |
| NEXT / PS NEXT | rezerva 19,3–20,4 dB / 20,3–21,1 dB |
| ACR-F / PS ACR-F | rezerva 16,0–16,5 dB / 17,3–18,0 dB |
| Útlm odrazu (RL) | rezerva 6,2–6,3 dB |
| Splnené štandardy | 10BASE-T, 100BASE-TX, 1000BASE-T, 2.5GBASE-T, 5GBASE-T, 10GBASE-T, ATM, TR-16 a ďalšie |

## Porovnanie s Amphenol (doplnenie)

| | Amphenol MSXS-08PFFR-SF7003 | Raicky 120708-04-049 |
|---|---|---|
| Panel – prvý rad pinov | 4,30 | **4,1 (orientačne)**, o 0,2 mm menej |
| Hrúbka panelu | **1,0–4,0 mm** | **max. 1,5 mm** |
| Krytie | IP67 po zasunutí | IP67 pri správnej montáži |
| Piny | pozlátené | pozlátené |
| Norma pinov | (M12 X) | IEC 61076-2-109 |
| Ukončenie | THT | DIP (THT) |

## Poznámky (môj záver)

- **Hrúbka panelu max. 1,5 mm je dôležitá:** ak má vaša krabica stenu hrubšiu ako 1,5 mm, Raicky sa nedá namontovať (Amphenol do 4 mm). Treba zmerať.
- Rozdiel 0,2 mm (4,1 vs. 4,30 mm) medzi panelom a pinmi: pri doske navrhnutej pre Amphenol bude zásuvka o 0,2 mm inak voči panelu; pravdepodobne v tolerancii, ale overiť na vzorke.
- Protokol je test krátkej zostavy (0,9 m) podľa limitu aplikácie 10GBASE-T, nie formálna skúška komponentu Cat6A podľa normy pre konektory. Pre naše použitie (10 Gbit) je to dobrý signál. Prístroj mal kalibráciu z 2. 7. 2022, teda viac ako 3 roky pred testom (Fluke zvyčajne odporúča ročnú kalibráciu).
- Technicky odpovedal na všetko; ďalší krok je cenová ponuka.
