# Prorakel · Prognose-Archiv

Jede Prognose der [Prorakel-Engine](https://prorakel.de/so-funktionierts?via=github),
**vor dem Anpfiff festgelegt** und nach dem Abpfiff ausgewertet — auch die, die
danebenlagen. Täglich aktualisiert. Dieselben Zeilen stehen in der
[Bilanz auf prorakel.de](https://prorakel.de/bilanz?via=github).

**Stand 12.10.2026:** 3.626 ausgewertete Spiele aus 64 Wettbewerben,
2026-06-11 bis 2026-10-11. Die Tendenz (Heimsieg, Unentschieden, Auswärtssieg) traf in
53,1 % der 3.626 Spiele (1.927), die Stärkste Ansage in
75,4 % (2.733), das exakte Ergebnis in 10,8 % (393).

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
| Superettan | 95 | 45,3 % |
| La Liga 2 | 94 | 47,9 % |
| 1. Lig | 90 | 46,7 % |
| DBU Pokalen | 88 | 50,0 % |
| I Liga | 88 | 37,5 % |
| Europa League | 86 | 53,5 % |
| Ekstraklasa | 86 | 45,3 % |
| Allsvenskan | 83 | 50,6 % |
| 3. Liga | 80 | 42,5 % |
| Champions League | 80 | 58,8 % |
| La Liga | 78 | 56,4 % |
| Jupiler Pro League | 72 | 65,3 % |
| Eredivisie | 72 | 52,8 % |
| 1. Division | 72 | 55,6 % |
| Ligue 2 | 71 | 46,5 % |
| Saudi Pro League | 71 | 53,5 % |
| Liga Portugal | 70 | 52,9 % |
| First NL | 64 | 39,1 % |
| 2. Bundesliga | 63 | 47,6 % |
| Süper Lig | 62 | 38,7 % |
| Super League | 60 | 55,0 % |
| Serie B | 60 | 43,3 % |
| Superliga | 59 | 47,5 % |
| 1. Division | 59 | 40,7 % |
| Premier League | 59 | 44,1 % |
| 2. Liga | 58 | 65,5 % |
| Serie A | 58 | 55,2 % |
| Ligue 1 | 54 | 55,6 % |
| Eliteserien | 53 | 47,2 % |
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
| Super League | 41 | 61,0 % |
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
| **Gesamt** | **3.626** | **53,1 %** |

Kleine Stichproben schwanken stark — ein Wettbewerb mit wenigen Spielen sagt
wenig über die Engine.

## Lizenz

Daten: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.de) —
freie Nutzung mit Quellenangabe „Prorakel, prorakel.de".

Prorakel ist ein Analyse-Angebot, kein Glücksspielangebot. Die Prognosen sind
Wahrscheinlichkeiten, keine Gewissheiten.

Auch ein Orakel kennt seine Grenzen.
