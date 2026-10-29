# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 29.10.2026:** 4.642 ausgewertete Spiele aus 66 Wettbewerben,
2026-06-11 bis 2026-10-28. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,5 % der 4.642 Spiele (2.483), die Stärkste Ansage in
75,5 % (3.504), das exakte Ergebnis in 10,8 % (502).

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
| League One | 143 | 46,9 % |
| Europa League | 122 | 56,6 % |
| La Liga 2 | 120 | 50,8 % |
| 1. Lig | 120 | 45,8 % |
| Champions League | 116 | 61,2 % |
| Superettan | 112 | 45,5 % |
| 3. Liga | 110 | 42,7 % |
| I Liga | 108 | 41,7 % |
| Ekstraklasa | 106 | 45,3 % |
| Allsvenskan | 106 | 49,1 % |
| Nations League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| La Liga | 99 | 58,6 % |
| 1. Division | 97 | 57,7 % |
| Saudi Pro League | 95 | 54,7 % |
| DBU Pokalen | 93 | 51,6 % |
| Ligue 2 | 90 | 46,7 % |
| Serie B | 90 | 43,3 % |
| Eredivisie | 90 | 50,0 % |
| Serie A | 88 | 61,4 % |
| 2. Bundesliga | 81 | 48,1 % |
| Liga Portugal | 81 | 50,6 % |
| Süper Lig | 81 | 49,4 % |
| Jupiler Pro League | 80 | 63,8 % |
| Premier League | 80 | 47,5 % |
| First NL | 79 | 38,0 % |
| 2. Liga | 74 | 62,2 % |
| Superliga | 72 | 47,2 % |
| Ligue 1 | 72 | 55,6 % |
| 1. Division | 71 | 42,3 % |
| Eliteserien | 70 | 52,9 % |
| Super League | 66 | 56,1 % |
| Veikkausliiga | 64 | 48,4 % |
| Super League 2 | 64 | 53,1 % |
| Bundesliga | 63 | 55,6 % |
| Premiership | 61 | 50,8 % |
| Bundesliga | 60 | 61,7 % |
| First Division | 59 | 47,5 % |
| Super League | 55 | 60,0 % |
| HNL | 54 | 51,9 % |
| Championship | 54 | 57,4 % |
| League One | 54 | 61,1 % |
| Ykkösliiga | 52 | 59,6 % |
| League Two | 50 | 46,0 % |
| DFB-Pokal | 48 | 70,8 % |
| Puchar Polski | 48 | 50,0 % |
| Schweizer Cup | 48 | 68,8 % |
| Challenge League | 46 | 56,5 % |
| Premier Division | 46 | 58,7 % |
| ÖFB Cup | 42 | 73,8 % |
| Griechischer Pokal | 35 | 65,7 % |
| Hrvatski kup | 34 | 67,6 % |
| Svenska Cupen | 33 | 69,7 % |
| Coppa Italia | 28 | 67,9 % |
| Türkiye Kupası | 27 | 59,3 % |
| Taça de Portugal | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| Scottish Cup | 15 | 40,0 % |
| FAI Cup | 14 | 64,3 % |
| Copa del Rey | 13 | 46,2 % |
| KNVB Beker | 13 | 46,2 % |
| FA Cup | 7 | 57,1 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **4.642** | **53,5 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 29.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,5 % von 4.642 Spielen aus 66 Wettbewerben (Stand 29.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 4.642 matches from 66 competitions,
2026-06-11 to 2026-10-28, updated daily. Column names are German: `datum` date ·
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
