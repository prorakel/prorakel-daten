# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 17.10.2026:** 3.806 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-16. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,3 % der 3.806 Spiele (2.029), die Stärkste Ansage in
75,5 % (2.875), das exakte Ergebnis in 10,9 % (413).

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
| Championship | 120 | 47,5 % |
| Europa League | 104 | 56,7 % |
| Nations League | 104 | 62,5 % |
| WM 2026 | 104 | 62,5 % |
| League One | 103 | 43,7 % |
| 1. Lig | 100 | 46,0 % |
| La Liga 2 | 99 | 46,5 % |
| Champions League | 98 | 60,2 % |
| Superettan | 96 | 45,8 % |
| I Liga | 92 | 39,1 % |
| 3. Liga | 91 | 41,8 % |
| Ekstraklasa | 90 | 44,4 % |
| DBU Pokalen | 88 | 50,0 % |
| Allsvenskan | 86 | 52,3 % |
| 1. Division | 80 | 56,2 % |
| La Liga | 79 | 55,7 % |
| Ligue 2 | 77 | 44,2 % |
| Saudi Pro League | 75 | 53,3 % |
| Eredivisie | 73 | 53,4 % |
| Jupiler Pro League | 72 | 65,3 % |
| Liga Portugal | 71 | 52,1 % |
| First NL | 66 | 39,4 % |
| 2. Bundesliga | 65 | 46,2 % |
| Süper Lig | 64 | 40,6 % |
| 2. Liga | 62 | 62,9 % |
| 1. Division | 62 | 40,3 % |
| Superliga | 61 | 47,5 % |
| Serie A | 61 | 57,4 % |
| Serie B | 61 | 42,6 % |
| Super League | 60 | 55,0 % |
| Premier League | 60 | 43,3 % |
| Ligue 1 | 55 | 56,4 % |
| First Division | 55 | 43,6 % |
| Eliteserien | 54 | 46,3 % |
| Veikkausliiga | 52 | 46,2 % |
| Bundesliga | 49 | 59,2 % |
| Super League 2 | 48 | 60,4 % |
| Bundesliga | 46 | 56,5 % |
| Ykkösliiga | 45 | 66,7 % |
| HNL | 45 | 53,3 % |
| League Two | 45 | 46,7 % |
| Championship | 44 | 56,8 % |
| League One | 44 | 61,4 % |
| Premiership | 43 | 48,8 % |
| Super League | 42 | 59,5 % |
| Challenge League | 41 | 58,5 % |
| Premier Division | 38 | 60,5 % |
| Puchar Polski | 37 | 54,1 % |
| Schweizer Cup | 36 | 66,7 % |
| ÖFB Cup | 35 | 82,9 % |
| Svenska Cupen | 33 | 69,7 % |
| DFB-Pokal | 32 | 71,9 % |
| Hrvatski kup | 32 | 68,8 % |
| Coppa Italia | 28 | 67,9 % |
| Griechischer Pokal | 28 | 71,4 % |
| FAI Cup | 14 | 64,3 % |
| Belgischer Pokal | 10 | 90,0 % |
| Türkiye Kupası | 10 | 70,0 % |
| Taça de Portugal | 9 | 77,8 % |
| Scottish Cup | 4 | 25,0 % |
| FA Cup | 2 | 100,0 % |
| DFL-Supercup | 1 | 100,0 % |
| Suomen Cup | 1 | 100,0 % |
| **Gesamt** | **3.806** | **53,3 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Zitieren

Die Nutzung ist frei, Bedingung ist die Quellenangabe. So passt sie:

> Quelle: Prorakel, [prorakel.de](https://prorakel.de/bilanz?via=zitat) · Prognose-Archiv, Stand 17.10.2026

Ein Satz zum Übernehmen — Stichprobe und Stand stehen schon drin:

> Laut dem Prognose-Archiv von Prorakel traf die vor dem Anpfiff festgelegte
> Tendenz in 53,3 % von 3.806 Spielen aus 64 Wettbewerben (Stand 17.10.2026).

Für wissenschaftliche Arbeiten liefert GitHub über „Cite this repository“
(rechte Spalte, aus `CITATION.cff`) die Angabe als APA und BibTeX.

## In English

Every pre-match forecast of the Prorakel engine (Elo ratings for team strength,
Poisson for goals), fixed before kick-off and evaluated after the final
whistle — including the misses. 3.806 matches from 64 competitions,
2026-06-11 to 2026-10-16, updated daily. Column names are German: `datum` date ·
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
