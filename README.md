# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 25.10.2026:** 4.396 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-24. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,5 % der 4.396 Spiele (2.353), die Stärkste Ansage in
75,7 % (3.329), das exakte Ergebnis in 10,7 % (472).

## Datei

`prognosen.csv` — eine Zeile je Spiel, UTF-8, Komma-getrennt.

| Spalte | Bedeutung |
|---|---|
| `datum` | Spieltag (deutsche Zeit) |
| `wettbewerb` | Kürzel des Wettbewerbs (Tabelle unten) |
| `heim`, `gast` | Mannschaften |
| `tendenz` | `1` Heimsieg · `X` Unentschieden · `2` Auswärtssieg |
| `ergebnis_prognose` | wahrscheinlichstes Ergebnis laut Engine |
| `staerkste_ansage` | die Aussage mit der höchsten Wahrscheinlichkeit für dieses Spiel |
| `staerkste_ansage_wahrscheinlichkeit` | vor dem Anpfiff angesagte Wahrscheinlichkeit (0–1) |
| `endstand_90_min` | Endstand nach 90 Minuten (ohne Verlängerung/Elfmeterschießen) |
| `tendenz_getroffen`, `ergebnis_getroffen`, `staerkste_ansage_getroffen` | `1` getroffen · `0` verfehlt |
| `rps` | Ranked Probability Score der 1X2-Prognose (kleiner = besser) |

Gezählt wird je Spiel die **letzte Prognose vor dem Anpfiff**; nachträglich
ändert sich keine Zeile. Methode in einem Satz: Elo für die Stärke, Poisson für
die Tore — ausführlich unter [So rechnet das Orakel](https://prorakel.de/so-funktionierts?via=github).

## Je Wettbewerb

| Wettbewerb | Spiele | Tendenz getroffen |
|---|---|---|
| Conference League | 242 | 59,5 % |
| Championship | 144 | 46,5 % |
| League One | 138 | 46,4 % |
| Europa League | 122 | 56,6 % |
| Champions League | 116 | 61,2 % |
| La Liga 2 | 115 | 50,4 % |
| 1. Lig | 115 | 46,1 % |
| Superettan | 108 | 46,3 % |
| 3. Liga | 107 | 42,1 % |
| Nations League | 104 | 62,5 % |
| I Liga | 104 | 41,3 % |
| WM 2026 | 104 | 62,5 % |
| Ekstraklasa | 103 | 45,6 % |
| Allsvenskan | 99 | 49,5 % |
| La Liga | 94 | 57,4 % |
| Saudi Pro League | 94 | 55,3 % |
| 1. Division | 90 | 58,9 % |
| DBU Pokalen | 89 | 50,6 % |
| Ligue 2 | 88 | 46,6 % |
| Eredivisie | 85 | 51,8 % |
| First NL | 79 | 38,0 % |
| 2. Bundesliga | 78 | 47,4 % |
| Serie B | 78 | 41,0 % |
| Jupiler Pro League | 76 | 61,8 % |
| Liga Portugal | 76 | 51,3 % |
| Süper Lig | 76 | 46,1 % |
| Premier League | 75 | 46,7 % |
| Serie A | 75 | 58,7 % |
| 2. Liga | 74 | 62,2 % |
| 1. Division | 71 | 42,3 % |
| Superliga | 67 | 46,3 % |
| Ligue 1 | 65 | 56,9 % |
| Eliteserien | 64 | 50,0 % |
| Super League | 63 | 55,6 % |
| Bundesliga | 61 | 55,7 % |
| Veikkausliiga | 61 | 49,2 % |
| Super League 2 | 60 | 55,0 % |
| Bundesliga | 58 | 63,8 % |
| First Division | 57 | 45,6 % |
| Premiership | 53 | 52,8 % |
| Championship | 53 | 56,6 % |
| League One | 53 | 62,3 % |
| Ykkösliiga | 51 | 60,8 % |
| Super League | 51 | 58,8 % |
| HNL | 51 | 52,9 % |
| League Two | 50 | 46,0 % |
| Schweizer Cup | 48 | 68,8 % |
| Premier Division | 46 | 58,7 % |
| Challenge League | 45 | 55,6 % |
| Puchar Polski | 37 | 54,1 % |
| ÖFB Cup | 35 | 82,9 % |
| Hrvatski kup | 33 | 69,7 % |
| Svenska Cupen | 33 | 69,7 % |
| DFB-Pokal | 32 | 71,9 % |
| Coppa Italia | 28 | 67,9 % |
| Griechischer Pokal | 28 | 71,4 % |
| Taça de Portugal | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| FAI Cup | 14 | 64,3 % |
| Scottish Cup | 14 | 42,9 % |
| Türkiye Kupası | 10 | 70,0 % |
| FA Cup | 7 | 57,1 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **4.396** | **53,5 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 25.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,5 % von 4.396 Spielen aus 64 Wettbewerben (Stand 25.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 4.396 matches from 64 competitions,
2026-06-11 to 2026-10-24, updated daily. Column names are German: `datum` date ·
`wettbewerb` competition · `heim`/`gast` home/away · `tendenz` 1/X/2 call ·
`ergebnis_prognose` most likely score · `staerkste_ansage` the statement with
the highest probability, `staerkste_ansage_wahrscheinlichkeit` its pre-match
probability · `endstand_90_min` score after 90 minutes · `…_getroffen` hit (1)
or miss (0) · `rps` ranked probability score. Licence CC BY 4.0, attribution
“Prorakel, prorakel.de”. Prorakel is an analysis service, not a gambling service.

## Lizenz

Daten: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.de)
(Volltext in `LICENSE`) — freie Nutzung mit Quellenangabe „Prorakel, prorakel.de".

Prorakel ist ein Analyse-Angebot, kein Glücksspielangebot. Die Prognosen sind
Wahrscheinlichkeiten, keine Gewissheiten.

Auch ein Orakel kennt seine Grenzen.
