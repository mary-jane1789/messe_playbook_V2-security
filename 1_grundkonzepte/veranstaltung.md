---
status: entwurf
stand: 2026-08-19
quelle: Playbook V1.0, Kap. 1 und 4
instanzen: inline
---

# Veranstaltung

Jede Veranstaltung wird als Projekt geführt. Drei voneinander unabhängige
Klassifikationen beschreiben sie gemeinsam: Art, Veranstalter, Größe. Eine
konkrete Veranstaltung erhält aus jeder Klassifikation genau eine Zuordnung.

Alle Arten und Veranstalter-Modelle durchlaufen dasselbe Phasenmodell
(siehe `phasen.md`). Der Veranstalter verändert die Rollenbesetzung, nicht die
Struktur.

## Art

| Art | Charakter |
|---|---|
| Kongress | agendagetrieben, ein- bis zweitägig, begrenzte Teilnehmerzahl, findet in Konferenzzentren statt |
| Corporate Event | Galas, Parteitage, Jubiläen; Bestuhlung und Ausstattung, kein Standbau; zu etwa 99 % im Modell Gast |
| Messe B2B | Fachmesse; Fachkunden, Vertriebs- und Leadgenerierungsziele |
| Messe B2C | Publikumsmesse; Einzelbesucher; in der Praxis aktuell ausschließlich im Modell Gast |

Sprachregelung: Kongress und Konferenz sind synonym, Messe B2C und
Publikumsmesse sind synonym. Der Begriff „Private Events" wird nicht verwendet.

Die Benennung der Arten ist noch nicht abschließend geklärt — offen ist, warum
die Messe auf dieser Achse nach B2B und B2C getrennt wird und ob die Messe die
Begriffe so verwendet. Die Frage steht in `../0_meta/offene-punkte.md`.

## Veranstalter

Zwei Funktionsrollen sind zu unterscheiden:

**Veranstalter** trägt die inhaltliche Konzeption, die Marke und das
wirtschaftliche Risiko und stellt nach VStättV die Veranstaltungsleitung.

**Betreiber** verantwortet das Gelände: Halle und Infrastruktur, Pflicht-Gewerke
(Elektro, Wasser, ITK, sicherheitsrelevante Leistungen), Geländesicherheit und
Logistik im Gelände.

| Modell | Veranstalter-Rolle | Betreiber-Rolle |
|---|---|---|
| Eigen | Messe | Messe |
| Gast | Gastveranstalter | Messe |
| Partner | Partner (Content und inhaltliche Ausrichtung), Durchführungshoheit bei der Messe | Messe |

## Größe

Klassifiziert wird nach Ausstellerzahl, Besucherzahl und Hallenfläche
(Brutto-Quadratmeter nach UFI-Standard).

| Klasse | Aussteller | Besucher | qm brutto |
|---|---|---|---|
| klein | 100 | 5.000 | 5.000 |
| mittel | 300 | 15.000 | 20.000 |
| groß | 1.500 | 50.000 | 100.000 |

Die Werte sind Richtwerte, keine Schwellen. Die Einstufung nimmt die für die
Veranstaltung verantwortliche Rolle vor. Die drei Werte korrelieren
typischerweise; eine Veranstaltung wird in eine Klasse einsortiert.

In V1.0 sind die Quadratmeter als Annahme und die Aussteller- und Besucherwerte
als branchen-plausibel geschätzte Hypothesen markiert.

## Was das Veranstalter-Modell verändert

**Veranstalter-Rolle bei Gast außerhalb der Messe.** Der Gastveranstalter stellt
die inhaltliche Veranstaltungsleitung, erfüllt die VStättV-Pflicht und bringt
ggf. eigene ServicePartner. Wo Messe-Rollen Gastrollen spiegeln, haben sie eine
andere Funktion und geringere Entscheidungsautorität als bei Eigen.

**Gewerke-Einordnung.** Pflicht-Gewerke laufen auch bei Gast zwingend über die
Messe. Wahl-Pflicht-Gewerke müssen erbracht werden, der Anbieter ist innerhalb
der zugelassenen Optionen wählbar. Wahl-Gewerke kann der Gast eigenständig
vergeben. Die Einordnung je Gewerk regelt `dienstleister.md`.

**Ticket-System-Isolation bei Gast.** Das Ticket-System des Gastveranstalters
wird nicht an die Messe angebunden; parallele Shops können entstehen. Für
Serviceprodukte sind Gastveranstalter an das Gast-OSC angebunden oder nutzen es
direkt.

**Partner-Hoheit.** Der Partner definiert Content und inhaltliche Ausrichtung.
Die Messe hat die Durchführungshoheit und besitzt Anteile.

## Add-ons und parallele Veranstaltungen

Add-ons verändern das Aktivitätspaket in einzelnen Phasen, nicht die
Phasenstruktur.

Eigenständige Veranstaltungen, die sich zeitlich überschneiden oder unmittelbar
aufeinander folgen, sind keine Add-ons: Jede durchläuft ihr eigenes Phasenmodell
mit eigenen Rollen. Sie erhöhen die Belastung in P3 und P4 und sind in der
Kapazitätsplanung zu berücksichtigen.
