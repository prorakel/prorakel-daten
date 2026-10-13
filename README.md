# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 13.10.2026:** 3.649 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-12. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,2 % der 3.649 Spiele (1.941), die Stärkste Ansage in
75,5 % (2.755), das exakte Ergebnis in 10,9 % (396).

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
| Conference League | 206 | 58,7 % |
| Championship | 107 | 46,7 % |
| Nations League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| League One | 102 | 44,1 % |
| La Liga 2 | 98 | 46,9 % |
| Superettan | 95 | 45,3 % |
| 1. Lig | 90 | 46,7 % |
| I Liga | 89 | 38,2 % |
| DBU Pokalen | 88 | 50,0 % |
| Ekstraklasa | 88 | 45,5 % |
| Europa League | 86 | 53,5 % |
| Allsvenskan | 85 | 51,8 % |
| 3. Liga | 80 | 42,5 % |
| Champions League | 80 | 58,8 % |
| La Liga | 78 | 56,4 % |
| Jupiler Pro League | 72 | 65,3 % |
| Ligue 2 | 72 | 45,8 % |
| Eredivisie | 72 | 52,8 % |
| 1. Division | 72 | 55,6 % |
| Liga Portugal | 71 | 52,1 % |
| Saudi Pro League | 71 | 53,5 % |
| First NL | 64 | 39,1 % |
| 2. Bundesliga | 63 | 47,6 % |
| Süper Lig | 63 | 39,7 % |
| Super League | 60 | 55,0 % |
| Superliga | 60 | 48,3 % |
| Premier League | 60 | 43,3 % |
| Serie A | 60 | 56,7 % |
| Serie B | 60 | 43,3 % |
| 1. Division | 59 | 40,7 % |
| 2. Liga | 58 | 65,5 % |
| Ligue 1 | 54 | 55,6 % |
| Eliteserien | 54 | 46,3 % |
| Veikkausliiga | 52 | 46,2 % |
| First Division | 50 | 46,0 % |
| Bundesliga | 48 | 58,3 % |
| Super League 2 | 47 | 59,6 % |
| Bundesliga | 45 | 55,6 % |
| Ykkösliiga | 45 | 66,7 % |
| League Two | 45 | 46,7 % |
| HNL | 44 | 52,3 % |
| League One | 44 | 61,4 % |
| Premiership | 43 | 48,8 % |
| Super League | 42 | 59,5 % |
| Championship | 42 | 57,1 % |
| Challenge League | 41 | 58,5 % |
| Puchar Polski | 37 | 54,1 % |
| ÖFB Cup | 35 | 82,9 % |
| Premier Division | 34 | 64,7 % |
| Svenska Cupen | 33 | 69,7 % |
| DFB-Pokal | 32 | 71,9 % |
| Hrvatski kup | 32 | 68,8 % |
| Schweizer Cup | 32 | 62,5 % |
| Coppa Italia | 28 | 67,9 % |
| Griechischer Pokal | 28 | 71,4 % |
| FAI Cup | 14 | 64,3 % |
| Türkiye Kupası | 10 | 70,0 % |
| Taça de Portugal | 7 | 85,7 % |
| Belgischer Pokal | 6 | 83,3 % |
| Scottish Cup | 4 | 25,0 % |
| FA Cup | 2 | 100,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **3.649** | **53,2 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 13.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,2 % von 3.649 Spielen aus 64 Wettbewerben (Stand 13.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 3.649 matches from 64 competitions,
2026-06-11 to 2026-10-12, updated daily. Column names are German: `datum` date ·
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
