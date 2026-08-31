---
status: entwurf
stand: 2026-08-29
quelle: Modul-Framework V0.2, Kap. 2.2; eigene Recherche zu VStättVO, § 34a GewO, vfdb 13-01, BaSiGo
---

# Rechtsrahmen

## Was hier steht

Die Belegstellen, auf die Security-Module verweisen, statt sie zu wiederholen:
Normen mit Auslöseschwellen, Fristen, externe Zustimmungen, Mitwirkende ohne
Weisungsverhältnis.

Ein Modul trägt im Feld „Rechtsgrundlage" den Verweis hierher, nicht den
Normtext. So steht jede Norm einmal, und die Fortschreibung bei einer Novelle
greift an einer Stelle.

Was hier **nicht** steht: Bemessungszahlen (siehe `bemessungsverfahren.md`),
Modulinhalte, veranstaltungsbezogene Auflagen. Auflagen entstehen je
Veranstaltung aus einer behördlichen Risikoeinstufung; sie sind Instanzdaten und
gehören in das jeweilige Modul, nicht in diese Datei.

## Geltungsbereich

Ein Standort, Geltung Deutschland. Bezugsfassung ist die
Muster-Versammlungsstättenverordnung.

Der **Fassungsstand** bleibt je Fundstelle anzugeben, weil Novellen die Inhalte
verschieben. Wo eine Landesfassung von der Musterfassung abweicht, wird die
Abweichung in der Zeile vermerkt.

## Die Tabellen sind noch leer

Jede Zeile wird einzeln freigegeben und am amtlichen Text geprüft, nicht am
Webabruf.

## Wertebereiche

Diese beiden Wertebereiche werden aus `security-modul.md` benutzt und stehen
deshalb hier nur einmal.

**Normqualität** — was die Fundstelle rechtlich ist.

| Wert | bedeutet |
|---|---|
| `Rechtsverordnung` | unmittelbar geltendes Landesrecht |
| `Verwaltungsvorschrift` | eingeführte technische Baubestimmung, keine Rechtsverordnung |
| `Gesetz` | Bundes- oder Landesgesetz |
| `Behördenauflage` | Anforderung aus dem Genehmigungsbescheid, je Veranstaltung verschieden |
| `Branchenstandard` | fachlich anerkannt, rechtlich freiwillig |
| `Hausentscheidung` | selbst gesetzt, jederzeit änderbar |

**Verbindlichkeitsstufe** — was aus der Fundstelle für das Modul folgt.

| Wert | bedeutet |
|---|---|
| `nicht unterschreitbar` | Mindestinhalt steht fest, die Ausprägung darf variieren |
| `im Einvernehmen zu bestimmen` | die Höhe wird mit einer externen Stelle festgelegt |
| `empfohlen` | fachlich begründet, ohne Bindung |
| `frei gesetzt` | Entscheidung des Hauses |

Die Unterscheidung ist nicht formal. Ohne sie wird Freiwilliges als Pflicht
geführt und Pflichtiges beim Tailoring gestrichen. Beispiel für den ersten Fall:
Die Veranstaltungsleitung hat in der Verordnung **keine** Qualifikationsanforderung
— die verbreiteten Anforderungen daran stammen aus einem Branchenstandard.

## Normen und Auflagen

| Fundstelle | Fassungsstand | Normqualität | Gegenstand | Auslöseschwelle | Art des Auslösers | Verbindlichkeitsstufe |
|---|---|---|---|---|---|---|
| | | | | | | |

Art des Auslösers: `Zahl` · `Bewertung` · `Bescheid`. Ein Gegenstand kann mehrere
Auslöser tragen; es gilt der zuerst greifende.

## Fristen

Externe Fristen sind bei Security selten ein Datum und meist eine Kette mit
Zwischenständen und einer Rückmeldezeit, die nicht in der Hand des Hauses liegt.

| Frist | Bezugspunkt | wer setzt sie | Verbindlichkeitsstufe | Folge, wenn sie reißt |
|---|---|---|---|---|
| | | | | |

## Externe Zustimmungen

| Stelle | Gegenstand | Form des Nachweises | Frist | Folge, wenn sie ausbleibt |
|---|---|---|---|---|
| | | | | |

Ob das Einvernehmen nach § 43 Abs. 2 VStättVO ein Mitentscheidungsrecht der
Behörde ist oder eine qualifizierte Abstimmungspflicht, ließ sich nicht belegen.
Bis zur Klärung wird es als Bedingung geführt, die scheitern kann.

## Mitwirkende ohne Weisungsverhältnis

Stellen, die weder eigene Rolle noch beschaffbarer Dienstleister sind und
trotzdem in den Betrieb hineinwirken.

| Stelle | Befugnis gegenüber dem Haus | Erreichbarkeit | nötiger Vorlauf |
|---|---|---|---|
| | | | |

## Offene Punkte

- Rechtsqualität des Einvernehmens nach § 43 Abs. 2 VStättVO ungeklärt.
- Wo die Dauerbestandteile geführt werden, steht in
  `../../../0_meta/offene-punkte.md`. Ein Rahmensicherheitskonzept existiert;
  welche Normzeilen daraus hierher gehören, ist beim Befüllen zu prüfen.
