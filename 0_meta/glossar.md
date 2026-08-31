---
status: entwurf
stand: 2026-08-31
---

# Glossar

Begriffe, die im Repository verbindlich verwendet werden — je Begriff eine
Definition und, wo nötig, die Abgrenzung zu einem ähnlichen Begriff.

## Begriffe des Repositories

**Gate** — Bedingung an einem Phasenübergang. *Abzugrenzen gegen den
Check-Point:* Ein Gate ist eine Bedingung an einem Phasenübergang, ein
Check-Point eine Übergabe zwischen zwei Rollen, meist innerhalb einer Phase.
Check-Points sind nicht ins Repository übernommen (E-18).

**Modul** — Die kleinste eigenständig verantwortbare Leistungseinheit eines
Bereichs. Langfassung in `../1_grundkonzepte/modul.md`.

**Modulart** — Sagt, *was* ein Modul ist: `Compliance` oder `Leistung`. Sie
steuert, welche Felder Pflicht sind.

**Pflichtstufe** — Sagt, *ob* ein Modul für eine Veranstaltung gilt: `Pflicht`,
`Wahlpflicht`, `Optional`. Sie ist eine Eigenschaft des Moduls im Katalog.
*Abzugrenzen gegen die Verbindlichkeitsstufe:* Die Pflichtstufe sagt, ob das
Modul gilt; die Verbindlichkeitsstufe sagt, wie bindend eine einzelne
Anforderung innerhalb des Moduls ist.

**Verbindlichkeitsstufe** — Was aus einer Fundstelle für das Modul folgt:
`nicht unterschreitbar`, `im Einvernehmen zu bestimmen`, `empfohlen`,
`frei gesetzt`. Wertebereich in
`../2_detailkonzepte/module/security-module-detailkonzept/rechtsrahmen.md`.

**Normqualität** — Was eine Fundstelle rechtlich ist: Rechtsverordnung,
Verwaltungsvorschrift, Gesetz, Behördenauflage, Branchenstandard,
Hausentscheidung. Wertebereich ebenda.

**Phase** — Zeitabschnitt einer Veranstaltung, P0 bis P7, relativ zum ersten
Laufzeittag. In `../1_grundkonzepte/phasen.md`.

**Betriebszustand** — Die feinere Zeitachse, in der das Haus den Betrieb
beschreibt: Nullbetrieb, technischer Aufbau, vorgezogener Aufbau, regulärer
Aufbau, Laufzeit, Abendveranstaltung, Abbau. Überlappt mit den Phasen und ist
noch nicht gesetzt. *Nicht* die Lageachse — dafür siehe Eskalationsstufe.

**Eskalationsstufe** — Wie weit eine Lage eskaliert ist, und wer das Modul dann
führt. Steuert das Modulfeld „Verhalten je Eskalationsstufe". Die Stufen gehören
in den Krisenablauf und sind noch nicht gesetzt. *Abzugrenzen gegen den
Eskalationspfad:* Der Pfad ist der Weg der Information (wer erfährt was über
welchen Weg, Feld „Meldeweg und Eskalation"); die Stufe ist der Zustand der
Lage.

**Geltungsbereich** — Zeitliche und räumliche Grenze eines Moduls. Beide
Angaben sind Pflicht; sie unterscheiden Module mit ähnlicher Tätigkeit.

**Gruppenrolle** — `Grundmodul` oder `Alternative zu <Modul-ID>`. Sie sagt, dass
mehrere Module Ausprägungen derselben Sache sind und immer nur eine gilt. Das
Grundmodul trägt Entscheider, Frist und die Liste der Alternativen; die
Alternativen tragen nur den Rückverweis. **Unabhängig von der Pflichtstufe** —
auch innerhalb von `Optional` möglich. Was bei Nichtentscheidung gilt, hängt
dagegen an der Pflichtstufe: bei `Wahlpflicht` das Grundmodul, bei `Optional`
keine der Ausprägungen.

**Durchführung · Auftragsverantwortung · Fortschreibung** — die drei
Verantwortungen eines Moduls, kurz **R · A · F**. *Durchführung* (R) erbringt die
Leistung und kann der Dienstleister sein. *Auftragsverantwortung* (A) ist eine
Rolle im Haus: verantwortet Anforderung und Mengengerüst, beauftragt, überwacht,
nimmt ab; sie bleibt im Haus, auch wenn die Durchführung vergeben ist.
*Fortschreibung* (F) ist eine namentlich benannte Person und verantwortet das
Modul im Playbook über die Zeit. Ein vollständiges RACI entsteht nicht:
*Consulted* und *Informed* stehen als die Felder **Zustimmung** und
**Meldeweg und Eskalation**.

## Begriffe aus dem Haus

Sie stehen hier, weil sie in Modulen und im Workshop benutzt werden. Wo ein
Modul eine behördlich etablierte Benennung trägt, steht der Hausbegriff als
Synonym in der Außensicht.

**TVK** — Technischer Veranstaltungskoordinator, Rolle 410. Veranstaltungsleiter
im Sinne der Versammlungsstättenverordnung; bestellt den Sicherheitsdienstleister.

**ODL** — Ordnungsdienstleiter. Vom Dienstleister gestellt, je Veranstaltung
separat bestellt, Pflicht aus der Versammlungsstättenverordnung.

**VVT** — Verantwortlicher für Veranstaltungstechnik, aus Abteilung 420. Nicht
Security.

**SCU** — Service Control Unit. Organisationseinheit mit 365-Tage-Auftrag:
Objektschutz, Videoauswertung, Auflauf der Brandmeldeanlagen, Fundsachen. Sitzt
im Operation Center. Kein Modul, sondern Schnittstelle.

**OC** — Operation Center. Das Gebäude, in dem SCU, Rettungswache und
Polizeiwache sitzen. Nicht zu verwechseln mit der SCU, die darin arbeitet.

**Pünktchenplan** — Der Geländeplan mit den sicherheitsrelevanten Positionen,
gefiltert nach der konkreten Veranstaltung. Ergebnis ist die Bestellung beim
Sicherheitsdienstleister. Zugleich das Bemessungsverfahren für den
Ordnungsdienst.

**Spotter** — Sicherheitskraft, die die ankommende Menge beobachtet und
stichprobenartig Kontrollen veranlasst. Minimalausprägung der Personenkontrolle;
es gibt kein Drehkreuz ohne Spotter. Kann von einem Abschnittsleiter mit
wahrgenommen werden.

**SDP** — Service-Ticketing-Portal. Legitimiert Personen, die weder Besucher
noch Aussteller sind, über einen QR-Code außerhalb der Laufzeit.

**Hallenstreife** — Streifengang durch Hallen und Gelände. In der Laufzeit auf
Veranstaltungssicherheit gerichtet, im Auf- und Abbau auf Rettungswegfreiheit
und Diebstahlprävention — deshalb zwei Module.

**Morgenlage** — Tägliche Sicherheitsbesprechung vor Veranstaltungsbeginn im
Kriseninterventionsraum, mit standardisiertem Protokoll.

**Marktfestsetzung** — Kommunalrechtliche Festsetzung, aus der sich neben
Waffenrecht und Versammlungsstättenverordnung Anforderungen an die Veranstaltung
ergeben.
