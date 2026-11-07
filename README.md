# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 07.11.2026:** 5.121 ausgewertete Spiele aus 66 Wettbewerben,
2026-06-11 bis 2026-11-06. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,7 % der 5.121 Spiele (2.751), die Stärkste Ansage in
75,4 % (3.863), das exakte Ergebnis in 10,7 % (550).

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
| Championship | 169 | 47,9 % |
| League One | 158 | 47,5 % |
| Europa League | 140 | 55,0 % |
| Champions League | 134 | 64,2 % |
| 1. Lig | 132 | 45,5 % |
| La Liga 2 | 131 | 48,1 % |
| 3. Liga | 121 | 43,8 % |
| Superettan | 120 | 47,5 % |
| I Liga | 119 | 40,3 % |
| Allsvenskan | 118 | 52,5 % |
| Ekstraklasa | 117 | 47,0 % |
| La Liga | 110 | 58,2 % |
| Ligue 2 | 105 | 45,7 % |
| 1. Division | 105 | 59,0 % |
| Nations League | 104 | 62,5 % |
| Saudi Pro League | 104 | 54,8 % |
| WM 2026 | 104 | 62,5 % |
| Serie A | 101 | 63,4 % |
| Serie B | 101 | 43,6 % |
| Eredivisie | 100 | 50,0 % |
| DBU Pokalen | 96 | 53,1 % |
| 2. Bundesliga | 92 | 50,0 % |
| Jupiler Pro League | 91 | 62,6 % |
| Premier League | 91 | 49,5 % |
| First NL | 91 | 37,4 % |
| Liga Portugal | 91 | 54,9 % |
| Süper Lig | 91 | 50,5 % |
| 2. Liga | 86 | 58,1 % |
| Ligue 1 | 82 | 56,1 % |
| 1. Division | 80 | 42,5 % |
| Superliga | 79 | 50,6 % |
| Eliteserien | 78 | 52,6 % |
| Bundesliga | 73 | 53,4 % |
| Super League | 72 | 54,2 % |
| Super League 2 | 72 | 52,8 % |
| Veikkausliiga | 69 | 47,8 % |
| Bundesliga | 67 | 61,2 % |
| Premiership | 64 | 50,0 % |
| Super League | 62 | 61,3 % |
| HNL | 60 | 48,3 % |
| First Division | 60 | 46,7 % |
| Championship | 60 | 60,0 % |
| League One | 59 | 61,0 % |
| League Two | 55 | 49,1 % |
| Challenge League | 54 | 57,4 % |
| Puchar Polski | 53 | 47,2 % |
| Ykkösliiga | 52 | 59,6 % |
| Premier Division | 51 | 54,9 % |
| DFB-Pokal | 48 | 70,8 % |
| Schweizer Cup | 48 | 68,8 % |
| ÖFB Cup | 43 | 72,1 % |
| Griechischer Pokal | 36 | 63,9 % |
| Hrvatski kup | 36 | 66,7 % |
| Svenska Cupen | 33 | 69,7 % |
| Türkiye Kupası | 32 | 59,4 % |
| Copa del Rey | 30 | 73,3 % |
| Coppa Italia | 28 | 67,9 % |
| Taça de Portugal | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| KNVB Beker | 16 | 43,8 % |
| Scottish Cup | 15 | 40,0 % |
| FAI Cup | 14 | 64,3 % |
| FA Cup | 9 | 55,6 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **5.121** | **53,7 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 07.11.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,7 % von 5.121 Spielen aus 66 Wettbewerben (Stand 07.11.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 5.121 matches from 66 competitions,
2026-06-11 to 2026-11-06, updated daily. Column names are German: `datum` date ·
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
