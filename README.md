# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 22.11.2026:** 5.717 ausgewertete Spiele aus 67 Wettbewerben,
2026-06-11 bis 2026-11-21. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
54,0 % der 5.717 Spiele (3.085), die Stärkste Ansage in
75,3 % (4.303), das exakte Ergebnis in 10,8 % (618).

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
| Championship | 191 | 48,2 % |
| League One | 175 | 48,0 % |
| Nations League | 156 | 64,1 % |
| La Liga 2 | 155 | 49,0 % |
| 1. Lig | 145 | 45,5 % |
| Europa League | 140 | 55,0 % |
| 3. Liga | 137 | 49,6 % |
| Champions League | 134 | 64,2 % |
| I Liga | 131 | 41,2 % |
| Superettan | 130 | 47,7 % |
| Ekstraklasa | 129 | 45,7 % |
| Allsvenskan | 129 | 49,6 % |
| La Liga | 124 | 58,1 % |
| Serie B | 118 | 44,1 % |
| Ligue 2 | 115 | 47,0 % |
| 1. Division | 115 | 59,1 % |
| Serie A | 114 | 64,0 % |
| Eredivisie | 113 | 49,6 % |
| Premier League | 107 | 48,6 % |
| 2. Bundesliga | 105 | 50,5 % |
| Saudi Pro League | 105 | 54,3 % |
| Jupiler Pro League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| Süper Lig | 103 | 53,4 % |
| First NL | 101 | 36,6 % |
| 2. Liga | 97 | 56,7 % |
| Liga Portugal | 97 | 55,7 % |
| DBU Pokalen | 96 | 53,1 % |
| Ligue 1 | 96 | 53,1 % |
| Super League 2 | 91 | 52,7 % |
| Eliteserien | 90 | 51,1 % |
| 1. Division | 89 | 42,7 % |
| Bundesliga | 88 | 58,0 % |
| Superliga | 85 | 52,9 % |
| Super League | 81 | 55,6 % |
| Premiership | 76 | 50,0 % |
| Bundesliga | 75 | 61,3 % |
| League One | 74 | 63,5 % |
| Veikkausliiga | 72 | 48,6 % |
| Championship | 72 | 58,3 % |
| Super League | 70 | 61,4 % |
| League Two | 69 | 49,3 % |
| HNL | 66 | 50,0 % |
| Challenge League | 61 | 57,4 % |
| First Division | 60 | 46,7 % |
| Puchar Polski | 53 | 47,2 % |
| Ykkösliiga | 52 | 59,6 % |
| Premier Division | 52 | 53,8 % |
| DFB-Pokal | 48 | 70,8 % |
| Schweizer Cup | 48 | 68,8 % |
| Copa del Rey | 43 | 74,4 % |
| ÖFB Cup | 43 | 72,1 % |
| FA Cup | 38 | 57,9 % |
| Hrvatski kup | 38 | 63,2 % |
| Griechischer Pokal | 36 | 63,9 % |
| Svenska Cupen | 33 | 69,7 % |
| Taça de Portugal | 33 | 51,5 % |
| Türkiye Kupası | 32 | 59,4 % |
| Coppa Italia | 28 | 67,9 % |
| Coupe de France | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| KNVB Beker | 16 | 43,8 % |
| FAI Cup | 15 | 66,7 % |
| Scottish Cup | 15 | 40,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **5.717** | **54,0 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 22.11.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 54,0 % von 5.717 Spielen aus 67 Wettbewerben (Stand 22.11.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 5.717 matches from 67 competitions,
2026-06-11 to 2026-11-21, updated daily. Column names are German: `datum` date ·
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
