# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 27.11.2026:** 5.910 ausgewertete Spiele aus 67 Wettbewerben,
2026-06-11 bis 2026-11-26. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
54,1 % der 5.910 Spiele (3.197), die Stärkste Ansage in
75,3 % (4.452), das exakte Ergebnis in 11,0 % (648).

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
| Conference League | 278 | 59,7 % |
| Championship | 204 | 48,0 % |
| League One | 180 | 47,8 % |
| La Liga 2 | 161 | 49,7 % |
| Europa League | 158 | 55,7 % |
| Nations League | 156 | 64,1 % |
| Champions League | 152 | 64,5 % |
| 1. Lig | 150 | 47,3 % |
| 3. Liga | 140 | 50,0 % |
| I Liga | 135 | 40,7 % |
| Allsvenskan | 134 | 50,0 % |
| Ekstraklasa | 133 | 46,6 % |
| Serie B | 130 | 43,8 % |
| Superettan | 130 | 47,7 % |
| La Liga | 129 | 58,1 % |
| Serie A | 120 | 62,5 % |
| Ligue 2 | 117 | 47,0 % |
| Eredivisie | 117 | 50,4 % |
| 1. Division | 117 | 59,0 % |
| Premier League | 110 | 49,1 % |
| Jupiler Pro League | 108 | 63,0 % |
| 2. Bundesliga | 108 | 50,0 % |
| Saudi Pro League | 108 | 54,6 % |
| Süper Lig | 108 | 54,6 % |
| WM 2026 | 104 | 62,5 % |
| First NL | 103 | 36,9 % |
| Ligue 1 | 99 | 52,5 % |
| 2. Liga | 97 | 56,7 % |
| Liga Portugal | 97 | 55,7 % |
| DBU Pokalen | 96 | 53,1 % |
| Super League 2 | 96 | 52,1 % |
| Eliteserien | 94 | 50,0 % |
| Bundesliga | 90 | 57,8 % |
| Superliga | 90 | 54,4 % |
| 1. Division | 90 | 42,2 % |
| Super League | 84 | 53,6 % |
| Bundesliga | 78 | 60,3 % |
| Premiership | 78 | 51,3 % |
| Super League | 76 | 63,2 % |
| League One | 74 | 63,5 % |
| Veikkausliiga | 72 | 48,6 % |
| Championship | 72 | 58,3 % |
| HNL | 69 | 50,7 % |
| League Two | 69 | 49,3 % |
| Challenge League | 61 | 57,4 % |
| First Division | 60 | 46,7 % |
| Puchar Polski | 54 | 48,1 % |
| Ykkösliiga | 52 | 59,6 % |
| Premier Division | 52 | 53,8 % |
| DFB-Pokal | 48 | 70,8 % |
| Schweizer Cup | 48 | 68,8 % |
| Copa del Rey | 43 | 74,4 % |
| ÖFB Cup | 43 | 72,1 % |
| FA Cup | 38 | 57,9 % |
| Hrvatski kup | 38 | 63,2 % |
| Taça de Portugal | 38 | 55,3 % |
| Griechischer Pokal | 36 | 63,9 % |
| Svenska Cupen | 33 | 69,7 % |
| Türkiye Kupası | 32 | 59,4 % |
| Coppa Italia | 28 | 67,9 % |
| Coupe de France | 25 | 56,0 % |
| Belgischer Pokal | 22 | 81,8 % |
| KNVB Beker | 16 | 43,8 % |
| FAI Cup | 15 | 66,7 % |
| Scottish Cup | 15 | 40,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **5.910** | **54,1 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 27.11.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 54,1 % von 5.910 Spielen aus 67 Wettbewerben (Stand 27.11.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 5.910 matches from 67 competitions,
2026-06-11 to 2026-11-26, updated daily. Column names are German: `datum` date ·
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
