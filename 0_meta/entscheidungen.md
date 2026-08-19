---
status: laufend
stand: 2026-08-19
---

# Entscheidungen

Zwei Reihen, weil sie verschiedene Urheber und verschiedene Verbindlichkeit
haben:

- **F** — Format und Repository. Aufbau, Konventionen, Arbeitsweise. Wird von
  1789 entschieden und hier mit Begründung festgehalten.
- **E** — Inhalte. Was aus dem Playbook und dem Modul-Framework übernommen wird,
  wie es benannt und geschnitten ist. Die Spalte `durch` zeigt, wer entschieden
  hat; offene Bestätigungen stehen in `offene-punkte.md`.

## Regeln für dieses Log

**Gebündelt, nicht laufend.** Einträge entstehen einmal am Ende eines
Arbeitstages, nicht während des Gesprächs. Ein Log, das jeden Zwischenschritt
mitschreibt, wird unlesbar.

**IDs werden nie neu vergeben.** Die E-Reihe setzt die Nummerierung aus
Kapitel 9 des Modul-Frameworks fort und beginnt deshalb bei E-14. Die dort
ausgefallenen Nummern E-01, E-06 und E-08 bleiben Lücken. Die F-Reihe beginnt
bei F-01.

**Revisionen werden angehängt, nicht überschrieben.** Wird eine Entscheidung
geändert, kommt ein neuer Eintrag dazu, der auf den alten verweist. Der alte
bleibt stehen.

---

## F — Format und Repository

### 2026-08-19

| ID | Entscheidung | Begründung |
|---|---|---|
| F-01 | Sechs Ordner, vier inhaltliche Ebenen. Der Ort ergibt sich aus vier Fragen in fester Reihenfolge. | Reichweite ist das einzige Zuordnungskriterium, das nicht vom Reifegrad abhängt. Damit ist der Ort bestimmbar, ohne zu diskutieren. |
| F-02 | Dateiformat Markdown durchgehend, Frontmatter für die strukturierten Felder. | Der Inhalt ist Prosa und Tabellen. Markdown ist exportierbar, im Diff lesbar und vom Fach bearbeitbar; das Frontmatter hält die filterbaren Felder maschinell auswertbar. |
| F-03 | Ebene 2 wendet Ebene 1 an und definiert nicht neu. Keine zweite Feldliste; Felder ergänzen ist erlaubt, umbenennen, weglassen oder anders bedeuten nicht. | Felder variieren über die Modulart, nicht über den Bereich. Zwei Feldlisten wären zwei Kataloge — nicht vergleichbar und nicht generierbar. |
| F-04 | Idee und Konkretisierung stehen in derselben Datei. Getrennt wird nur, wo Instanzen vielfach und unabhängig voneinander entstehen. | Zwei Dateien, die immer gemeinsam geändert werden müssen, sind eine zu viel. |
| F-05 | Ebene 1 hält Schemata. Schema im Singular, entschiedene geschlossene Menge im Plural. | Der Dateiname zeigt den Typ, ohne die Datei zu öffnen. |
| F-06 | Jede Datei in Ebene 1 deklariert im Frontmatter `instanzen:` — `inline`, ein Ordnerpfad, oder `keine bisher`. | Ebene 1 mischt Schemata mit und ohne eigene Instanzen. Ohne Deklaration ist nicht erkennbar, ob eine Datei vollständig ist, und die Mischung driftet unbemerkt. |
| F-07 | Ein Schema verweist auf den Ordner seiner Instanzen, nie auf einzelne Dateien darin. | Der Ordnerpfad bleibt stabil; eine Dateiliste müsste bei jeder neuen Instanz angefasst werden. |
| F-08 | Status und Reifegrad stehen im Frontmatter, nicht im Ablageort. | Sonst wandern Dateien beim Reifen von Ordner zu Ordner und jeder Verweis darauf bricht. |
| F-09 | Ebene 3 gliedert nach Baustein, nicht nach Bereich: `module/<bereich>/` und `ablaeufe/`. | Module haben eine Bereichsdimension, Abläufe nicht. Ein Bereich und ein Baustein dürfen nicht auf derselben Ebene stehen. |
| F-10 | Abläufe sind ein eigener Baustein mit Schema in Ebene 1 und eigenem Ordner in Ebene 3. | Retrospektive, Krise und Konfiguration sind weder Modul noch Rolle noch Phase. Ohne eigenen Baustein bleiben sie heimatlos. |
| F-11 | Neue Bereichsordner werden erst angelegt, wenn der Bereich beauftragt ist. | Leere Platzhalter behaupten eine Vollständigkeit, die nicht da ist. |
| F-12 | Entscheidungen und offene Punkte werden getrennt geführt. IDs werden nie neu vergeben. | Verschiedene Lebensdauer. In Kapitel 9 des Frameworks und in Anhang A des Playbooks sind Nummern ausgefallen — beide Listen sind dadurch nicht zitierfähig. |
| F-13 | Dieses Log führt zwei Reihen: F für Format und Repository, E für Inhalte. Einträge entstehen gebündelt am Ende eines Arbeitstages. | Getrennte Urheber und getrennte Verbindlichkeit. Laufendes Mitschreiben macht das Log unlesbar. |
| F-14 | Nichts wird ohne Freigabe übernommen: prüfen, vorlegen, besprechen, migrieren. | Das Playbook V1.0 ist verabschiedet; stille Übernahmen mit Interpretation wären nicht mehr unterscheidbar vom Original. |
| F-15 | Die Projektleitung gibt die leere Steckbrief-Vorlage heraus, das Fach füllt aus, die Projektleitung übergibt den Rücklauf zum Auslesen. Die Datei im Repository ist danach der Datenstand; Word, PDF und Außensicht sind immer Ausgabe. | Zwei Datenstände laufen auseinander. Es kann nur einen geben. |
| F-16 | Beim Übertragen wird nichts ergänzt und nichts verloren: leere Felder bleiben leer und werden markiert, nicht zuordenbare Inhalte gehen in die offenen Punkte oder als Frage zurück. | Still verschwundene Inhalte sind das größere Risiko als falsche — falsche fallen auf. |
| F-17 | Jeder Blattordner ist repositoryweit eindeutig und nennt seinen Typ: `security-module-detailkonzept/`, `security-module-instanzen/`. Die Bausteinebene (`module/`) darf sich wiederholen. | Ein Pfadsegment wie `security/`, das an zwei Stellen vorkommt, sagt allein nicht, wo man ist — nicht in der Suche, nicht im Editor-Tab, nicht im Verweis. Ergänzt F-01. |
| F-18 | Abläufe liegen in Ebene 2, nicht in Ebene 3. **Revidiert F-10 und die Ortsangabe in E-28.** Damit ist die Grenze zwischen den Ebenen geschärft: Ebene 2 sind Konzepte, Ebene 3 sind ausgefüllte Schemata. | Ein Krisenablauf ist ein Konzepttext, kein gefülltes Formular. Die vorherige Zuordnung hätte Ebene 3 zu zwei verschiedenen Dingen gemacht. Folge: Ebene 2 ist nicht mehr nur bereichsspezifisch. |
| F-19 | Ebene 2 und Ebene 3 sind gleich gegliedert: Ebene, dann Baustein, dann die konkrete Sache. **Revidiert F-09.** | Symmetrie zwischen den Ebenen orientiert beim Navigieren. Der Preis ist, dass `module/` zweimal vorkommt; der nummerierte Elternordner macht den Pfad trotzdem eindeutig. |

---

## E — Inhalte

### 2026-08-19 · Durchgang durch die 16 Kapitel des Playbooks V1.0

| ID | Entscheidung | durch |
|---|---|---|
| E-14 | Die einleitenden Kapitel — Worum geht es, Verankerung im Unternehmen, Leitprinzipien, Geltungsbereich — gehen in den Projektkontext, nicht in ein Grundkonzept. | 1789 |
| E-15 | Veranstaltung wird Grundkonzept, mit allen drei Kategorisierungen und den Unterschieden nach Veranstalter. | 1789 |
| E-16 | Phasen wird Grundkonzept, P0 bis P7, mit den Gates an den Übergängen. | 1789 |
| E-17 | Gate wird Glossareintrag, kein eigenes Grundkonzept. Die konkreten Gates stehen in `phasen.md`. | 1789 |
| E-18 | Check-Points werden nicht übernommen. Sie sind dieselbe Art Ding wie die Übergaben eines Moduls — und nicht dasselbe wie Gates: ein Gate ist eine Bedingung an einem Phasenübergang, ein Check-Point eine Übergabe zwischen Rollen, meist innerhalb einer Phase. | 1789 |
| E-19 | Die methodische Empfehlung zum Service Blueprint wird nicht übernommen. | 1789 |
| E-20 | Rollen werden auf zwei Grundkonzepte aufgeteilt: `lead-modell.md` und `rolle.md`. | 1789 |
| E-21 | Gremium wird als Schema aufgenommen. Die konkreten Gremien sind Entwürfe und werden nicht festgeschrieben. | 1789 |
| E-22 | Eskalationspfade werden kein eigenes Grundkonzept, sondern Teil des Krisenablaufs. | 1789 |
| E-23 | Entscheidungstypen werden nicht übernommen. | 1789 |
| E-24 | `dienstleister.md` wird Grundkonzept — Kategorien und die Einordnung Pflicht / Wahl-Pflicht / Wahl. Vollständigkeit der Kategorien ist mit der Messe zu klären. | 1789 |
| E-25 | Abrechnungsmodelle werden nicht übernommen. Kein Modul braucht sie, um beschrieben zu werden; die Verrechnungseinheit ist ein Feld im Modul. | 1789 |
| E-26 | SLAs werden nicht übernommen. Dienstleistersteuerung liegt in der Linie, nicht im Modul. | 1789 |
| E-27 | Risikomanagement wird kein Grundkonzept. Die Risikostufe wird ein Feld im Modul (`niedrig / mittel / hoch`), „hoch" löst eine Pre-mortem-Pflicht aus. | 1789 |
| E-28 | Konfiguration, Krisenablauf und Lernschleife werden Abläufe in Ebene 3. Alle drei sind Entwürfe. Damit sind Krise und Triage, Retrospektiven und das Pre-mortem eingeordnet. | 1789 |
