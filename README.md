# Messe Playbook V2 — Security

Repository für die bereichsspezifischen Module des Operations Playbooks.
Pilotbereich ist Security.

**Stand:** Skelett angelegt, Migration der Inhalte aus Playbook V1.0 läuft.
Übertragen sind `1_grundkonzepte/veranstaltung.md` und
`1_grundkonzepte/phasen.md`. Was übernommen wird, steht in
`0_meta/entscheidungen.md`, was noch zu klären ist in `0_meta/offene-punkte.md`.

## Referenzrahmen: Eigenveranstaltung

Das Modell ist an der **Eigenveranstaltung** ausgerichtet. Playbook V1.0 legt sie
im Abschnitt Versionierung als Referenzrahmen fest; Details zu Gast-, Partner-
und B2C-Veranstaltungen folgen in späteren Ausbaustufen.

Für dieses Repository heißt das: Struktur, Bemessung und Rollenbesetzung sind für
die Eigenveranstaltung geschrieben. An einzelnen Stellen verweist das Modell auf
Gastveranstaltungen — etwa beim Gate P6 → P7 oder bei der Gewerke-Einordnung —
aber das ist die Ausnahme und jeweils am Ort vermerkt, nicht der Regelfall.
Wo eine Aussage nur für Gast oder Partner gilt, muss sie das sagen.

## Aufbau

| Ordner | Inhalt |
|---|---|
| `0_meta/` | Der Rahmen des Repositories selbst: Projektkontext, Glossar, Konventionen, Entscheidungen, offene Punkte, Quellen |
| `1_grundkonzepte/` | Was für alle Bereiche gilt — und was ein Modul ist |
| `2_detailkonzepte/` | Wo ein Grundkonzept ausdetailliert wird: `module/<bereich>-module-detailkonzept/` und `ablauf/` |
| `3_instanzen/` | Die ausgefüllten Module: `module/<bereich>-module-instanzen/` |
| `4_workspace/` | Was im Prozess ist: Entwürfe, Transkripte, Rücklauf aus dem Fach |
| `5_archiv/` | Artefakte und abgelöste Stände |

Die Ebenen 1 bis 3 verhalten sich wie allgemein zu speziell: Ein Modul in Ebene 3
verweist auf sein Detailkonzept in Ebene 2, dieses auf die Grundkonzepte in
Ebene 1. Nie umgekehrt.

Ebene 2 wendet Ebene 1 an und definiert nicht neu — in einem Bereichs-Detailkonzept
stehen dieselben drei Fragen wie im Grundkonzept, mit den Antworten dieses Bereichs.

Die Grenze zwischen Ebene 2 und 3 ist nicht bereichsspezifisch gegen
bereichsübergreifend, sondern: **Ebene 2 sind Konzepte, Ebene 3 sind ausgefüllte
Schemata.** Ein Krisenablauf ist ein Konzepttext und liegt in Ebene 2; ein
Modulsteckbrief ist ein gefülltes Formular und liegt in Ebene 3.

## Wo gehört etwas hin

Vier Fragen, in dieser Reihenfolge:

1. Beschreibt es das Repository selbst? → `0_meta/`
2. Gilt es für alle Bereiche? → `1_grundkonzepte/`
3. Detailliert es ein Grundkonzept aus — für einen Bereich oder als konkreter Ablauf? → `2_detailkonzepte/`
4. Ist es ein ausgefülltes Modul? → `3_instanzen/module/<bereich>-module-instanzen/`

Ist es noch nicht entschieden, gehört es nach `4_workspace/`.

## Wo anfangen

`0_meta/projektkontext.md` für den Zusammenhang, `0_meta/konventionen.md` für
die Regeln, `0_meta/entscheidungen.md` für das, was gilt, und
`0_meta/offene-punkte.md` für den aktuellen Klärungsbedarf.
