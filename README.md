# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 18.10.2026:** 3.969 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-17. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,3 % der 3.969 Spiele (2.117), die Stärkste Ansage in
75,5 % (2.997), das exakte Ergebnis in 10,8 % (427).

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
| Europa League | 104 | 56,7 % |
| Nations League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| La Liga 2 | 103 | 48,5 % |
| 1. Lig | 102 | 45,1 % |
| Superettan | 100 | 46,0 % |
| Champions League | 98 | 60,2 % |
| 3. Liga | 97 | 40,2 % |
| I Liga | 95 | 41,1 % |
| Ekstraklasa | 93 | 44,1 % |
| DBU Pokalen | 88 | 50,0 % |
| Allsvenskan | 87 | 51,7 % |
| La Liga | 83 | 55,4 % |
| Ligue 2 | 80 | 45,0 % |
| 1. Division | 80 | 56,2 % |
| Saudi Pro League | 77 | 51,9 % |
| Eredivisie | 76 | 53,9 % |
| Jupiler Pro League | 72 | 65,3 % |
| First NL | 71 | 38,0 % |
| Liga Portugal | 71 | 52,1 % |
| 2. Bundesliga | 69 | 47,8 % |
| Süper Lig | 68 | 44,1 % |
| Serie B | 67 | 41,8 % |
| 2. Liga | 65 | 61,5 % |
| Premier League | 65 | 44,6 % |
| 1. Division | 64 | 42,2 % |
| Serie A | 64 | 57,8 % |
| Superliga | 61 | 47,5 % |
| Super League | 60 | 55,0 % |
| Ligue 1 | 58 | 56,9 % |
| Veikkausliiga | 57 | 47,4 % |
| Eliteserien | 57 | 47,4 % |
| First Division | 55 | 43,6 % |
| Bundesliga | 52 | 55,8 % |
| Bundesliga | 51 | 60,8 % |
| Ykkösliiga | 50 | 62,0 % |
| Super League 2 | 50 | 58,0 % |
| League Two | 50 | 46,0 % |
| League One | 49 | 61,2 % |
| Premiership | 48 | 47,9 % |
| Championship | 48 | 56,2 % |
| HNL | 47 | 53,2 % |
| Super League | 43 | 58,1 % |
| Schweizer Cup | 42 | 69,0 % |
| Challenge League | 41 | 58,5 % |
| Premier Division | 39 | 59,0 % |
| Puchar Polski | 37 | 54,1 % |
| ÖFB Cup | 35 | 82,9 % |
| Svenska Cupen | 33 | 69,7 % |
| DFB-Pokal | 32 | 71,9 % |
| Hrvatski kup | 32 | 68,8 % |
| Coppa Italia | 28 | 67,9 % |
| Griechischer Pokal | 28 | 71,4 % |
| Belgischer Pokal | 17 | 88,2 % |
| Taça de Portugal | 17 | 70,6 % |
| FAI Cup | 14 | 64,3 % |
| Türkiye Kupası | 10 | 70,0 % |
| FA Cup | 6 | 50,0 % |
| Scottish Cup | 4 | 25,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **3.969** | **53,3 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 18.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,3 % von 3.969 Spielen aus 64 Wettbewerben (Stand 18.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 3.969 matches from 64 competitions,
2026-06-11 to 2026-10-17, updated daily. Column names are German: `datum` date ·
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
