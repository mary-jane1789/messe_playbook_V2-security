---
status: entwurf
stand: 2026-09-17
quelle: Modul-Framework V0.2, Kap. 2.2 (Rechtsrahmen, behördliche Anschlussfähigkeit, verkaufbare Leistung); eigene Recherche zu VStättVO, § 34a GewO, vfdb 13-01, BaSiGo, DSGVO und zur Praxis deutscher Messegesellschaften; anonymisiertes veranstaltungsbezogenes Sicherheitskonzept in `../../../0_meta/quellen/` als Realprobe
---

# Security-Modul

## Was diese Datei tut

Sie sagt, was ein Security-Modul über `../../../1_grundkonzepte/modul.md` hinaus
braucht, und worauf zu achten ist, wenn eines geschrieben wird.

Sie definiert nichts neu. Die harte Grenze aus `../../README.md` gilt: keine
zweite Feldliste. Was hier steht, sind ergänzende Felder und Ausfüllhinweise zu
Feldern, die es in Ebene 1 bereits gibt.

Der Maßstab für jeden Satz hier: **Stimmt er beim nächsten Bereich auch?** Wenn
ja, gehört er nach `1_grundkonzepte/` und nicht hierher. Wo die Antwort unsicher
ist, steht es dabei.

## Warum Security zusätzliche Angaben braucht

Drei Eigenschaften, aus denen sich alles Weitere ableitet.

**Fremde Autorität.** Norm, Behörde und Genehmigungsbescheid bestimmen Existenz,
Mindestinhalt, Frist und Freigabe eines Moduls. Der Bescheid kann Anforderungen
über die Verordnung hinaus stellen und die Verordnungsschwelle auch nach unten
unterlaufen. Ein Security-Modul ist damit nach oben offen: seine Sollbeschreibung
ist nie abschließend aus der Norm ableitbar.

**Wirkung auf und Bindung an Personen.** Die Leistung schränkt Menschen ein und
hängt an namentlich benannten, anwesenden, behördlich geprüften Personen. Die
Bußgeldbewehrung trifft diese Personen einzeln, nicht die Organisation.

**Umschaltung zur Laufzeit.** Lage, Betriebszustand und Eskalationsstufe ändern
sich innerhalb einer Veranstaltung, nicht nur zwischen Phasen. Wer ein Modul
führt, kann davon abhängen.

## Die vier Zusatzangaben

Spalten wie im Feldkatalog in `modul.md`. Diese Felder gelten zusätzlich für
Module des Bereichs Security.

| Feld | gilt-wenn | Zone | Pflicht | Wertebereich |
|---|---|---|---|---|
| Befugnisgrundlage | immer | Prosa | Pflicht | worauf sich die Maßnahme gegenüber Dritten stützt und wo sie endet. Zu nennen: die Grundlage (Hausrecht, vertragliche Einwilligung, Jedermannsrecht, behördliche Anordnung) und die Grenze — was das Modul ausdrücklich nicht darf |
| Verhalten je Eskalationsstufe | immer | Tabelle | Pflicht | je Eskalationsstufe eine Zeile: Stufe, was mit dem Modul geschieht (läuft weiter, ändert die Ausprägung, ruht), wer es auf dieser Stufe führt |
| Handlungsvollmacht ohne Rückfrage | immer | Tabelle | Pflicht | je Maßnahme eine Zeile: Maßnahme, auslösende Rolle, Voraussetzung, wer sie beendet, wer unverzüglich informiert wird. Wenn es keine gibt: ausdrücklich „keine" |
| Rechtlich verantwortliche Stelle | Modul wird auch bei Gastveranstaltungen eingesetzt | Frontmatter | Pflicht | die Stelle, die die Pflicht rechtlich trägt, wenn sie nicht mit der Durchführung zusammenfällt |

### Zu Befugnisgrundlage

Ein Ordnungsdienst hat keine hoheitlichen Befugnisse. § 34a Abs. 5 GewO lässt
Wachpersonen ausdrücklich nur die Jedermannsrechte — Notwehr, Notstand,
Selbsthilfe. Alles darüber hinaus, Zutrittsverweigerung und Taschenkontrolle
eingeschlossen, läuft über das Hausrecht und die Einwilligung, die mit dem
Betreten erklärt wird.

Ohne dieses Feld beschreibt das Modul eine Handlung, ohne zu sagen, warum sie
zulässig ist. Kein anderer Bereich schränkt Menschen ein; deshalb kennt Ebene 1
das Feld nicht.

### Zu Verhalten je Eskalationsstufe

Der Grund für dieses Feld: Die Verantwortung für ein Security-Modul ist keine
Konstante, sondern hängt davon ab, wie weit die Lage eskaliert ist. Im
Regelbetrieb verantwortet der Veranstalter; im Schadensfall greift die
Gefahrenabwehrbehörde ein und behandelt die Lage als Krisenfall.

**Drei Achsen, drei Wörter — sie werden nicht vermischt.**

| Achse | Wort | wo sie geführt wird |
|---|---|---|
| Zeit, grob | **Phase** | P0 bis P7 in `../../../1_grundkonzepte/phasen.md`; im Modul über die Deadlines |
| Zeit, fein | **Betriebszustand** | Nullbetrieb, Aufbau, Laufzeit, Abbau — die Folge, in der das Haus den Betrieb beschreibt. Bisher nirgends gesetzt |
| Lage | **Eskalationsstufe** | dieses Feld; die Stufen gehören in `../../ablauf/krisenablauf.md` |

Der Begriff „Betriebszustand" war zuvor für die Lageachse benutzt und ist im
Haus für die Zeitachse belegt. Er gehört dorthin; dieses Feld heißt
Eskalationsstufe.

**Die Eskalationsstufen selbst sind noch nicht gesetzt.** Sie gehören in
`../../ablauf/krisenablauf.md`, der noch nicht geschrieben ist. Bis dahin trägt
das Modul die Stufen, die es tatsächlich unterscheidet, und die Abstimmung steht
als offener Punkt. Nicht hier eine eigene Stufenlogik erfinden — sie würde mit
dem Krisenablauf kollidieren.

Abzugrenzen von drei bestehenden Feldern: **Abbruchkriterien** sagen, wann der
Einsatz endet. **Meldeweg und Eskalation** sagt, wer informiert wird — das ist
der *Pfad*, nicht die *Stufe*. Dieses Feld sagt, wer das Modul führt, wenn die
Lage umschaltet.

### Zu Handlungsvollmacht ohne Rückfrage

**Was das Feld regelt:** Wer darf eine Maßnahme sofort auslösen, ohne vorher zu
fragen — und wo ist Rücksprache zwingend, auch wenn es drängt.

Der Impuls kommt dabei aus einem Ereignis, nicht aus einer Rolle. Niemand
entscheidet planvoll, jetzt eine Zusatzkontrolle anzusetzen; etwas passiert, und
daraus folgt eine Maßnahme in Minuten. Deshalb genügen die vorhandenen Felder
nicht: Die Entscheidungsfrist eines Grundmoduls ist relativ zu T0 bemessen und
damit ein Planungskonstrukt.

Zwei Fälle aus dem Haus zeigen die Grenze:

- Ein Aggregat auf dem Ladehof verliert Öl. Abbinden und Abstreuen und die
  Alarmierung von Feuerwehr und Polizei laufen **ohne Rückfrage** — die
  unmittelbare Gefahr für Personen trägt die Maßnahme.
- Eine angemeldete Demonstration eskaliert. Hier wird **nicht** eigenständig
  eingegriffen; Maßnahmen laufen in Rücksprache mit der Polizei, weil die
  Zuständigkeit dort liegt.

Je Zeile sind auslösende Rolle, Voraussetzung, beendende Stelle und der
unverzüglich zu Informierende vier verschiedene Angaben. Wer auslöst, beendet
nicht notwendig.

### Zu Rechtlich verantwortliche Stelle

Bei Eigenveranstaltungen sind Veranstalter und Betreiber dieselbe Organisation;
das Feld ist dann ausgeblendet. Es greift, wenn ein Modul auch bei
Gastveranstaltungen eingesetzt wird: § 43 Abs. 2 VStättVO legt das
Sicherheitskonzept dem **Betreiber** auf, nicht dem Veranstalter. Nach § 38
Abs. 5 ist eine Übertragung auf den Veranstalter nur schriftlich möglich, und die
Verantwortung des Betreibers bleibt davon unberührt.

Ohne das Feld behauptet der Steckbrief bei einer Gastveranstaltung eine
Verantwortungsverlagerung, die es rechtlich nicht gibt.

## Ausfüllhinweise zu Feldern aus Ebene 1

Keine neuen Felder. Was hier steht, ist die Security-Antwort auf ein Feld, das
`modul.md` nur benennt.

| Feld | Bei Security gilt |
|---|---|
| Modulname | Wo eine behördlich etablierte Benennung existiert, wird sie übernommen — Ordnungsdienstkonzept, Sanitätsdienstkonzept, Räumungskonzept, Verkehrskonzept nach vfdb 13-01 Kap. 3.2. Eine eigene Nomenklatur erzeugt Reibung im Genehmigungsverfahren. **Die eingeführte Hausbezeichnung geht dabei nicht verloren:** Pünktchenplan, Hallenstreife, Spotter, SCU, ODL und SDP stehen als Synonym in der Außensicht und mit Definition im Glossar. Ein Modulname, den im Haus niemand benutzt, wird im Workshop nicht wiedererkannt. |
| Rechtsgrundlage | Norm **und Fassungsstand und Normqualität**. Die Normqualität unterscheidet Rechtsverordnung, Verwaltungsvorschrift, Branchenstandard und Behördenauflage; der Wertebereich steht in `rechtsrahmen.md`. Die Fundstelle verweist dorthin, statt die Norm zu wiederholen. |
| Auslöseschwelle | Mehrere Auslöser einzeln nennen, je mit Art: **Zahl**, **Bewertung** oder **Bescheid**. § 43 VStättVO trägt beide ersten Arten nebeneinander — eine Zahl in Abs. 2 und einen unbestimmten Rechtsbegriff in Abs. 1. Es gilt der zuerst greifende. Für Ausstellungsräume rechnet § 1 Abs. 2 mit einem Besucher je Quadratmeter Grundfläche; die Pflicht greift damit bei einer Messe im Regelfall, nicht als Ausnahme. |
| Fristen | Bei Security fast immer eine **Kette**, kein Datum: mit Zwischenständen und einer Rückmeldezeit, die nicht in der Hand des Hauses liegt. vfdb 13-01 empfiehlt sechs Wochen für den Entwurf und vier für die Endfassung; verbreitete Muster-Sicherheitskonzepte verlangen acht Wochen, vierzehn Tage Behördenrückmeldung, zwei Wochen für die Endfassung und fünf Werktage für die Unterschriften. Eigene Planungstermine gehören nicht hierher, sondern in die Deadlines. |
| Zustimmung | Bei einer Stelle außerhalb des Hauses zusätzlich: Form des Nachweises, Frist relativ T0 und was gilt, wenn die Zustimmung ausbleibt. Das Einvernehmen nach § 43 Abs. 2 ist ein eigener Verfahrensschritt, kein Konzeptinhalt — es kann scheitern, und die Fertigstellung des Moduls liegt insoweit nicht in der Hand des Hauses. |
| Qualifikationsnachweis vor Einsatz | Nicht nur ob und welcher: **Stufe**, **zulässige Belegarten**, **Gültigkeitsdauer**, **Prüfweg**. Die Stufe hängt an der Tätigkeit, nicht an der Person — § 34a Abs. 1a GewO zählt die sachkundepflichtigen Tätigkeiten abschließend auf, für einfache Zugangskontrolle genügt die Unterrichtung. § 8 BewachV kennt mehrere gleichwertige Belegarten. Die Zuverlässigkeit wird spätestens nach fünf Jahren wiederholt geprüft, der Nachweis hat also ein Ablaufdatum. Der Auftraggeber kann das Bewacherregister nicht selbst abfragen; der Prüfweg ist Zusicherung des Erbringers plus Sichtprüfung des Ausweises. |
| Nachweise und Dokumentation | Die Aufbewahrungsdauer ist zu **setzen und zu begründen**, nicht zu übernehmen: für Kontrollprotokolle und Vorfallmeldungen existiert keine normierte Frist. § 21 BewachV bindet mit drei Jahren den Bewachungsunternehmer, nicht den Auftraggeber; Ansprüche wegen Personenschäden verjähren nach § 199 Abs. 2 BGB erst nach dreißig Jahren. Dazu gehört die Angabe, **wo der Beleg liegt** — bei Fremdvergabe liegt er beim Dienstleister und ist ohne vertraglichen Zugriff nicht verfügbar. |
| Lieferobjekte | Wo ein Lieferobjekt Rechtswirkung hat, reicht der Ablageort nicht. Zusätzlich: Adressat, Form, Übergabezeitpunkt und wer gegenzeichnet. Betroffen sind unter anderem das Bestellungsschreiben eines Funktionsträgers, die Dienstanweisung nach § 17 BewachV, die Einvernehmenserklärung und das Sicherheitskonzept selbst, sobald es Bestandteil des Genehmigungsbescheids wird. Wo ein Dokument verteilt wird, gehören Verteiler und Sicherung der aktuellen Fassung dazu. |
| Bemessungsregel | Das **Verfahren** ist selbst anzugeben, nicht nur das Ergebnis: mit Quelle, Verbindlichkeitsstufe, Eingangsgrößen und der Angabe, ob das Ergebnis ein Mindest- oder ein Richtwert ist und wer es abnimmt. Einzelheiten in `bemessungsverfahren.md`. |
| Startbedingung | Vorbedingungen, die den Einsatz sperren, bis sie erfüllt sind: Zulassung des Erbringers, bei Verarbeitung personenbezogener Daten die Rechtsgrundlage der Verarbeitung, die Beschilderung und — wo einschlägig — die Datenschutz-Folgenabschätzung, die Art. 35 DSGVO ausdrücklich „vorab" verlangt, sowie bei Fremdvergabe der Auftragsverarbeitungsvertrag. |
| Risikostufe | Nicht pauschal je Veranstaltung. Eingetragen wird die **höchste** Stufe im Zeitverlauf, und die Zeitabschnitte, in denen sie erreicht wird, werden benannt. |
| Ressourcenbedarf | Je Phase ist zu grob. Bei Security zusätzlich als Grundlage des Postenplans: Posten und Zeitfenster. Die Realprobe zeigt den Unterschied — derselbe Sanitätsdienst steht im Aufbau mit zwei Kräften und in der Laufzeit mit sieben Kräften einschließlich Arzt und Rettungswagen. |
| Nachbereitung und Rückkopplung | Bemessungsergebnis und tatsächlicher Bedarf werden getrennt geführt und gegeneinander ausgewertet. Der einzige veröffentlichte Vergleich der beiden gängigen Sanitätsdienst-Verfahren zeigt beide als deutlich überdimensionierend; ohne Rückkopplung bleibt das unbemerkt. |

## Schnittregeln für Security

`modul.md` sagt, was ein Modul ist. Wie man in der Praxis entscheidet, wo eines
aufhört, ist dort als offener Punkt vermerkt; der Werkstatt-Test ist bisher der
einzige Maßstab. Drei Regeln für Security, die ihn ergänzen.

**Compliance und Leistung werden nicht in einem Modul vermischt.** Auch dann
nicht, wenn derselbe Kräftepool beides erbringt — der Ordnungsdienst ist Pflicht,
die Standwache ist eine an Aussteller verkaufte Leistung. Der Werkstatt-Test
trennt sie, weil Adressat, Nachweis und Abrechnung verschieden sind. Die
Konkurrenz um dieselben Kräfte wird als Abhängigkeit geführt, nicht durch
Zusammenlegen aufgelöst.

**Das Veranstalter-Modell ist weder Variante noch Parameter.** Es ändert nicht,
wie gearbeitet wird, sondern wer rechtlich haftet. Nach dem Werkstatt-Test bleibt
es damit ein Modul — mit dem bedingten Feld „Rechtlich verantwortliche Stelle",
nicht mit einer zweiten Anleitung.

**Ein Szenario ist kein Modul.** Bombendrohung, Räumung, Überfüllung, Unwetter
sind Krisenfälle. Sie gehören in `../../ablauf/krisenablauf.md`. Was im Modul
steht, ist das Verhalten je Eskalationsstufe — nicht der Ablauf des
Ereignisses.

**Ein Ablaufschritt wird nicht dadurch zum Modul, dass er einen Namen hat.**
Dieselbe Tätigkeit kommt in mehreren Modulen als Abschnitt vor — eine
Personenkontrolle findet am Einlass statt und noch einmal durch die
Hallenstreife in der Veranstaltung. Das sind nicht zwei Module gleichen Namens
und auch kein drittes, das beide bedient. Unterschieden wird über den
**Geltungsbereich**: Das Modul am Einlass gilt räumlich vor der Ticketkontrolle,
die Hallenstreife in der Veranstaltung.

Dazu eine Abgrenzung, die häufig verwechselt wird: **Ein Teilkonzept ist ein
Lieferobjekt, kein Modul.** Das Ordnungsdienstkonzept ist das, was das Modul
Ordnungsdienst hervorbringt. Der Name ist derselbe, die Sache nicht.

## Übergaben an Stellen ohne Weisungsverhältnis

Ebene 1 kennt drei Arten von Beteiligten: eigene Rollen, Dienstleister, die die
Linie beschafft, und Nachbarn, an die übergeben wird. Bei Security kommt eine
vierte hinzu, für die keine dieser drei passt: Polizei, Feuerwehr, Ordnungsamt,
Zoll, Rettungsdienst und die Brandsicherheitswache. Sie sind nicht
weisungsgebunden, sie sind nicht beschaffbar, und sie können in den laufenden
Betrieb hineinweisen — bei der Brandsicherheitswache nach § 41 Abs. 2 VStättVO
ausdrücklich mit der Folge, dass ihren Anweisungen Folge zu leisten ist.

Wo ein Modul an eine solche Stelle grenzt, wird die Übergabe wie jede andere
beschrieben — Objekt, Medium, Auslöser, Rollen — und zusätzlich in
`rechtsrahmen.md` mit ihrer Befugnis gegenüber dem Haus, ihrer Erreichbarkeit und
dem nötigen Vorlauf geführt. Der Vorlauf ist der Punkt, der in der Praxis
gerissen wird: das Behördenmeeting liegt weit vor der Veranstaltung.

## Prüfliste

Beim Schreiben eines Security-Moduls zusätzlich zur Definition of Done aus
`modul.md`:

- Steht bei jeder Anforderung, ob sie Rechtspflicht, Behördenauflage,
  Branchenstandard oder Hausentscheidung ist? Ohne das wird Freiwilliges als
  Pflicht geführt — und Pflichtiges beim Tailoring gestrichen.
- Sind alle Auslöser genannt, nicht nur der bekannteste?
- Ist die Frist eine Kette oder ein Datum? Externe Fristen haben Zwischenstände
  und eine Rückmeldezeit, die nicht in der Hand des Hauses liegt.
- Ist gesagt, was gilt, wenn eine externe Zustimmung ausbleibt?
- Steht die Befugnisgrundlage **und** ihre Grenze?
- Ist das Modul lückenlos besetzt, und ist die Übergabe beschrieben? Für den
  Schichtwechsel existiert keine Norm, auf die verwiesen werden könnte — das
  Modul muss sie selbst definieren.
- Hat jeder personengebundene Nachweis ein Ablaufdatum und einen Prüfweg?
- Ist die Aufbewahrungsdauer gegen den Haftungshorizont begründet, und ist
  gesagt, wo der Beleg liegt?
- Ist die Bemessung als Posten mal Zeit ausgedrückt, nicht als Stückzahl?
- Steht bei jedem Lieferobjekt mit Rechtswirkung, wer es gegenzeichnet?

## Offene Punkte

Mit Stand der Klärung in `../../../0_meta/offene-punkte.md`.

- **Eskalationsstufen sind nicht gesetzt.** Das Feld „Verhalten je
  Eskalationsstufe" braucht sie. Sie gehören in den Krisenablauf, der noch nicht
  geschrieben ist.
- **Betriebszustände sind ebenfalls nicht gesetzt**, jetzt aber als eigene
  Achse. Das Haus unterscheidet Nullbetrieb, technischen Aufbau, vorgezogenen
  Aufbau, regulären Aufbau, Laufzeit, Abendveranstaltung und Abbau; drei davon
  liegen innerhalb von P4. Ob die Phasenbeschreibung das aufnimmt, ist mit der
  Projektleitung zu klären. Der Optionen-Entwurf dazu liegt nicht mehr im
  Workspace; die Frage steht in `../../../0_meta/offene-punkte.md`.
- **Vier Bestandteile ohne bekannten Ort.** Die Realprobe verweist auf
  Gefahrenabwehrplan, Funkregeln, sicherheitstechnische Anlagen und Glossar als
  Anlagen eines Rahmensicherheitskonzepts. Ob es diese Bestandteile im Haus gibt
  und wo sie geführt werden, ist offen. Werden sie je Veranstaltung neu
  geschrieben, ist das Doppelarbeit, die die Module beheben würden.
- **Vorrang zwischen Modulen.** § 38 Abs. 4 VStättVO verpflichtet zur
  Einstellung des Betriebes; ein Security-Modul kann damit andere stillstellen.
  Das Feld „Abhängigkeiten" in `modul.md` kennt nur `setzt voraus` und
  `nicht gemeinsam mit`. Nicht hier gelöst, weil die Veranstaltungstechnik
  dasselbe kann — Frage an Ebene 1.

## Belege

Die Wortlaute stammen aus Webabrufen und sind vor der Aufnahme in
`rechtsrahmen.md` am amtlichen Text der maßgeblichen Landesfassung zu prüfen.

- MVStättVO (ARGEBAU, Fassung Juni 2005, zuletzt geändert Juli 2014) —
  https://www.is-argebau.de/Dokumente/4231724917250.pdf
- § 38, § 41, § 42, § 43 VStättVO — https://dejure.org/gesetze/VStaettVO/38.html
  · /41.html · /42.html · /43.html
- § 34a GewO — https://dejure.org/gesetze/GewO/34a.html
- BewachV §§ 8, 12, 16, 17, 18, 21 — https://lxgesetze.de/bewachv/8
- DIHK-Merkblatt Bewachungsgewerbe, Unterrichtung oder Sachkundeprüfung —
  https://www.dihk.de/resource/blob/2480/fd3b81202233a1493b7a94ad74caba87/recht-merkblatt-bewachungsgewerbe-unterrichtung-oder-sachkundepruefung--data.pdf
- vfdb-Merkblatt 13-01, Sicherheitskonzept für Großveranstaltungen, Oktober 2014
  — https://www.vfdb.de/media/doc/merkblaetter/MB_13_01_sicherheitskonzept.pdf
- BaSiGo, Betriebsarten —
  https://basigo.vfsg.org/index.php?title=Grundlagen/Betriebsarten
- § 199 BGB — https://dejure.org/gesetze/BGB/199.html
- Art. 35 DSGVO —
  https://www.datenschutz-grundverordnung.eu/grundverordnung/art-35-ds-gvo/
- DSK, Orientierungshilfe Videoüberwachung durch nicht-öffentliche Stellen —
  https://www.datenschutzkonferenz-online.de/media/oh/20200903_oh_v%C3%BC_dsk.pdf
