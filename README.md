# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 31.10.2026:** 4.730 ausgewertete Spiele aus 66 Wettbewerben,
2026-06-11 bis 2026-10-30. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,5 % der 4.730 Spiele (2.531), die Stärkste Ansage in
75,4 % (3.567), das exakte Ergebnis in 10,9 % (514).

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
| Championship | 145 | 46,9 % |
| League One | 143 | 46,9 % |
| Europa League | 122 | 56,6 % |
| 1. Lig | 121 | 46,3 % |
| La Liga 2 | 120 | 50,8 % |
| Champions League | 116 | 61,2 % |
| Superettan | 113 | 46,0 % |
| 3. Liga | 111 | 42,3 % |
| I Liga | 109 | 41,3 % |
| Allsvenskan | 109 | 49,5 % |
| Ekstraklasa | 108 | 44,4 % |
| Nations League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| Saudi Pro League | 101 | 55,4 % |
| La Liga | 100 | 58,0 % |
| 1. Division | 97 | 57,7 % |
| DBU Pokalen | 95 | 52,6 % |
| Ligue 2 | 95 | 46,3 % |
| Serie A | 90 | 61,1 % |
| Serie B | 90 | 43,3 % |
| Eredivisie | 90 | 50,0 % |
| 2. Bundesliga | 83 | 49,4 % |
| First NL | 82 | 37,8 % |
| Liga Portugal | 82 | 51,2 % |
| Süper Lig | 82 | 50,0 % |
| Jupiler Pro League | 81 | 64,2 % |
| Premier League | 80 | 47,5 % |
| 2. Liga | 76 | 61,8 % |
| Ligue 1 | 75 | 54,7 % |
| Superliga | 73 | 47,9 % |
| 1. Division | 72 | 41,7 % |
| Eliteserien | 71 | 53,5 % |
| Super League | 66 | 56,1 % |
| Veikkausliiga | 66 | 47,0 % |
| Bundesliga | 64 | 54,7 % |
| Super League 2 | 64 | 53,1 % |
| Bundesliga | 61 | 60,7 % |
| Premiership | 61 | 50,8 % |
| First Division | 59 | 47,5 % |
| Super League | 55 | 60,0 % |
| HNL | 55 | 50,9 % |
| Championship | 55 | 58,2 % |
| League One | 54 | 61,1 % |
| Puchar Polski | 53 | 47,2 % |
| Ykkösliiga | 52 | 59,6 % |
| Premier Division | 51 | 54,9 % |
| Challenge League | 50 | 56,0 % |
| League Two | 50 | 46,0 % |
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
| **Gesamt** | **4.730** | **53,5 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 31.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,5 % von 4.730 Spielen aus 66 Wettbewerben (Stand 31.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 4.730 matches from 66 competitions,
2026-06-11 to 2026-10-30, updated daily. Column names are German: `datum` date ·
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
