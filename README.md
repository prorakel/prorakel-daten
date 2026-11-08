# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 08.11.2026:** 5.276 ausgewertete Spiele aus 66 Wettbewerben,
2026-06-11 bis 2026-11-07. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,8 % der 5.276 Spiele (2.836), die Stärkste Ansage in
75,4 % (3.977), das exakte Ergebnis in 10,7 % (567).

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
| Conference League | 260 | 59,6 % |
| Championship | 180 | 47,8 % |
| League One | 158 | 47,5 % |
| Europa League | 140 | 55,0 % |
| 1. Lig | 136 | 46,3 % |
| La Liga 2 | 135 | 48,9 % |
| Champions League | 134 | 64,2 % |
| Superettan | 128 | 47,7 % |
| 3. Liga | 127 | 45,7 % |
| I Liga | 122 | 41,0 % |
| Ekstraklasa | 121 | 47,1 % |
| Allsvenskan | 120 | 52,5 % |
| La Liga | 114 | 57,0 % |
| Ligue 2 | 108 | 45,4 % |
| Serie B | 107 | 43,9 % |
| 1. Division | 106 | 59,4 % |
| Serie A | 105 | 62,9 % |
| Nations League | 104 | 62,5 % |
| Saudi Pro League | 104 | 54,8 % |
| WM 2026 | 104 | 62,5 % |
| Eredivisie | 103 | 49,5 % |
| 2. Bundesliga | 96 | 50,0 % |
| DBU Pokalen | 96 | 53,1 % |
| Jupiler Pro League | 95 | 62,1 % |
| Premier League | 95 | 48,4 % |
| Süper Lig | 95 | 51,6 % |
| First NL | 94 | 37,2 % |
| Liga Portugal | 93 | 54,8 % |
| 2. Liga | 89 | 57,3 % |
| Ligue 1 | 84 | 57,1 % |
| 1. Division | 82 | 41,5 % |
| Superliga | 80 | 51,2 % |
| Eliteserien | 79 | 53,2 % |
| Bundesliga | 78 | 55,1 % |
| Super League | 75 | 54,7 % |
| Super League 2 | 74 | 54,1 % |
| Bundesliga | 69 | 60,9 % |
| Veikkausliiga | 69 | 47,8 % |
| Premiership | 68 | 48,5 % |
| Super League | 64 | 62,5 % |
| Championship | 64 | 57,8 % |
| League One | 64 | 60,9 % |
| HNL | 62 | 46,8 % |
| First Division | 60 | 46,7 % |
| League Two | 60 | 50,0 % |
| Challenge League | 55 | 56,4 % |
| Puchar Polski | 53 | 47,2 % |
| Ykkösliiga | 52 | 59,6 % |
| Premier Division | 52 | 53,8 % |
| DFB-Pokal | 48 | 70,8 % |
| Schweizer Cup | 48 | 68,8 % |
| ÖFB Cup | 43 | 72,1 % |
| Griechischer Pokal | 36 | 63,9 % |
| Hrvatski kup | 36 | 66,7 % |
| FA Cup | 35 | 62,9 % |
| Svenska Cupen | 33 | 69,7 % |
| Türkiye Kupası | 32 | 59,4 % |
| Copa del Rey | 30 | 73,3 % |
| Coppa Italia | 28 | 67,9 % |
| Taça de Portugal | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| KNVB Beker | 16 | 43,8 % |
| Scottish Cup | 15 | 40,0 % |
| FAI Cup | 14 | 64,3 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **5.276** | **53,8 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 08.11.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,8 % von 5.276 Spielen aus 66 Wettbewerben (Stand 08.11.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 5.276 matches from 66 competitions,
2026-06-11 to 2026-11-07, updated daily. Column names are German: `datum` date ·
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
