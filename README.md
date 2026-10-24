# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 24.10.2026:** 4.240 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-23. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,7 % der 4.240 Spiele (2.277), die Stärkste Ansage in
75,8 % (3.212), das exakte Ergebnis in 10,7 % (453).

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
| Championship | 133 | 48,1 % |
| League One | 126 | 47,6 % |
| Europa League | 122 | 56,6 % |
| Champions League | 116 | 61,2 % |
| 1. Lig | 111 | 45,9 % |
| La Liga 2 | 110 | 50,0 % |
| Superettan | 105 | 46,7 % |
| Nations League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| 3. Liga | 101 | 40,6 % |
| I Liga | 100 | 42,0 % |
| Ekstraklasa | 99 | 43,4 % |
| Allsvenskan | 95 | 50,5 % |
| Saudi Pro League | 91 | 56,0 % |
| La Liga | 90 | 56,7 % |
| DBU Pokalen | 89 | 50,6 % |
| 1. Division | 89 | 58,4 % |
| Ligue 2 | 86 | 46,5 % |
| Eredivisie | 82 | 52,4 % |
| First NL | 75 | 38,7 % |
| 2. Bundesliga | 74 | 47,3 % |
| Liga Portugal | 73 | 52,1 % |
| Süper Lig | 73 | 45,2 % |
| 2. Liga | 72 | 62,5 % |
| Jupiler Pro League | 72 | 65,3 % |
| Premier League | 71 | 46,5 % |
| Serie A | 71 | 57,7 % |
| Serie B | 71 | 40,8 % |
| Superliga | 67 | 46,3 % |
| 1. Division | 67 | 43,3 % |
| Ligue 1 | 64 | 56,2 % |
| Eliteserien | 62 | 50,0 % |
| Super League | 60 | 55,0 % |
| Veikkausliiga | 59 | 49,2 % |
| Super League 2 | 56 | 55,4 % |
| Bundesliga | 55 | 63,6 % |
| Bundesliga | 55 | 56,4 % |
| First Division | 55 | 43,6 % |
| Ykkösliiga | 51 | 60,8 % |
| League Two | 50 | 46,0 % |
| HNL | 49 | 55,1 % |
| Premiership | 49 | 49,0 % |
| Championship | 49 | 55,1 % |
| League One | 49 | 61,2 % |
| Super League | 48 | 60,4 % |
| Schweizer Cup | 48 | 68,8 % |
| Premier Division | 46 | 58,7 % |
| Challenge League | 44 | 56,8 % |
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
| Türkiye Kupası | 10 | 70,0 % |
| FA Cup | 7 | 57,1 % |
| Scottish Cup | 4 | 25,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **4.240** | **53,7 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 24.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,7 % von 4.240 Spielen aus 64 Wettbewerben (Stand 24.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 4.240 matches from 64 competitions,
2026-06-11 to 2026-10-23, updated daily. Column names are German: `datum` date ·
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
