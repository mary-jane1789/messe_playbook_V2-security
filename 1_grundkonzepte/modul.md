---
status: entwurf
stand: 2026-09-17
quelle: Modul-Framework V0.2 (nicht freigegeben); Phasen nach Playbook V1.0, Kap. 2; Risikostufe und Zustimmung nach Playbook V1.0, Kap. 9, 13, 15; Änderungen aus der ersten Befüllung am 24.08.2026 (E-63 bis E-72); Ordnung Modulgruppe → Modul → Variante nach Modullandkarte Security — konsolidiert, 08.09.2026 (E-88)
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

**Das Ergebnis ist eine Schnittprüfung, kein Steckbrieffeld.** Es entscheidet, ob
ein Kandidat ein Modul ist (Bedingung 1 unten). Im Steckbrief trägt das Feld
„Zweck und Schutzziel" diese Aussage — es ist immer formulierbar, auch bei
Dauerleistungen, und für die Bearbeitung durch das Fach die eindeutigere Frage.

## Der Schnitt

Module werden nach Ergebnis und Verantwortung geschnitten — nicht nach Phasen
und nicht nach Aufbauorganisation.

Ein Modul liegt quer zu den Phasen. Es beginnt in der strategischen Konzeption,
wird in der Feinplanung bestellt, in der Laufzeit erbracht und in der
Nachbereitung ausgewertet. Das ist der Normalfall, nicht die
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
| Modulgruppe | Ordnungsebene über dem Modul; kein Träger, kein Ergebnis, keine Verantwortung | Register des Bereichs |
| Rolle | Träger, nicht Leistung | `rolle.md`, `lead-modell.md` |
| Einzelner Prozessschritt | zu fein; erzwingt synchrone Änderung anderswo | Ablaufabschnitt innerhalb eines Moduls |
| Dokument oder Vorlage | Lieferobjekt, nicht Leistungseinheit | Feld „Lieferobjekte" des Moduls |
| Organisationseinheit | scheitert am Stabilitätstest bei der nächsten Reorganisation | Feld „Durchführung" |
| Veranstaltungsübergreifender Prozess der Organisation | Zuständigkeit CPFP | Verweis, nicht nachschreiben |
| Dauerhafte Bewertungs- oder Lagearbeit ohne Anfang und Ende | kein Ergebnis, das je vorliegt; sie ist Eingangsgröße für Module | Verweis; als Voraussetzung im Feld „Abhängigkeiten" |
| Auswahl, Vertrag und Onboarding von Dienstleistern | liegt in der Linie | Modul liefert die Anforderung |
| Querschnittsmechanik (Terminologie, Eskalationslogik) | hängt mit fast allen Modulen zusammen | Ebene 1 oder `2_detailkonzepte/ablauf/` |
| Parameterwert | ändert nur einen Wert | Feld „Parameter" des Moduls |

## Zwei Abgrenzungen

**Ein Modul ist kein Prozess.** Ein Prozess folgt dem Fluss, über
Bereichsgrenzen hinweg. Ein Modul folgt der Verantwortung und endet dort, wo
eine andere beginnt; der Prozess läuft weiter. Beides ist orthogonal: Ein Prozess
kreuzt viele Module, ein Modul kommt in vielen Prozessen vor.

Praktische Folge für das Befüllen: Was andere Verantwortliche tun, steht nicht
als Ablaufschritt, sondern als Übergabe. Im Ablauf gibt es keine parallel
weiterlaufenden Zweige — Unterschiede sind Variante oder Parameter. Und es gilt
Steuerungstiefe statt Ausführungstiefe: ein Abschnitt je Phase.

**Ein Modul ist keine Dienstleistersteuerung — aber die Beauftragung gehört
hinein.** Die Grenze verläuft zwischen Linie und Veranstaltung, nicht zwischen
Haus und Dienstleister:

| in der Linie, nicht im Modul | im Modul |
|---|---|
| Auswahl und Ausschreibung | Anforderung und Mengengerüst je Veranstaltung |
| Rahmenvertrag, Konditionen, Vertragsmanagement | konkrete Bestellung und ihr Auslöser |
| Onboarding und Grundqualifizierung | Prüfung, ob das Bestellte in Zahl, Qualifikation und Zeit geliefert wurde |

Was je Veranstaltung mit dem Dienstleister passiert — beauftragen, übergeben,
abnehmen — ist Teil des Moduls und kein eigenes Modul.

## Die Ordnung des Katalogs

Drei Ebenen, von oben nach unten: **Modulgruppe → Modul → Variante.** Darunter
liegt der Parameter als Wertebene.

| Ebene | was sie ist | was sie steuert |
|---|---|---|
| **Modulgruppe** | fachlich verwandte Module unter einem Namen | nichts. Sie ordnet und macht den Katalog lesbar |
| **Modul** | die Leistungseinheit: einzeln bestellbar, bemessbar und prüfbar, mit einem Ergebnis | alles, was ein Steckbrief trägt |
| **Variante** | Ausprägung desselben Moduls — anderer Mitteleinsatz, gleiches Ergebnis | nichts Eigenes; sie steht in der Varianten-Tabelle ihres Moduls |
| **Parameter** | ein Wert innerhalb der Ausprägung | nur diesen Wert |

**Die Modulgruppe ordnet und steuert nichts.** Sie ist kein Träger, keine
Organisationseinheit und keine Verantwortung; sie hat keinen Steckbrief, keine
Rolle und keine Pflichtstufe. Ein Modul gehört zu genau einer Gruppe. Wechselt
es die Gruppe, ändert sich am Modul selbst nichts.

**Welche Gruppen es gibt, steht nicht hier.** Der Zuschnitt ist Sache des
Bereichs und steht in seinem Register — für Security in
`../3_instanzen/module/security-module-instanzen/`. Ebene 1 sagt nur, dass es
die Ebene gibt und was sie nicht darf.

### Was am Modul hängt, ordnet den Katalog nicht

Drei Angaben stehen am einzelnen Modul. Sie sind Merkmale, keine
Gliederungsachsen: Der Katalog wird nicht nach ihnen geschnitten, und zwei
Module derselben Gruppe dürfen sich in allen dreien unterscheiden.

| Angabe | Werte | sagt |
|---|---|---|
| **Modulart** | `Compliance` \| `Leistung` | *was* das Modul ist — und damit, welche Felder Pflicht sind |
| **Pflichtstufe** | `Muss` \| `Wählen` \| `Kann` | *ob* es für eine Veranstaltung gilt |
| **Grundmodul** oder **Alternative zu** | — \| Modul-ID | ob es mit anderen Modulen eine Wahl bildet |

Compliance ist damit ein Merkmal eines Moduls und keine Ordnungsebene. Ein
Compliance-Modul und ein Leistungs-Modul stehen ohne Weiteres nebeneinander in
derselben Gruppe — bei den Ordnungs- und Wachdiensten ist genau das der Fall.

### Vier Achsen, die quer liegen

Phase, Akteur, Betriebszustand und Eskalationsstufe beschreiben ein Modul
ebenfalls, stehen aber nicht in der Hierarchie: Ein Modul liegt quer zu allen
vieren. Sie werden auf den Katalog **gemappt**, nicht in ihn eingebaut.

| Achse | Werte | steht im Modul als |
|---|---|---|
| Phase | P0 bis P7, siehe [phasen.md](phasen.md) | Deadlines und Schwerpunkt-Phase |
| Akteur | Veranstalter · Dienstleister · Genehmigungsbehörde · Gefahrenabwehr | Durchführung, Auftragsverantwortung, beteiligte Rollen, Übergaben |
| Betriebszustand | noch nicht gesetzt | Geltungsbereich, zeitlicher Teil |
| Eskalationsstufe | noch nicht gesetzt | Zusatzfeld des Security-Detailkonzepts |

### Modulart — bestimmt, welche Felder Pflicht sind

| | Compliance | Leistung |
|---|---|---|
| Zweck | rechtliche oder normative Pflicht erfüllen, Nachweis erbringen | Leistung für Kunden oder internen Auftraggeber erbringen |
| Adressat | Behörde, Geschäftsleitung | Aussteller, Gastveranstalter, interner Auftraggeber |
| Außensicht | Nachweissicht | Katalogsicht |
| Zusätzliche Pflichtfelder | Rechtsgrundlage, Auslöseschwelle, Nachweisart, Fristen, Zustimmung | Preis und Verrechnungseinheit, Bestellweg, Vorlauf- und Stornofrist, Mitwirkung, Servicezeiten |

Eine dritte Modulart für Befähigungsleistungen gibt es nicht. Die geprüften
Kandidaten — Unterweisung, Räumungsübung — sind rechtlich verlangt und damit
Compliance. Sollte in dieser Projektphase ein Baustein auftauchen, der weder
Rechtspflicht noch verkaufte Leistung ist, wird die dritte Art nachgezogen
(E-87).

Im Register darf `offen` stehen, solange die Art nicht gesetzt ist. Das ist ein
Bearbeitungsstand und keine dritte Art: Solange sie offen ist, steht nicht fest,
welche Felder Pflicht sind, und der Steckbrief wird nicht freigegeben.

### Pflichtstufe — bestimmt, ob es für eine Veranstaltung gilt

Drei Werte, in der Sprache, in der im Haus über eine Veranstaltung entschieden
wird:

| Wert | bedeutet |
|---|---|
| `Muss` | gibt es bei jeder Veranstaltung |
| `Wählen` | gibt es bei jeder Veranstaltung, aber in unterschiedlichen Ausprägungen — eine davon muss gewählt werden |
| `Kann` | gibt es bei manchen Veranstaltungen, nicht bei allen |

**Woraus eine Pflicht entsteht.** Nur aus Recht — Gesetz, Verordnung oder
Behördenauflage — oder aus einer Setzung der Messe. Ein Wunsch des Veranstalters,
des Ausstellers oder eines internen Auftraggebers erzeugt keine Pflicht, auch
wenn er im Einzelfall unabweisbar wirkt. Er wird als `Kann` geführt und im
Modul bestellt.

**Schwellen erzeugen kein Hochstufen, sondern ein anderes Modul.** Wo eine
Ausprägung ab einem Schwellenwert verlangt ist — ab einer Besucherzahl, ab einer
Risikoeinstufung, ab einer Auflage im Bescheid —, ist das ein eigenes Modul mit
der Schwelle im Namen, nicht dasselbe Modul mit gewechselter Pflichtstufe. Sonst
trägt ein Steckbrief zwei verschiedene Sollzustände und ist nicht mehr prüfbar.

### Grundmodul und Alternativen — wo mehrere Module sich gegenseitig ausschließen

Wo mehrere Module Ausprägungen derselben Sache sind und immer nur eine davon
gilt, ist eines das **Grundmodul** und die übrigen sind **Alternativen**. Das
gilt **unabhängig von der Pflichtstufe**.

Das Grundmodul trägt die Entscheidung: wer entscheidet, bis wann, und welche
Alternativen es gibt. Die Alternativen tragen nur den Rückverweis
`Alternative zu <Modul-ID>`. Damit stehen Entscheider und Frist genau einmal und
können nicht auseinanderlaufen.

**Jede Alternative ist ein eigenes Modul** mit eigener ID und eigenem
Steckbrief — das Feld `Alternativen` führt Modul-IDs. Eine Wahl besteht also aus
mindestens zwei Modulen, und alle erscheinen einzeln im Register. Ein einzelnes
Modul, dessen Ausprägungen mit derselben Anleitung laufen, ist keine Wahl,
sondern ein Modul mit einer Varianten-Tabelle. Welcher Fall vorliegt,
entscheidet der Werkstatt-Test.

**Was gilt, wenn nicht entschieden wird, hängt an der Pflichtstufe** — und das
ist der Grund, warum die beiden Angaben getrennt bleiben:

| Pflichtstufe | Wird nichts entschieden, dann … |
|---|---|
| `Wählen` | gilt das **Grundmodul**. Eine der Ausprägungen muss laufen, also greift die Vorbelegung |
| `Kann` | gilt **keine** der Ausprägungen. Das Grundmodul ist hier keine Vorbelegung, sondern die einfachste Ausprägung, falls gebucht wird |

Eine Wahl innerhalb von `Kann` ist damit ausdrücklich möglich und braucht keine
eigene Form: Zwei Kann-Module, von denen eines Grundmodul ist, sagen genau
„wenn überhaupt, dann eines von beiden".

**Welches Modul das Grundmodul ist:** die einfachste Ausprägung, die mit dem
geringsten Ressourceneinsatz auskommt.

**Die Grenze dazu:** Das Grundmodul darf nicht unter das Mindestmaß fallen, das
Recht oder Risikoeinstufung verlangen. Sonst führt eine nicht getroffene
Entscheidung zur schwächeren Ausprägung — bei sicherheitsrelevanten Modulen der
gefährlichere Fall.

**Die Entscheidungsfrist ist verbindlich gemeint.** Sie sagt, bis wann
entschieden sein muss, damit das Modul in der laufenden Planung noch greifen
kann. Sie ist damit ein Steuerungstermin und steht im Feldkatalog neben den
Deadlines, nicht bei den Feldern, die beschreiben, wie ein Modul variiert.

## Modul, Variante oder Parameter

Die häufigste Frage beim Befüllen: ein neues Modul oder nur eine Abwandlung?
Wo die Grenze liegt, entscheidet ein Test:

> Können dieselben Menschen mit **derselben Anleitung** beide Ausprägungen
> ausführen? → **Variante.**
> Bräuchte eine Vertretung **zwei verschiedene Anleitungen**? → **Zwei Module.**
> Ändert sich nur ein Wert? → **Parameter.**

Der Test ist an die Vertretungsfähigkeit gekoppelt und damit an dasselbe
Kriterium wie die Definition of Done. Modulgrenzen werden dadurch aus der Praxis
entschieden, nicht am Reißbrett.

Der Katalog selbst ist bereichsweit und stabil. Welche seiner Module für eine
einzelne Veranstaltung gelten, regelt die Pflichtstufe; mit welchen Werten sie
laufen, regeln die Parameter. Tailoring-Regeln werden als Bedingung formuliert,
nicht als Ablauftext. So sind sie prüfbar.

## Verantwortung: drei Rollen, R · A · F

Ein Modul trägt drei Verantwortungen. Sie fallen bei Security systematisch
auseinander — der Fachbereich plant, der Dienstleister führt aus, und eine
Person pflegt den Standard über Veranstaltungen hinweg. Zwei Felder genügen
dafür nicht.

| | Feld | Wer das ist | Frage, die es beantwortet |
|---|---|---|---|
| **R** | **Durchführung** | eine Rolle; kann ein Dienstleister sein | Wer erbringt die Leistung? |
| **A** | **Auftragsverantwortung** | eine Rolle im Haus | Wer steht dafür ein, dass sie erbracht wird — beauftragt, überwacht, nimmt ab? |
| **F** | **Fortschreibung** | eine Person, namentlich | Wer verantwortet das Modul im Playbook über die Zeit? |

**Durchführung (R).** Erbringt das Modul bei der Veranstaltung, von Anfang bis
Ende. Dazu eine benannte Vertretung, die im Ausfall einspringt. Bei Security ist
das häufig zu hundert Prozent der Dienstleister.

**Auftragsverantwortung (A).** Bleibt immer im Haus, auch wenn die Durchführung
vergeben ist. Sie verantwortet Anforderung und Mengengerüst, löst die Bestellung
aus oder gibt sie an die bestellende Stelle weiter, und nimmt ab, ob das
Bestellte in Zahl, Qualifikation und Zeit geliefert wurde. Ohne sie hängt eine
vergebene Leistung an niemandem.

*Wo die formale Bestellung über eine dritte Stelle läuft, bleibt die
Auftragsverantwortung dennoch hier; die Bestellung selbst ist dann ein
Ablaufabschnitt und eine Übergabe. Bei Security verantwortet 214 fachlich, die
Bestellung löst 410 aus.*

**Fortschreibung (F).** Verantwortet das Modul über die Zeit: Prüfintervall,
Änderungen, Einarbeitung der Erkenntnisse aus Retrospektiven. Steht für den
Standard ein, auch ohne ihn selbst auszuführen. Die namentliche Nennung ist eine
bewusste Abweichung vom Grundsatz, dass im Playbook nur Rollen vorkommen: Eine
Rolle, die niemand konkret besetzt, pflegt nichts.

**Warum nur R, A und F.** Das Playbook benutzt kein vollständiges RACI.
*Consulted* und *Informed* entstehen nicht als Rollenspalte, sondern als eigene
Felder — **Zustimmung** sagt, wer inhaltlich einverstanden sein muss,
**Meldeweg und Eskalation** sagt, wer erfährt was. Eine vierte und fünfte
Rollenzeile wäre die zweite Stelle für dieselbe Aussage.

Ohne Durchführung und ohne Auftragsverantwortung entsteht kein Modul. Ohne
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
| Modulgruppe | immer | Frontmatter | Pflicht | genau eine Gruppe aus dem Register des Bereichs |
| Modulname | immer | Frontmatter | Pflicht | substantivisch, ergebnisorientiert; nie Verb, Tool- oder Abteilungsname |
| Modulart | immer | Frontmatter | Pflicht | `Compliance` \| `Leistung` |
| Zweck und Schutzziel | immer | Prosa | Pflicht | wovor schützt es wen, als angestrebter Zustand. Trägt zugleich, was am Ende vorliegt |
| Geltungsbereich | immer | Prosa | Pflicht | **zeitlich**: ab wann bis wann es gilt. **räumlich**: wo es gilt. Zwei Angaben, beide erforderlich |
| Durchführung | immer | Frontmatter | Pflicht | eine Rolle; erbringt die Leistung (R) |
| Vertretung | immer | Frontmatter | Pflicht | eine Rolle, die im Ausfall der Durchführung einspringt — nicht eine, die zusätzlich eingreifen darf |
| Auftragsverantwortung | immer | Frontmatter | Pflicht | eine Rolle im Haus; beauftragt, überwacht, nimmt ab (A) |
| Fortschreibung | immer | Frontmatter | Pflicht | ein Name; pflegt das Modul über die Zeit (F) |
| Ablauf in Abschnitten | immer | Tabelle | Pflicht | je Phase ein Abschnitt, mit Auslöser, Tätigkeit, Ergebnis, Rolle |
| Lieferobjekte | immer | Tabelle | Pflicht | je Objekt ein Ablageort |

### Block 2 · Zusammenspiel — damit es an die Nachbarn anschließt

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Deadlines | immer | Tabelle | Pflicht | je Zeile: Phase, bis wann, was bis dahin entschieden oder erledigt sein muss, Ergebnis, führende Rolle |
| Entscheidungsfrist | Modul ist Grundmodul | Frontmatter | Pflicht | Zeitpunkt relativ T0, mit der Phase, in die er fällt |
| Schwerpunkt-Phase | immer | Frontmatter | Pflicht | eine oder mehrere Phasen aus P0 bis P7 |
| Übergaben rein und raus | immer | Tabelle | Pflicht | je Grenze: Richtung, Objekt, Medium, Auslöser, gebende und nehmende Rolle |
| Beteiligte Rollen | immer | Tabelle | Pflicht | je Rolle die Abschnitte, in denen sie mitwirkt |
| Abhängigkeiten | wenn vorhanden | Frontmatter | optional | `setzt voraus:` \| `nicht gemeinsam mit:` |

Die Entscheidungsfrist steht hier und nicht in Block 4: Sie ist ein Termin, bis
zu dem etwas entschieden sein muss, und beantwortet damit dieselbe Frage wie
eine Deadline-Zeile. Welche Alternativen zur Wahl stehen und wer entscheidet,
bleibt in Block 4.

Die Deadlines-Tabelle ersetzt das frühere Phasenprofil und beantwortet die Frage,
die das Lead Committee je Phase stellt: Was muss bis zum nächsten Gate
entschieden oder erledigt sein? Deshalb steht die Phase in der Zeile und nicht
als eigenes Feld darüber. Der Auslöser eines Moduls hat kein eigenes Feld — er
steht in der ersten Ablaufzeile und, wo er von anderen Modulen abhängt, unter
Abhängigkeiten.

### Block 3 · Sicherheit und Nachweis — was belegt sein muss, was schiefgehen kann

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Rechtsgrundlage | Modulart Compliance | Frontmatter | Pflicht | Norm, Paragraph, Auflage im Genehmigungsbescheid |
| Auslöseschwelle | Modulart Compliance | Prosa | Pflicht | ab wann die Pflicht greift |
| Fristen | immer | Tabelle | Pflicht bei Compliance, sonst optional | je Frist: Bezugspunkt, wer sie setzt, Verbindlichkeit, Folge wenn sie reißt. Für Ketten mit Zwischenständen und fremder Rückmeldezeit — die Termine der eigenen Planung stehen in den Deadlines |
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
| Pflichtstufe | immer | Frontmatter | Pflicht | `Muss` \| `Wählen` \| `Kann` |
| Grundmodul | Modul ist die einfachste von mehreren Ausprägungen, von denen nur eine gilt | Frontmatter | Pflicht in diesem Fall | `ja`. Unabhängig von der Pflichtstufe |
| Alternative zu | Modul ist eine Ausprägung neben einem Grundmodul | Frontmatter | Pflicht in diesem Fall | Modul-ID des Grundmoduls |
| Entscheider | Modul ist Grundmodul | Frontmatter | Pflicht | eine Rolle, gegebenenfalls im Einvernehmen mit einer zweiten |
| Alternativen | Modul ist Grundmodul | Frontmatter | Pflicht | Modul-IDs der Alternativen |
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
| Nutzen in einem Satz | Zweck und Schutzziel |
| Adressat | Modulart |
| Typischer Anlass | erste Zeile des Ablaufs |
| Enthaltene Leistung | Ablauf |
| Nicht enthalten — Abgrenzung | Geltungsbereich, Ablauf und Übergaben. Pflichtfeld, häufigste Reklamationsursache |
| Was wir vom Adressaten brauchen | Übergaben und Ablauf |
| Servicezeiten und Einsatzfenster | Geltungsbereich und Deadlines |
| Ausprägungen zur Wahl | Varianten sowie Grundmodul und Alternativen |
| Bestellweg, Vorlauffrist, Storno | nur Leistungs-Module |
| Preis und Verrechnungseinheit | nur Leistungs-Module; ohne definierte Einheit kein Preis |
| Ansprechpunkt bei Reklamation | Meldeweg |
| Version, Stand, Dokumentfreigabe | identisch mit der Innensicht |

### Kopplungsregeln

1. Beide Sichten werden gemeinsam freigegeben.
2. Jede Zusage außen hat innen eine Grundlage. Kein Servicelevel im Schaufenster
   ohne Messpunkt in der Werkstatt.
3. Jede Mitwirkungspflicht außen ist innen ein Ablaufabschnitt mit Termin.
   Bestellfrist außen entspricht einer Zeile in den Deadlines innen.
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
- Zweck und Schutzziel in einem Satz formulierbar, und die Prüffrage „Was liegt
  am Ende vor?" hat genau eine Antwort
- Geltungsbereich zeitlich **und** räumlich angegeben
- Vier-Augen-Review dokumentiert, Reviewer nicht Autor; bei Compliance-Modulen
  verpflichtend
- Übergabetest bestanden: Eine benannte Vertretung kann den Ablauf ohne
  Rückfrage ausführen
- Übergaben beidseitig bestätigt — die empfangende Rolle hat gegengezeichnet
- Mindestens eine Selbstprüfungskennzahl benannt
- Pflichtstufe formuliert, auch wenn sie `Muss` lautet
- Genau einer Modulgruppe zugeordnet, und die Modulart ist gesetzt — nicht `offen`
- Durchführung, Auftragsverantwortung und Fortschreibung benannt — R, A und F
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

Der **Zuschnitt der Modulgruppen** ist dagegen ausdrücklich Sache des Bereichs.
Er steht nicht im Detailkonzept, sondern im Register neben den Instanzen: Die
Gruppe ordnet Module, sie ändert keine Definition. Was sie nicht darf, steht
oben — ein Träger werden, eine Verantwortung tragen, Felder steuern.

Was hier als Feld steht, wird dort mit Inhalt gefüllt: Das Feld
„Rechtsgrundlage" gehört hierher, welche Normen und Auslöseschwellen bei einem
Bereich gelten, gehört ins Detailkonzept. Ebenso beim
Qualifikationsnachweis — das Feld hier, der konkrete Nachweis dort.

## Offene Punkte

Mit Stand der Klärung in `../0_meta/offene-punkte.md`.

- **Muster der Modul-ID.** Hier gilt `MOD-<BEREICH>-<NR>` (F-24). Das Register
  Security arbeitet mit sprechenden Arbeitsnummern `<BEREICH>-<GRUPPE>-<NR>`,
  weil ein Verweis damit die Gruppe mitnennt. Beides nebeneinander ist ein
  Übergangszustand: Das Muster wird gesetzt, sobald der Gruppenzuschnitt steht —
  als F-Entscheidung mit Begründung und mit einer Regel für die dann abgelösten
  IDs.
- **Der Gruppenzuschnitt ist vorläufig.** Ebene 1 sagt, dass es die Modulgruppe
  gibt; welche Gruppen ein Bereich führt und wie viele Module in eine gehören,
  entscheidet der Bereich mit dem Fachbereich. Solange das nicht bestätigt ist,
  ist die Zuordnung eines Moduls zu einer Gruppe änderbar.
- **Das Mapping auf die Querachsen steht aus.** Phase und Akteur sind als Achsen
  benannt und im Modul als Felder verankert; ein Register, das den Katalog je
  Phase oder je Akteur zeigt, gibt es noch nicht. Betriebszustand und
  Eskalationsstufe sind nicht gesetzt.
- **Vorrang zwischen Modulen.** Das Feld „Abhängigkeiten" kennt nur
  `setzt voraus` und `nicht gemeinsam mit`. Ein Modul, das andere stillstellen
  kann, hat dafür keine Form.
- **Die Schnittregeln fehlen.** Was ein Modul ist, steht hier. Wie man in der
  Praxis entscheidet, wo eines aufhört, stand im Schwesterdokument des
  Frameworks, das nicht vorliegt. Der Werkstatt-Test und die Schnittregeln im
  Security-Detailkonzept sind bisher der einzige Ersatz.
- **Übungs- und Trainingsformate** — Modul oder Linie, ungeklärt.
