# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 11.10.2026:** 3.609 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-11. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,1 % der 3.609 Spiele (1.917), die Stärkste Ansage in
75,4 % (2.720), das exakte Ergebnis in 10,8 % (390).

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
| WM2026 | 104 | 62,5 % |
| League One | 102 | 44,1 % |
| Superettan | 95 | 45,3 % |
| La Liga 2 | 92 | 47,8 % |
| 1. Lig | 90 | 46,7 % |
| DBU Pokalen | 88 | 50,0 % |
| I Liga | 87 | 37,9 % |
| Europa League | 86 | 53,5 % |
| Ekstraklasa | 85 | 44,7 % |
| Allsvenskan | 83 | 50,6 % |
| Champions League | 80 | 58,8 % |
| 3. Liga | 79 | 43,0 % |
| La Liga | 76 | 56,6 % |
| Eredivisie | 72 | 52,8 % |
| 1. Division | 72 | 55,6 % |
| Ligue 2 | 71 | 46,5 % |
| Jupiler Pro League | 70 | 65,7 % |
| Saudi Pro League | 70 | 52,9 % |
| Liga Portugal | 68 | 51,5 % |
| First NL | 64 | 39,1 % |
| 2. Bundesliga | 63 | 47,6 % |
| Süper Lig | 62 | 38,7 % |
| Super League | 60 | 55,0 % |
| Superliga | 59 | 47,5 % |
| 1. Division | 59 | 40,7 % |
| Premier League | 59 | 44,1 % |
| Serie B | 59 | 42,4 % |
| 2. Liga | 58 | 65,5 % |
| Serie A | 57 | 56,1 % |
| Ligue 1 | 53 | 54,7 % |
| Eliteserien | 52 | 48,1 % |
| Veikkausliiga | 50 | 44,0 % |
| First Division | 50 | 46,0 % |
| Bundesliga | 48 | 58,3 % |
| Bundesliga | 45 | 55,6 % |
| Ykkösliiga | 45 | 66,7 % |
| Super League 2 | 45 | 57,8 % |
| League Two | 45 | 46,7 % |
| HNL | 44 | 52,3 % |
| League One | 44 | 61,4 % |
| Premiership | 43 | 48,8 % |
| Championship | 42 | 57,1 % |
| Challenge League | 41 | 58,5 % |
| Super League | 40 | 60,0 % |
| Puchar Polski | 37 | 54,1 % |
| ÖFB Cup | 35 | 82,9 % |
| Premier Division | 33 | 63,6 % |
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
| **Gesamt** | **3.609** | **53,1 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Lizenz

Daten: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.de) —
freie Nutzung mit Quellenangabe „Prorakel, prorakel.de".

Prorakel ist ein Analyse-Angebot, kein Glücksspielangebot. Die Prognosen sind
Wahrscheinlichkeiten, keine Gewissheiten.

Auch ein Orakel kennt seine Grenzen.
