---
status: entwurf
stand: 2026-09-16
---

# Konventionen

## Ordner

Klein geschrieben, deutsch, ohne Umlaute (`5_archiv`, nicht `5_Archive`),
ohne Leerzeichen. Top-Level nummeriert, damit die Sortierung der
Abstraktionsreihenfolge folgt.

**Jeder Blattordner ist repositoryweit eindeutig und nennt seinen Typ.** Nicht
`security/` an zwei Stellen, sondern `security-module-detailkonzept/` und
`security-module-instanzen/`. Der Name muss allein genügen, um zu wissen, wo man
ist — in der Suche, im Editor-Tab, im Verweis aus einer anderen Datei. Dass der
Typ damit auch im Elternordner steht, ist eine bewusste Doppelung: Ein
Pfadsegment, das nur im Zusammenhang verständlich ist, kostet bei jedem Lesen
einen Blick nach oben.

**Die Bausteinebene darf sich wiederholen.** `module/` kommt in Ebene 2 und in
Ebene 3 vor. Das ist gewollt: Die Gliederung ist auf beiden Ebenen dieselbe —
Ebene, dann Baustein, dann die konkrete Sache — und der nummerierte Elternordner
macht den Pfad eindeutig. Die Symmetrie orientiert mehr, als die Wiederholung
stört.

Neue Bereichsordner in Ebene 2 und 3 werden angelegt, wenn der Bereich
beauftragt ist — nicht vorher.

## Dateien

Klein geschrieben, Wörter mit Bindestrich getrennt, Endung `.md`:
`lead-modell.md`, `einlasskontrolle.md`.

Jeder Ordner hat eine `README.md`, die erklärt, was hineingehört. Sie ist der
Einstiegspunkt — für Menschen und für den Assistenten.

## Format

Markdown, durchgehend. Am Anfang jeder Inhaltsdatei ein Frontmatter-Block,
abgetrennt durch drei Bindestriche:

```markdown
---
status: entwurf
stand: 2026-08-19
quelle: Playbook V1.0, Kap. 2
---

# Phasen

...
```

Felder im Frontmatter:

| Feld | Bedeutung | wo Pflicht |
|---|---|---|
| `status` | Bearbeitungsstand der Datei | überall |
| `stand` | Datum der letzten inhaltlichen Änderung | überall |
| `quelle` | woher der Inhalt stammt, mit Kapitel | wo aus einem Dokument übernommen |
| `instanzen` | wo die Ausprägungen dieses Schemas liegen | in Ebene 1 |
| `id` | eindeutiger Schlüssel | bei Modulen |
| `owner` | verantwortliche Funktion | bei Modulen |

`instanzen` hat genau drei mögliche Werte:

| Wert | bedeutet |
|---|---|
| `inline` | Schema und Ausprägungen stehen in derselben Datei |
| ein Ordnerpfad | die Ausprägungen liegen in dem Ordner |
| `keine bisher` | das Schema gilt, die Ausprägungen sind noch nicht festgelegt |

Ohne diese Angabe ist beim Lesen nicht erkennbar, ob eine Datei vollständig ist
oder ihre Ausprägungen woanders stehen — und beim Erzeugen von Vorlagen nicht
maschinell auflösbar.

`quelle` ist das Feld, das den Unterschied macht: Ohne Belegstelle ist im
Zweifel nicht klärbar, ob eine Aussage aus dem verabschiedeten Playbook stammt
oder unterwegs entstanden ist.

Bei Modulen wird das Frontmatter größer. Welche Felder dort stehen, legt der
Feldkatalog in `1_grundkonzepte/modul.md` fest — nicht diese Datei. Drei Zonen:
kurze und aufzählbare Felder ins Frontmatter, wiederholte Datensätze in Tabellen
mit festen Spalten, Prosa unter feste Überschriften. Der Katalog sagt je Feld,
welche Zone gilt, weil daraus der leere Steckbrief und später die Darstellung
erzeugt werden. Er führt fünf Spalten: Feld, gilt-wenn, Zone, Pflicht oder
optional, Wertebereich.

Modul-IDs folgen dem Muster `MOD-<BEREICH>-<NR>`. Das Präfix `M-` ist für
Schemata reserviert und wird für Module nicht verwendet.

Die Modullandkarte Security nummeriert abweichend `<BEREICH>-<GRUPPE>-<NR>`,
etwa `SEC-03-01`. Das sind **Arbeitsnummern**, solange der Gruppenzuschnitt
vorläufig ist; welches Muster gilt, wird entschieden, sobald er steht (F-34).

## Verweise

Relative Pfade. Die Richtung geht immer von speziell zu allgemein: Ein Modul
verweist auf sein Detailkonzept, dieses auf ein Grundkonzept. Ein Grundkonzept
listet nicht auf, welche Module es benutzen — sonst muss es bei jedem neuen
Modul angefasst werden.

Eine Ausnahme, die keine ist: Ein Schema darf auf den **Ordner** seiner Instanzen
zeigen (`instanzen: 2_detailkonzepte/ablauf/`). Der Ordnerpfad bleibt stabil, egal
wie viele Dateien darin liegen. Auf einzelne Dateien zu zeigen wäre eine
Aufzählung und verstößt gegen die Regel.

Was an einer Stelle steht, wird nicht an einer zweiten wiederholt, sondern
verlinkt.

## Sprache

Deutsch, auch in Ordner- und Dateinamen.

## Farben und Typografie in Ausgabedateien

Für alles, was als Ausgabe entsteht — HTML-Onepager, Landkarten, Workshop-
Material —, gilt das Brand System der Messe, „Hello Opportunities". Quelle ist
`brand-system.md` im Repository `messe-playbook_v1`, Ordner `00_Meta`.

| Farbe | Hex | Rolle |
|---|---|---|
| Empowering Orange | `#F94F14` | Akzent, Interaktion, Hervorhebung |
| Embracing Red | `#E00229` | Titel und Überschriften |
| Inspirational Pink | `#F31194` | Akzent für Struktur und Gliederung |
| Navigation Red | `#DB2F00` | nur Navigations- und Fußleisten |

Neutrals: `#FFFFFF` Flächen, `#F8F8F8` Tönung, `#E5E7EB` Linien, `#6B7280`
Sekundärtext, `#000000` Text. Schrift Google Sans, Fallback Product Sans und
Figtree.

Jede Farbe trägt in einer Datei genau eine Bedeutung. Ohne diese Regel wird aus
drei Markenfarben eine bunte Fläche, in der keine Auszeichnung mehr trägt.

Die Farben sind Ausgabe, nicht Datenstand: Markdown-Dateien im Repository
bleiben ungestaltet.

## Noch offen

- Zulässige Werte für `status` bei Konzeptdateien. Für Module ist die
  Statuskette in `1_grundkonzepte/modul.md` festgelegt.
- Ausgabeformat der Steckbrief-Vorlage
- Umgang mit Versionsständen: nur in Git oder zusätzlich im Frontmatter
