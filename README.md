# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 02.11.2026:** 4.965 ausgewertete Spiele aus 66 Wettbewerben,
2026-06-11 bis 2026-11-01. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,6 % der 4.965 Spiele (2.662), die Stärkste Ansage in
75,5 % (3.747), das exakte Ergebnis in 10,8 % (534).

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
| Championship | 156 | 48,7 % |
| League One | 155 | 47,7 % |
| 1. Lig | 129 | 45,0 % |
| La Liga 2 | 127 | 48,0 % |
| Europa League | 122 | 56,6 % |
| 3. Liga | 120 | 43,3 % |
| Superettan | 118 | 46,6 % |
| Champions League | 116 | 61,2 % |
| Allsvenskan | 114 | 51,8 % |
| Ekstraklasa | 112 | 44,6 % |
| I Liga | 112 | 41,1 % |
| La Liga | 108 | 58,3 % |
| Nations League | 104 | 62,5 % |
| 1. Division | 104 | 59,6 % |
| Saudi Pro League | 104 | 54,8 % |
| WM 2026 | 104 | 62,5 % |
| Serie B | 100 | 44,0 % |
| Eredivisie | 99 | 50,5 % |
| Serie A | 98 | 63,3 % |
| Ligue 2 | 97 | 46,4 % |
| DBU Pokalen | 95 | 52,6 % |
| 2. Bundesliga | 90 | 50,0 % |
| Jupiler Pro League | 89 | 62,9 % |
| Premier League | 89 | 49,4 % |
| Süper Lig | 89 | 50,6 % |
| Liga Portugal | 88 | 53,4 % |
| First NL | 87 | 36,8 % |
| 2. Liga | 82 | 61,0 % |
| Ligue 1 | 80 | 56,2 % |
| Eliteserien | 78 | 52,6 % |
| Superliga | 77 | 49,4 % |
| 1. Division | 77 | 42,9 % |
| Bundesliga | 72 | 52,8 % |
| Super League | 72 | 54,2 % |
| Super League 2 | 71 | 52,1 % |
| Veikkausliiga | 67 | 46,3 % |
| Bundesliga | 66 | 60,6 % |
| Premiership | 64 | 50,0 % |
| Super League | 60 | 61,7 % |
| First Division | 60 | 46,7 % |
| HNL | 59 | 49,2 % |
| Championship | 59 | 59,3 % |
| League One | 59 | 61,0 % |
| League Two | 55 | 49,1 % |
| Puchar Polski | 53 | 47,2 % |
| Ykkösliiga | 52 | 59,6 % |
| Challenge League | 51 | 56,9 % |
| Premier Division | 51 | 54,9 % |
| DFB-Pokal | 48 | 70,8 % |
| Schweizer Cup | 48 | 68,8 % |
| ÖFB Cup | 43 | 72,1 % |
| Griechischer Pokal | 36 | 63,9 % |
| Hrvatski kup | 34 | 67,6 % |
| Svenska Cupen | 33 | 69,7 % |
| Türkiye Kupası | 31 | 58,1 % |
| Copa del Rey | 30 | 73,3 % |
| Coppa Italia | 28 | 67,9 % |
| Taça de Portugal | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| KNVB Beker | 16 | 43,8 % |
| Scottish Cup | 15 | 40,0 % |
| FAI Cup | 14 | 64,3 % |
| FA Cup | 7 | 57,1 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **4.965** | **53,6 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 02.11.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,6 % von 4.965 Spielen aus 66 Wettbewerben (Stand 02.11.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 4.965 matches from 66 competitions,
2026-06-11 to 2026-11-01, updated daily. Column names are German: `datum` date ·
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
