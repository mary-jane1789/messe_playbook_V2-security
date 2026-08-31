---
status: entwurf, zur Abstimmung
stand: 2026-08-29
zweck: Vorschlagstext zur Frage, ob die Betriebszustände in die Phasenbeschreibung aufgenommen werden
quelle: Blueprint-Sparring 24.08.2026, Schilderung der Leitung Security; Prüfung gegen 1_grundkonzepte/phasen.md
---

# Betriebszustände — Entwurf zur Abstimmung

## Warum das hier liegt

Im Sparring am 24.08.2026 wurde nach den Betriebszuständen gefragt, und die
Antwort war eine **zeitliche** Folge, nicht eine Eskalationslogik: Nullbetrieb,
technischer Aufbau, vorgezogener Aufbau, regulärer Aufbau, Laufzeit,
Abendveranstaltung, Abbau. Für die Lageachse ist im Modulsteckbrief seither die
**Eskalationsstufe** zuständig; der Begriff Betriebszustand ist damit frei für
diese Zeitachse.

## Befund: in der Phasenbeschreibung steht das so nicht

Geprüft gegen `../1_grundkonzepte/phasen.md`:

- **P4 Aufbauphase**, `T0 −3/4 Tage bis T0`, Primär-Träger Expo Realisation und
  ServicePartner. Der einzige erläuternde Satz ist die Auflösung der Schreibweise
  („−3/4 Tage" heißt drei bis vier Tage vor T0).
- Eine Unterscheidung zwischen technischem, vorgezogenem und regulärem Aufbau
  gibt es nicht.
- **Nullbetrieb** kommt nicht vor. Die Phasen sind durchgehend relativ zu einer
  Veranstaltung bemessen; der Zustand ohne Veranstaltung liegt außerhalb.
- **Abendveranstaltung** kommt nicht vor. P5 ist mit `T0 bis letzter
  Laufzeittag` bemessen, ohne Tagesstruktur.

Die drei Aufbau-Zustände liegen zudem alle innerhalb von P4 und teilweise
davor — der vorgezogene Aufbau beginnt vor dem Fenster von P4. Die
Betriebszustände sind damit keine feinere Unterteilung der Phasen, sondern eine
zweite Achse, die sich mit ihnen überlappt.

## Was im Sparring geschildert wurde

Ohne Interpretation, in der Reihenfolge der Schilderung:

| Zustand | was ihn ausmacht | wer im Vordergrund steht |
|---|---|---|
| Nullbetrieb | keine Veranstaltung auf dem Gelände. Nur Mitarbeitende und Firmen für Renovierung und Technik. Zutritt über Personenvereinzelungsanlagen und Ausweis, alle anderen über die Pforte | Geländeschutz, SCU |
| Technischer Aufbau | Vertragsfirmen ertüchtigen die bespielten Hallen: Technik, Strom, Licht, Rigging. Läuft nach dem Hallenplan, noch ohne Aussteller. Findet nach jeder Veranstaltung statt, nicht nur nach der Sommerpause | Veranstaltungstechnik |
| Vorgezogener Aufbau | Aussteller mit besonderem Aufwand bauen früher auf, gegen Aufschlag. Ab hier greifen Sicherheitsmaßnahmen: Zutrittsausweise, erste Hallenstreifen | Security, Arbeitsschutz, Diebstahlschutz |
| Regulärer Aufbau | Aufbau freigegeben. Logistiksteuerung an den Toren, hohe Dichte an Dienstleistern in den Hallen, Zutrittskontrolle über QR-Code oder Badge. Ausgangskontrollen gibt es heute nicht | Logistik und Security |
| Laufzeit | Veranstaltung geöffnet. Einlass eine Stunde vor Öffnung, Aussteller früher. Geländestreifen, Raucherbereiche, Rettungs- und Fluchtwege. Tägliche Lagebesprechung vor Beginn | Veranstaltungsleitung nach VStättV |
| Abendveranstaltung | nach dem Messetag, meist nahtlos anschließend. Andere Regeln: eher Event-Security, präventiv gegen alkoholbedingte Auseinandersetzungen | Ordnungsdienstleiter |
| Abbau | hoher Zeitdruck, weil die nächste Veranstaltung wartet. Safety steht im Vordergrund; erhöhtes Risiko von Diebstahl durch Innentäter | ServicePartner, Security |

## Drei Optionen

**A · Nichts tun.** Die Betriebszustände bleiben ungeschrieben. Jedes Modul
benennt im Feld „Geltungsbereich, zeitlich" den Zustand, den es meint, in
eigenen Worten.
*Kosten:* Die Wörter driften. Drei Module beschreiben denselben Zeitraum
verschieden, und beim Zusammensetzen einer Veranstaltung fällt das erst spät
auf.

**B · Als Abschnitt in `phasen.md`.** Ein kurzer Abschnitt „Betriebszustände"
mit der Tabelle oben und dem Satz, dass Phase und Betriebszustand zwei Achsen
sind, die sich überlappen.
*Kosten:* `phasen.md` ist aus V1.0 migriert und trägt bisher nur, was dort
belegt ist. Die Betriebszustände stehen in V1.0 nicht — sie kämen als erste
Aussage aus dem Haus dazu, mit dem Sparring als Beleg. Das ist zulässig, muss
aber im `quelle`-Feld sichtbar sein.

**C · Eigenes Grundkonzept `betriebszustand.md`.** Neben `phasen.md`, mit
`instanzen: inline`.
*Kosten:* Ein Grundkonzept mehr, für das der Gegentest aus
`1_grundkonzepte/README.md` erst zu bestehen ist: Nimm es weg — lässt sich ein
Modul dann noch schreiben? Vermutlich ja, solange der Geltungsbereich ihn in
Worten trägt.

## Empfehlung

**B**, aber erst, wenn ein zweites Modul den Zustand tatsächlich braucht. Beim
Testmodul Personenkontrolle genügte die Formulierung „über die gesamte
Einlasszeit". Ein Konzept, das auf Verdacht angelegt wird, ist teurer als eines,
das eine Woche später aus einem echten Bedarf entsteht.

Was jetzt schon gilt und keine Entscheidung braucht: Der Begriff
**Betriebszustand** ist für diese Zeitachse reserviert und wird nicht mehr für
die Lage benutzt. Das steht im Security-Detailkonzept.

## Was zu entscheiden ist

- Option A, B oder C.
- Falls B oder C: Ist die Tabelle oben inhaltlich richtig? Sie gibt eine
  mündliche Schilderung wieder und ist nicht gegengelesen.
- Gehört der Nullbetrieb überhaupt ins Playbook? Er ist nicht
  veranstaltungsbezogen und fällt damit unter dieselbe Abgrenzung wie das
  Lagebild und die SCU.
