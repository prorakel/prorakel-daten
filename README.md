# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 11.11.2026:** 5.401 ausgewertete Spiele aus 66 Wettbewerben,
2026-06-11 bis 2026-11-10. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,8 % der 5.401 Spiele (2.905), die Stärkste Ansage in
75,4 % (4.073), das exakte Ergebnis in 10,8 % (582).

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
| 1. Lig | 140 | 45,7 % |
| La Liga 2 | 139 | 48,2 % |
| Champions League | 134 | 64,2 % |
| 3. Liga | 130 | 46,9 % |
| Superettan | 128 | 47,7 % |
| I Liga | 126 | 42,1 % |
| Allsvenskan | 125 | 50,4 % |
| Ekstraklasa | 124 | 46,8 % |
| La Liga | 119 | 58,0 % |
| 1. Division | 114 | 59,6 % |
| Serie A | 110 | 62,7 % |
| Serie B | 110 | 44,5 % |
| Ligue 2 | 108 | 45,4 % |
| Eredivisie | 108 | 50,0 % |
| Nations League | 104 | 62,5 % |
| Saudi Pro League | 104 | 54,8 % |
| WM 2026 | 104 | 62,5 % |
| Premier League | 100 | 49,0 % |
| Jupiler Pro League | 99 | 62,6 % |
| 2. Bundesliga | 99 | 50,5 % |
| Süper Lig | 99 | 53,5 % |
| Liga Portugal | 97 | 55,7 % |
| DBU Pokalen | 96 | 53,1 % |
| First NL | 95 | 36,8 % |
| Ligue 1 | 90 | 54,4 % |
| 2. Liga | 89 | 57,3 % |
| Eliteserien | 86 | 52,3 % |
| Superliga | 84 | 52,4 % |
| 1. Division | 83 | 42,2 % |
| Bundesliga | 81 | 56,8 % |
| Super League 2 | 80 | 51,2 % |
| Super League | 78 | 53,8 % |
| Bundesliga | 72 | 61,1 % |
| Veikkausliiga | 72 | 48,6 % |
| Premiership | 70 | 48,6 % |
| Super League | 69 | 60,9 % |
| HNL | 64 | 48,4 % |
| Championship | 64 | 57,8 % |
| League One | 64 | 60,9 % |
| First Division | 60 | 46,7 % |
| League Two | 60 | 50,0 % |
| Challenge League | 56 | 55,4 % |
| Puchar Polski | 53 | 47,2 % |
| Ykkösliiga | 52 | 59,6 % |
| Premier Division | 52 | 53,8 % |
| DFB-Pokal | 48 | 70,8 % |
| Schweizer Cup | 48 | 68,8 % |
| ÖFB Cup | 43 | 72,1 % |
| FA Cup | 38 | 57,9 % |
| Griechischer Pokal | 36 | 63,9 % |
| Hrvatski kup | 36 | 66,7 % |
| Copa del Rey | 35 | 77,1 % |
| Svenska Cupen | 33 | 69,7 % |
| Türkiye Kupası | 32 | 59,4 % |
| Coppa Italia | 28 | 67,9 % |
| Taça de Portugal | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| KNVB Beker | 16 | 43,8 % |
| FAI Cup | 15 | 66,7 % |
| Scottish Cup | 15 | 40,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **5.401** | **53,8 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 11.11.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,8 % von 5.401 Spielen aus 66 Wettbewerben (Stand 11.11.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 5.401 matches from 66 competitions,
2026-06-11 to 2026-11-10, updated daily. Column names are German: `datum` date ·
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
