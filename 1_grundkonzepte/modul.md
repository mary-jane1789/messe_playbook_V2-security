---
status: entwurf
stand: 2026-08-23
quelle: Modul-Framework V0.2 (nicht freigegeben); Phasen nach Playbook V1.0, Kap. 2; Risikostufe und Zustimmung nach Playbook V1.0, Kap. 9, 13, 15
instanzen: 3_instanzen/module/
---

# Modul

## Was ein Modul ist

Ein Modul ist keine Gliederungsebene des Playbooks, sondern die kleinste
eigenständig verantwortbare Leistungseinheit eines Bereichs — mit einem Namen,
einer Durchführungsverantwortung, einem definierten Ergebnis, prüfbaren
Übergabepunkten und zwei Sichten: einer Innensicht für die Erbringung und einer
daraus abgeleiteten Außensicht.

Glossarfähige Langfassung:

> **Modul** — Eine dauerhaft benannte, eigenständig verantwortbare
> Leistungseinheit eines operativen Bereichs. Sie erbringt ein definiertes
> Ergebnis für einen benannten Adressaten, ist über Veranstaltungen hinweg
> wiederverwendbar, wird über standardisierte Übergabepunkte in die
> Veranstaltungsdurchführung eingebunden und wird in einer Innensicht
> (Erbringung) und einer daraus abgeleiteten Außensicht (Leistungsversprechen
> oder Nachweis) beschrieben.

## Der Schnitt

Module werden nach Ergebnis und Verantwortung geschnitten — nicht nach Phasen
und nicht nach Aufbauorganisation.

Ein Modul liegt quer zu den Phasen. Ein Sicherheitsmodul beginnt in der
strategischen Konzeption, wird in der Feinplanung bestellt, in der Laufzeit
erbracht und in der Nachbereitung ausgewertet. Das ist der Normalfall, nicht die
Ausnahme. Ein Schnitt entlang der Phasen erzeugt Bausteine, die nur in Reihe
funktionieren; ein Schnitt entlang der Bereiche erzeugt Bausteine, die niemand
allein verantworten kann.

## Die fünf Bedingungen

Ein Kandidat ist erst ein Modul, wenn alle fünf erfüllt sind.

| | Bedingung | Prüffrage |
|---|---|---|
| 1 | **Ein Ergebnis** | Auf die Frage „Was liegt am Ende vor?" gibt es eine Antwort, nicht zwei. Wer zwei Dinge aufzählen muss, hat zwei Module vor sich. |
| 2 | **Eine Durchführungsverantwortung** | Gibt es genau eine Rolle, die es von Anfang bis Ende verantwortet? |
| 3 | **Wiederverwendbar** | Kommt es bei mehr als einer Veranstaltung in gleicher Grundgestalt vor? |
| 4 | **Definierte Übergaben** | Sind Eingang und Ausgang mit Objekt, Medium, Auslöser und Rollen beschreibbar? |
| 5 | **Eigener Treiber** | Gibt es einen Grund, warum es ein eigener Baustein ist — Rechtspflicht, Varianzträger, Verkaufbarkeit, Personenrisiko, gezielte Weiterentwicklung? |

„Kleinste" ist durch Bedingung 1 und 2 begrenzt: die kleinste Einheit, die noch
ein Ergebnis und eine Durchführungsverantwortung trägt. Nicht kleiner — sonst
entstehen Splitter, die einzeln nichts leisten.

## Was kein Modul ist

| Kein Modul | Warum | Wohin |
|---|---|---|
| Phase (P0 bis P7) | Zeitabschnitt, nicht Leistung. Module wirken in Phasen und laufen quer dazu | `phasen.md` |
| Rolle | Träger, nicht Leistung | `rolle.md`, `lead-modell.md` |
| Einzelner Prozessschritt | zu fein; erzwingt synchrone Änderung anderswo | Ablaufabschnitt innerhalb eines Moduls |
| Dokument oder Vorlage | Lieferobjekt, nicht Leistungseinheit | Feld „Lieferobjekte" des Moduls |
| Organisationseinheit | scheitert am Stabilitätstest bei der nächsten Reorganisation | Feld „Durchführung" |
| Veranstaltungsübergreifender Prozess der Organisation | Zuständigkeit CPFP | Verweis, nicht nachschreiben |
| Dienstleisterauswahl und -steuerung | liegt in der Linie | Modul liefert die Anforderung |
| Querschnittsmechanik (Terminologie, Eskalationslogik) | hängt mit fast allen Modulen zusammen | Ebene 1 oder `2_detailkonzepte/ablauf/` |
| Parameterwert | ändert nur einen Wert | Feld „Parameter" des Moduls |

## Drei Abgrenzungen

**Ein Modul ist kein Prozess.** Ein Prozess folgt dem Fluss, über
Bereichsgrenzen hinweg. Ein Modul folgt der Verantwortung und endet dort, wo
eine andere beginnt; der Prozess läuft weiter. Beides ist orthogonal: Ein Prozess
kreuzt viele Module, ein Modul kommt in vielen Prozessen vor.

Praktische Folge für das Befüllen: Was andere Verantwortliche tun, steht nicht
als Ablaufschritt, sondern als Übergabe. Im Ablauf gibt es keine Verzweigungen —
Unterschiede sind Variante oder Parameter. Und es gilt Steuerungstiefe statt
Ausführungstiefe: vier bis acht Abschnitte, je Abschnitt eine Rolle und ein
Ergebnis.

**Ein Modul ist keine Dienstleistersteuerung.** Auswahl, Vertrag und
Qualitätssteuerung liegen in der Linie. Das Modul liefert die Anforderung, die
Linie beschafft und steuert.

**Ein Modul ist kein Controlling-Objekt.** Kennzahlen im Modul dienen der
Selbstprüfung des ausführenden Teams. Sie sind kein Instrument der
Leistungsbewertung durch die Führung.

Eine Grenze der dritten Abgrenzung: Bei Compliance-Modulen ist die Abweichung
von einer Frist oder einer Behördenauflage nichts, was das Team mit sich selbst
klärt. Sie ist meldepflichtig an eine benannte Rolle. Das ist kein Controlling,
sondern Weitergabe von Haftung.

## Zwei Einordnungen

Ein Modul wird auf zwei unabhängigen Achsen eingeordnet. Die Trennung ist
nötig, weil sonst vermischt wird, *was* ein Modul ist, und *ob* es für eine
Veranstaltung gilt.

### Modulart — bestimmt, welche Felder Pflicht sind

| | Compliance | Leistung |
|---|---|---|
| Zweck | rechtliche oder normative Pflicht erfüllen, Nachweis erbringen | Leistung für Kunden oder internen Auftraggeber erbringen |
| Adressat | Behörde, Geschäftsleitung | Aussteller, Gastveranstalter, interner Auftraggeber |
| Außensicht | Nachweissicht | Katalogsicht |
| Zusätzliche Pflichtfelder | Rechtsgrundlage, Auslöseschwelle, Nachweisart, Fristen, Zustimmung | Preis und Verrechnungseinheit, Bestellweg, Vorlauf- und Stornofrist, Mitwirkung, Servicezeiten |

Bei Compliance-Modulen gilt: Die Bindung darf nicht unter die Rechtsschwelle,
die Ausprägung darf variieren.

Ob eine dritte Modulart für Befähigungsleistungen gebraucht wird, ist offen und
mit der Messe zu klären.

### Bindung — bestimmt, ob es für eine Veranstaltung gilt

Vier Werte:

| Wert | bedeutet |
|---|---|
| `gilt immer` | ohne Ausnahme aktiv |
| `gilt auf Bedarf, wenn …` | aktiv bei benanntem Auslöser |
| `Wahlpflicht — Grundmodul` | Normalfall einer Wahl; gilt, solange nichts anderes entschieden ist |
| `Wahlpflicht — Alternative zu …` | tritt an die Stelle eines Grundmoduls, mit Rückverweis darauf |

**Wie eine Wahlpflicht funktioniert.** Von mehreren Alternativen ist eine das
Grundmodul. Sie trägt die Entscheidung: wer entscheidet, bis wann, und welche
Alternativen es gibt. Die Alternativen tragen nur den Rückverweis auf das
Grundmodul. Damit stehen Entscheider und Frist genau einmal und können nicht
auseinanderlaufen.

Wird nichts entschieden, gilt das Grundmodul. Ist eine Alternative gewählt, ist
die Entscheidung getroffen und die Frage erledigt.

**Welches Modul das Grundmodul ist:** die einfachste Variante, die mit dem
geringsten Ressourceneinsatz auskommt.

**Die Grenze dazu:** Das Grundmodul darf nicht unter eine Pflichtschwelle
fallen. Wo Recht oder Risikoeinstufung eine Mindestausprägung verlangen, gilt
diese, nicht die Vorbelegung. Sonst führt eine nicht getroffene Entscheidung zur
schwächeren Ausprägung — bei sicherheitsrelevanten Modulen der gefährlichere
Fall.

**Die Entscheidungsfrist ist verbindlich gemeint.** Sie sagt, bis wann
entschieden sein muss, damit das Modul in der laufenden Planung noch greifen
kann.

## Modul, Variante, Parameter

Drei Ebenen:

1. **Modulkatalog** — welche Bausteine existieren. Bereichsweit, stabil.
2. **Modulauswahl je Veranstaltung** — welche gelten. Das regelt die Bindung.
3. **Parametrisierung** — mit welchen Werten der gewählte Baustein läuft.

Wo die Grenze liegt, entscheidet ein Test:

> Können dieselben Menschen mit **derselben Anleitung** beide Ausprägungen
> ausführen? → **Variante.**
> Bräuchte eine Vertretung **zwei verschiedene Anleitungen**? → **Zwei Module.**
> Ändert sich nur ein Wert? → **Parameter.**

Der Test ist an die Vertretungsfähigkeit gekoppelt und damit an dasselbe
Kriterium wie die Definition of Done. Modulgrenzen werden dadurch aus der Praxis
entschieden, nicht am Reißbrett.

Tailoring-Regeln werden als Bedingung formuliert, nicht als Ablauftext. So sind
sie prüfbar.

## Verantwortung: Durchführung und Fortschreibung

Ein Modul hat zwei Verantwortungen mit unterschiedlicher Lebensdauer. Sie werden
getrennt geführt.

**Durchführung** — eine Rolle. Verantwortet, dass das Modul bei der
Veranstaltung erbracht wird, von Anfang bis Ende. Dazu eine benannte Vertretung.

**Fortschreibung** — eine Person, namentlich. Verantwortet das Modul über die
Zeit: Prüfintervall, Änderungen, Einarbeitung der Erkenntnisse aus
Retrospektiven.

Die namentliche Nennung bei der Fortschreibung ist eine bewusste Abweichung vom
Grundsatz, dass im Playbook nur Rollen vorkommen. Eine Rolle, die niemand
konkret besetzt, pflegt nichts.

Ohne Durchführungsverantwortung entsteht kein Modul. Ohne
Fortschreibungsverantwortung wird kein Steckbrief freigegeben.

## Übergaben

Jede Modulgrenze wird mit vier Angaben beschrieben. Übergaben brauchen ein
benanntes Trägermedium und eine verantwortliche Rolle — sonst passieren sie über
den kürzesten Weg.

| Angabe | was darin steht |
|---|---|
| Übergabeobjekt | was übergeben wird |
| Übergabemedium | worüber: Formular, Plan, Protokoll, Besprechung |
| Auslöser | woran erkennbar ist, dass die Übergabe fällig ist |
| Rollen | gebende Rolle → nehmende Rolle |

## Der Feldkatalog

**Eine Datenquelle, zwei Sichten.** Die Innensicht ist der führende Datensatz.
Die Außensicht ist eine gefilterte Ansicht darauf, kein zweites Dokument.

**Zwei Ausbaustufen.** Block 1 und 2 bilden den Kurzsteckbrief — davon kann ein
Team bereits arbeiten. Die Blöcke 3 bis 5 wachsen beim Befüllen und bei der
ersten Anwendung. Zehn gefüllte Felder sind mehr wert als dreißig halbe.

Felder, die für die Modulart nicht gelten, werden ausgeblendet, nicht leer
gelassen.

**Zone** sagt, wo das Feld in der Datei steht: `Frontmatter` für kurze und
aufzählbare Werte, `Tabelle` für wiederholte Datensätze, `Prosa` für Text unter
einer festen Überschrift.

### Block 1 · Kern — damit überhaupt jemand handeln kann

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Modul-ID | immer | Frontmatter | Pflicht | `MOD-<BEREICH>-<NR>` |
| Modulname | immer | Frontmatter | Pflicht | substantivisch, ergebnisorientiert; nie Verb, Tool- oder Abteilungsname |
| Modulart | immer | Frontmatter | Pflicht | `Compliance` \| `Leistung` |
| Ergebnis | immer | Prosa | Pflicht | ein Satz: „Fertig ist, wenn …" |
| Zweck und Schutzziel | immer | Prosa | Pflicht | Freitext: wovor schützt es wen |
| Durchführung | immer | Frontmatter | Pflicht | eine Rolle |
| Vertretung | immer | Frontmatter | Pflicht | eine Rolle |
| Fortschreibung | immer | Frontmatter | Pflicht | ein Name |
| Auslöser | immer | Prosa | Pflicht | Freitext: woran erkennt man, dass es losgeht |
| Ablauf in Abschnitten | immer | Tabelle | Pflicht | 4 bis 8 Abschnitte; je Abschnitt Auslöser, Tätigkeit, Ergebnis, Rolle; keine Verzweigungen |
| Lieferobjekte | immer | Tabelle | Pflicht | je Objekt ein Ablageort |

### Block 2 · Zusammenspiel — damit es an die Nachbarn anschließt

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Phasenprofil | immer | Tabelle | Pflicht | eine Zeile je beteiligter Phase: Phase, was passiert, Ergebnis am Phasenende, führende Rolle |
| Auslöser-Phase | immer | Frontmatter | Pflicht | eine Phase aus P0 bis P7 |
| Schwerpunkt-Phase | immer | Frontmatter | Pflicht | eine oder mehrere Phasen aus P0 bis P7 |
| Übergaben rein und raus | immer | Tabelle | Pflicht | je Grenze: Richtung, Objekt, Medium, Auslöser, gebende und nehmende Rolle |
| Beteiligte Rollen | immer | Tabelle | Pflicht | je Rolle die Abschnitte, in denen sie mitwirkt |
| Abhängigkeiten | wenn vorhanden | Frontmatter | optional | `setzt voraus:` \| `nicht gemeinsam mit:` |

### Block 3 · Sicherheit und Nachweis — was belegt sein muss, was schiefgehen kann

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Rechtsgrundlage | Modulart Compliance | Frontmatter | Pflicht | Norm, Paragraph, Auflage im Genehmigungsbescheid |
| Auslöseschwelle | Modulart Compliance | Prosa | Pflicht | ab wann die Pflicht greift |
| Nachweise und Dokumentation | immer | Tabelle | Pflicht bei Compliance, sonst optional | je Nachweis: was, Aufbewahrungsdauer, Änderungsvermerk von wem und wann |
| Meldeweg und Eskalation | immer | Prosa | Pflicht bei Compliance, sonst optional | wer erfährt was über welchen Weg; zwei unabhängige Erreichbarkeitswege. Abweichung von Rechtspflicht oder Auflage ist meldepflichtig an eine benannte Rolle. Verweist auf `../2_detailkonzepte/ablauf/` |
| Qualifikationsnachweis vor Einsatz | immer | Frontmatter | Pflicht | `ja` \| `nein`; bei `ja` welcher Nachweis vor Dienstbeginn vorliegen muss |
| Zustimmung | immer | Frontmatter | Pflicht | eine oder mehrere Stellen, die inhaltlich einverstanden sein müssen |
| Startbedingung | immer | Prosa | Pflicht | was erfüllt sein muss, damit der Einsatz beginnen darf |
| Abbruchkriterien | immer | Prosa | Pflicht | wann der Einsatz abgebrochen wird; dokumentierte Abweichung mit Begründung, Befristung und Genehmiger |
| Risikostufe | immer | Frontmatter | Pflicht | `niedrig` \| `mittel` \| `hoch`. `hoch` löst eine Pre-mortem-Pflicht aus |
| Risiken | immer | Tabelle | Pflicht | je Risiko eine Gegenmaßnahme |

### Block 4 · Anpassung — wie es je Veranstaltung variiert

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Bindung | immer | Frontmatter | Pflicht | die vier Werte oben |
| Entscheider | Bindung ist Wahlpflicht-Grundmodul | Frontmatter | Pflicht | eine Rolle, gegebenenfalls im Einvernehmen mit einer zweiten |
| Entscheidungsfrist | Bindung ist Wahlpflicht-Grundmodul | Frontmatter | Pflicht | Zeitpunkt relativ T0 |
| Alternativen | Bindung ist Wahlpflicht-Grundmodul | Frontmatter | Pflicht | Modul-IDs der Alternativen |
| statt | Bindung ist Wahlpflicht-Alternative | Frontmatter | Pflicht | Modul-ID des Grundmoduls |
| Varianten | wenn vorhanden | Tabelle | optional | Ausprägungen, die mit derselben Anleitung laufen |
| Parameter | wenn vorhanden | Tabelle | optional | je Parameter ein Wertebereich |
| Bemessungsregel | immer | Prosa | Pflicht | Schlüsselzahl oder Rechenweg, mit Quelle |
| Ressourcenbedarf | immer | Tabelle | Pflicht | je Phase: internes Personal, Budget |

### Block 5 · Lernen und Pflege — damit es nicht veraltet

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Selbstprüfungskennzahl | immer | Tabelle | Pflicht | höchstens zwei, prozessbegleitend messbar, für das ausführende Team |
| Nachbereitung und Rückkopplung | immer | Prosa | Pflicht | Debrief-Fragen und wohin die Erkenntnis fließt |
| Offene Lücken | immer | Prosa | Pflicht | benannt oder ausdrücklich „keine"; nicht leer |
| Reifegrad | immer | Frontmatter | Pflicht | Ist und Ziel, je `1` bis `4` |
| Version | immer | Frontmatter | Pflicht | — |
| Stand | immer | Frontmatter | Pflicht | Datum |
| Prüfintervall | immer | Frontmatter | Pflicht | Compliance-Module häufiger als der Rest |
| Dokumentfreigabe | immer | Frontmatter | Pflicht | wer diesen Steckbrief in dieser Version freigegeben hat |

## Die Außensicht

Die Außensicht wird abgeleitet, nicht neu erfunden. Bei Leistungs-Modulen ist
sie eine Katalogsicht, bei Compliance-Modulen eine Nachweissicht: gleiche
Struktur, Adressat ist Behörde oder Geschäftsleitung, Preis- und Bestellfelder
entfallen, an ihre Stelle treten Auflagen-, Mitwirkungs- und Erfüllungsnachweis.

| Feld der Außensicht | abgeleitet aus |
|---|---|
| Name in Adressatensprache, mit Synonymen | Modulname |
| Nutzen in einem Satz | Ergebnis und Zweck |
| Adressat | Modulart |
| Typischer Anlass | Auslöser |
| Enthaltene Leistung | Ablauf |
| Nicht enthalten — Abgrenzung | Ablauf und Übergaben. Pflichtfeld, häufigste Reklamationsursache |
| Was wir vom Adressaten brauchen | Übergaben und Ablauf |
| Servicezeiten und Einsatzfenster | Phasenprofil |
| Ausprägungen zur Wahl | Bindung und Varianten |
| Bestellweg, Vorlauffrist, Storno | nur Leistungs-Module |
| Preis und Verrechnungseinheit | nur Leistungs-Module; ohne definierte Einheit kein Preis |
| Ansprechpunkt bei Reklamation | Meldeweg |
| Version, Stand, Dokumentfreigabe | identisch mit der Innensicht |

### Kopplungsregeln

1. Beide Sichten werden gemeinsam freigegeben.
2. Jede Zusage außen hat innen eine Grundlage. Kein Servicelevel im Schaufenster
   ohne Messpunkt in der Werkstatt.
3. Jede Mitwirkungspflicht außen ist innen ein Ablaufabschnitt mit Termin.
   Bestellfrist außen entspricht einem Vorlauf-Gate innen.
4. Änderungen laufen innen zuerst. Außen wird neu erzeugt.
5. Verständlichkeitsprüfung als Freigabekriterium: Zwei Leser müssen die
   Leistungsbeschreibung im gleichen Sinne verstehen.
6. Referenzieren statt duplizieren. Bestehende Konzepte werden verlinkt, nicht
   nachgeschrieben; das Modul enthält dann Verweis, Verantwortung und Prüfstand.

## Lebenszyklus

**Bevor ein Entwurf entsteht** wird geprüft: Passt der Kandidat in ein
bestehendes Modul? Sind die fünf Bedingungen erfüllt? Wer trägt die
Durchführung? Ohne Durchführungsverantwortung kein Entwurf.

**Statuskette:** `Entwurf` → `Geprüft` → `Freigegeben` → `In Überarbeitung` →
`Abgelöst`. `Geprüft` heißt: Vier-Augen-Review und Übergabetest bestanden.

Eine Verprobung an einer echten Veranstaltung ist nicht Teil der Beauftragung.
Ein Modul erreicht `Freigegeben` auf Basis von Review und Übergabetest, nicht
auf Basis eines gelaufenen Einsatzes.

### Definition of Done

- Alle Felder der Ausbaustufe gefüllt oder als offene Lücke markiert — keine
  leeren Felder ohne Vermerk
- Ergebnis in einem Satz formulierbar
- Vier-Augen-Review dokumentiert, Reviewer nicht Autor; bei Compliance-Modulen
  verpflichtend
- Übergabetest bestanden: Eine fachfremde Vertretung kann den Ablauf ohne
  Rückfrage ausführen
- Übergaben beidseitig bestätigt — die empfangende Rolle hat gegengezeichnet
- Mindestens eine Selbstprüfungskennzahl benannt
- Bindung formuliert, auch wenn sie `gilt immer` lautet
- Fortschreibungsverantwortung benannt
- Im Modulindex registriert, Ablageort und Version gesetzt
- Bei Compliance-Modulen: Rechtsgrundlage, Nachweisart und Zustimmung belegt

### Reifegrade

| | Stufe | Woran man es sieht |
|---|---|---|
| 1 | Personengebunden | funktioniert, ist aber nicht dokumentiert; hängt an Einzelpersonen |
| 2 | Beschrieben | Steckbrief vorhanden, Verantwortung benannt; je Veranstaltung individuell ausgelegt |
| 3 | Angewendet | wird aus dem Standard getailort, Gates nachweisbar, Vertretung funktioniert, das Team prüft sich selbst |
| 4 | Fortgeschrieben | Erkenntnisse aus Veranstaltungen ändern nachweisbar den Standard |

Die Zielstufe wird je Modul festgelegt. Für viele Module ist 3 der richtige
Endpunkt, nicht 4. Innerhalb des Projekts erreichbar ist Stufe 2 für alle
bearbeiteten Module; Stufe 3 entsteht erst, wenn der Standard bei einer
Veranstaltung benutzt wird.

Die Bewertung erfolgt im gemeinsamen Termin, nicht per Selbstauskunft.

## Was ein Detailkonzept ergänzen darf

Dies ist das Grundkonzept. Es gilt für alle Bereiche. Je Bereich entsteht in
`2_detailkonzepte/module/` ein Detailkonzept, das es anwendet.

Ein Detailkonzept darf **Felder ergänzen**. Es darf Felder aus diesem Katalog
nicht umbenennen, nicht weglassen und nicht anders bedeuten lassen. Welche
Felder ein Modul hat, steuert die Modulart — nicht der Bereich.

Was hier als Feld steht, wird dort mit Inhalt gefüllt: Das Feld
„Rechtsgrundlage" gehört hierher, welche Normen und Auslöseschwellen bei einem
Bereich gelten, gehört ins Detailkonzept. Ebenso beim
Qualifikationsnachweis — das Feld hier, der konkrete Nachweis dort.

## Offene Punkte

Vier Stellen sind noch nicht entschieden. Sie stehen mit Stand der Klärung in
`../0_meta/offene-punkte.md`.

- **Dritte Modulart** für Befähigungsleistungen — mit der Messe zu klären.
- **Keine erprobten Beispiele.** Das Framework ist an keinem echten Modul
  getestet; seine Beispiele waren durchgehend hypothetisch und sind hier
  deshalb nicht übernommen.
- **Die Schnittregeln fehlen.** Was ein Modul ist, steht hier. Wie man in der
  Praxis entscheidet, wo eines aufhört, stand im Schwesterdokument des
  Frameworks, das nicht vorliegt. Der Werkstatt-Test ist bisher der einzige
  Ersatz.
- **Übungs- und Trainingsformate** — Modul oder Linie, ungeklärt.
