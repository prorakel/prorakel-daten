# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 19.10.2026:** 4.083 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-18. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,5 % der 4.083 Spiele (2.183), die Stärkste Ansage in
75,6 % (3.085), das exakte Ergebnis in 10,8 % (440).

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
| Conference League | 224 | 59,8 % |
| Championship | 131 | 48,1 % |
| League One | 114 | 45,6 % |
| La Liga 2 | 108 | 49,1 % |
| 1. Lig | 106 | 45,3 % |
| Europa League | 104 | 56,7 % |
| Nations League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| Superettan | 102 | 47,1 % |
| 3. Liga | 100 | 40,0 % |
| Champions League | 98 | 60,2 % |
| I Liga | 98 | 41,8 % |
| Ekstraklasa | 96 | 43,8 % |
| Allsvenskan | 92 | 51,1 % |
| DBU Pokalen | 88 | 50,0 % |
| 1. Division | 88 | 58,0 % |
| La Liga | 87 | 57,5 % |
| Eredivisie | 81 | 51,9 % |
| Ligue 2 | 80 | 45,0 % |
| Saudi Pro League | 78 | 51,3 % |
| Jupiler Pro League | 72 | 65,3 % |
| 2. Bundesliga | 72 | 48,6 % |
| First NL | 72 | 38,9 % |
| Liga Portugal | 71 | 52,1 % |
| Süper Lig | 71 | 45,1 % |
| Serie B | 70 | 41,4 % |
| Premier League | 69 | 46,4 % |
| Serie A | 68 | 57,4 % |
| 2. Liga | 66 | 60,6 % |
| Superliga | 65 | 44,6 % |
| 1. Division | 65 | 43,1 % |
| Ligue 1 | 63 | 57,1 % |
| Eliteserien | 62 | 50,0 % |
| Super League | 60 | 55,0 % |
| Veikkausliiga | 58 | 48,3 % |
| First Division | 55 | 43,6 % |
| Bundesliga | 54 | 63,0 % |
| Bundesliga | 54 | 57,4 % |
| Super League 2 | 54 | 55,6 % |
| Ykkösliiga | 50 | 62,0 % |
| League Two | 50 | 46,0 % |
| HNL | 49 | 55,1 % |
| Premiership | 49 | 49,0 % |
| League One | 49 | 61,2 % |
| Super League | 48 | 60,4 % |
| Championship | 48 | 56,2 % |
| Schweizer Cup | 48 | 68,8 % |
| Challenge League | 41 | 58,5 % |
| Premier Division | 39 | 59,0 % |
| Puchar Polski | 37 | 54,1 % |
| ÖFB Cup | 35 | 82,9 % |
| Svenska Cupen | 33 | 69,7 % |
| DFB-Pokal | 32 | 71,9 % |
| Hrvatski kup | 32 | 68,8 % |
| Coppa Italia | 28 | 67,9 % |
| Griechischer Pokal | 28 | 71,4 % |
| Taça de Portugal | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| FAI Cup | 14 | 64,3 % |
| Türkiye Kupası | 10 | 70,0 % |
| FA Cup | 6 | 50,0 % |
| Scottish Cup | 4 | 25,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **4.083** | **53,5 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 19.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,5 % von 4.083 Spielen aus 64 Wettbewerben (Stand 19.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 4.083 matches from 64 competitions,
2026-06-11 to 2026-10-18, updated daily. Column names are German: `datum` date ·
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
