# Arbeitsanweisung

## Worum es geht

Dieses Repository enthält die bereichsspezifischen Module des Operations
Playbooks der Messe. Pilotbereich ist Security. Das Playbook V1.0 ist
verabschiedet und gilt; dieses Repository baut die Module darauf auf.

Stand: Skelett. Inhaltlich noch leer.

## Aufbau und Zuordnung

| Ordner | Inhalt |
|---|---|
| `0_meta/` | Rahmen des Repositories: Projektkontext, Glossar, Konventionen, Entscheidungen, offene Punkte, Quellen |
| `1_grundkonzepte/` | gilt für alle Bereiche, inkl. `modul.md` — was ein Modul ist |
| `2_detailkonzepte/` | Ausdetaillierung: `module/<bereich>-module-detailkonzept/` und `ablauf/` |
| `3_instanzen/` | die ausgefüllten Module: `module/<bereich>-module-instanzen/` |
| `4_workspace/` | im Prozess: Entwürfe, Transkripte, Rücklauf aus dem Fach |
| `5_archiv/` | Artefakte, abgelöste Stände |

Vier Fragen bestimmen den Ort, in dieser Reihenfolge:

1. Beschreibt es das Repository selbst? → `0_meta/`
2. Gilt es für alle Bereiche? → `1_grundkonzepte/`
3. Detailliert es ein Grundkonzept aus — für einen Bereich oder als konkreter Ablauf? → `2_detailkonzepte/`
4. Ist es ein ausgefülltes Modul? → `3_instanzen/module/<bereich>-module-instanzen/`

Noch nicht entschieden → `4_workspace/`.

Ebene 2 wendet Ebene 1 an und definiert nicht neu. Die harte Grenze: keine
zweite Feldliste. Welche Felder ein Modul hat, steuert die Modulart, nicht der
Bereich. Ein Bereich darf Felder ergänzen, aber keine aus Ebene 1 umbenennen,
weglassen oder anders bedeuten lassen.

## Regeln

**Nichts wird ohne Freigabe übernommen.** Inhalte aus dem Playbook V1.0 oder
dem Modul-Framework wandern nicht selbstständig in die Ebenen 1 bis 3. Der Weg
ist: prüfen, vorlegen, besprechen, dann migrieren.

**Der Weg eines ausgefüllten Steckbriefs.** Die Projektleitung gibt eine leere
Vorlage heraus, das Fach füllt sie aus, die Projektleitung übergibt den Rücklauf
zum Auslesen. Dabei gelten zwei Regeln:

- *Nichts ergänzen.* Was leer bleibt, bleibt leer und wird als Lücke markiert.
  Keine plausiblen Vervollständigungen.
- *Nichts verlieren.* Was das Fach geschrieben hat und in kein Feld passt, geht
  in `0_meta/offene-punkte.md` oder als Frage zurück an die Projektleitung.
  Still verschwundene Inhalte sind das größere Risiko als falsche.

Der ausgefüllte Rücklauf bleibt in `4_workspace/`, solange er ausgelesen wird,
und wandert danach als Beleg nach `5_archiv/`. Das `quelle`-Feld des Moduls
verweist darauf.

**Die Datei im Repository ist der Datenstand.** Word, PDF und Außensicht sind
immer Ausgabe, nie Eingabe. Eine ausgefüllte Vorlage gilt nicht als Wahrheit,
sondern als Beleg für den Übertrag.

**Offene Punkte werden markiert, nicht plausibel gefüllt.** Wo beim Verdichten
eine Lücke auffällt, kommt sie nach `0_meta/offene-punkte.md`. Keine
Ergänzungen aus eigener Annahme.

**Jede übernommene Aussage bekommt eine Belegstelle** im Frontmatter-Feld
`quelle`, mit Kapitel.

**Neue Ordner nur bei Beauftragung.** Keine leeren Platzhalter für Bereiche,
die noch nicht dran sind.

**Verweisen statt wiederholen.** Richtung immer von speziell zu allgemein.
Ausnahme: Ein Schema in Ebene 1 darf auf den **Ordner** seiner Instanzen zeigen,
nie auf einzelne Dateien darin — der Ordnerpfad bleibt stabil, eine Dateiliste
müsste bei jeder neuen Instanz angefasst werden.

**Jede Datei in Ebene 1 deklariert, wo ihre Instanzen liegen** — Frontmatter-Feld
`instanzen:` mit einem von drei Werten: `inline` (Schema und Ausprägungen in
derselben Datei), ein Ordnerpfad (Ausprägungen liegen dort), oder `keine bisher`
(Schema gilt, Ausprägungen noch nicht festgelegt). Ohne diese Angabe ist nicht
erkennbar, ob eine Datei vollständig ist.

**Status und Reifegrad stehen im Frontmatter, nicht im Ablageort.** Ein Entwurf
liegt am richtigen Platz und ist als Entwurf markiert. Dateien wandern beim
Reifen nicht von Ordner zu Ordner.

**Entscheidungen gehören nach `0_meta/entscheidungen.md`**, offene Punkte nach
`0_meta/offene-punkte.md`. Zwei Reihen: `F-` für Format und Repository, mit
Begründung; `E-` für Inhalte, mit der Spalte `durch`. Die E-Reihe setzt die
Nummerierung aus Kapitel 9 des Modul-Frameworks fort und beginnt bei E-14.
IDs werden nie neu vergeben; Revisionen werden angehängt, nicht überschrieben.

**Das Log wird gebündelt am Ende eines Arbeitstages geschrieben**, nicht laufend
während des Gesprächs. Während der Arbeit wird nichts mitprotokolliert.

**Konventionen gelten** wie in `0_meta/konventionen.md` beschrieben — Ordner
und Dateien klein und deutsch, Markdown mit Frontmatter.

## Sprache und Ton

Deutsch. Sachlich, präzise, praxisorientiert. Kein Beratungsjargon.
Keine Nutzenargumentation in Konzeptdateien — sie beschreiben, was gilt,
nicht warum es gut ist.

Im Gespräch: direkt, ohne Zustimmungsfloskeln und ohne Selbstkritik. Erst
nachdenken, dann antworten. Sagen, ob etwas stimmt oder nicht.
