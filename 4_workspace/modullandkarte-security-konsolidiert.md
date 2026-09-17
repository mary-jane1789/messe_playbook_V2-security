---
status: entwurf
stand: 2026-09-17
quelle: Modullandkarte Security V0.2 vom 02.09.2026 (34 Module unverändert übernommen); Ergänzungen aus Veranstaltungssicherheit — Leitfaden der Branddirektion München / BaSiGo, 3. Auflage Juni 2015, Kap. 3.3.2.2., 6.2.6., 7.1.; Phasen nach 1_grundkonzepte/phasen.md
---

# Modullandkarte Security — konsolidiert

45 Module in neun Modulgruppen. Baut auf der Modullandkarte V0.2 auf: deren
Module, Modularten und Pflichtstufen sind unverändert übernommen. Ergänzt sind
elf neue Module und eine neue Gruppe — die Stellen, an denen der Durchgang
durch den Münchner Leitfaden Leistungen ohne Träger gefunden hat. Ein Modul ist
verschoben.

Nicht validiert, weder mit dem Fachbereich noch mit dem Verfasser der V0.2.

Die laienverständlichen Beschreibungen je Gruppe und Modul, die Rollenliste und
die fünf Entscheidungsfragen stehen in
[modullandkarte-security-konsolidiert.html](modullandkarte-security-konsolidiert.html) —
dort aufklappbar am jeweiligen Eintrag. Rechtsbezüge sind dort Hinweise zur
Orientierung; verbindlich ist die Fundstellentabelle in
`../2_detailkonzepte/module/security-module-detailkonzept/rechtsrahmen.md`, die
noch leer ist.

## Aufbau

**Drei Ebenen: Modulgruppe → Modul → Variante.** Die Modulgruppe ordnet und
steuert nichts. Das Modul ist die Leistungseinheit: einzeln bestellbar,
bemessbar und prüfbar, mit einem Ergebnis. Die Variante ist eine Ausprägung
desselben Moduls — anderer Mitteleinsatz, gleiches Ergebnis.

**Tags am Modul, keine Ordnungsebenen.** Die drei Angaben aus V0.2 hängen am
einzelnen Modul und schneiden den Katalog nicht: Compliance ist ein Merkmal,
keine Achse. Zwei Module derselben Gruppe dürfen sich in allen dreien
unterscheiden.

| Tag | Werte | sagt |
|---|---|---|
| Modulart | Compliance · Leistung · offen | was das Modul ist — und damit, welche Felder Pflicht sind |
| Pflichtstufe | Muss · Wählen · Kann | ob ein Modul für eine Veranstaltung gilt |
| Grundmodul / Alternative zu | — · Modul-ID | ob es mit anderen Modulen eine Wahl bildet |

**Mapping-Achsen, die quer liegen** und deshalb nicht in der Hierarchie stehen:
Phase (P0 bis P7 nach [phasen.md](../1_grundkonzepte/phasen.md)) und Akteur
(Veranstalter · Dienstleister · Genehmigungsbehörde · Gefahrenabwehr). Beide
Mappings stehen noch aus. Als dritte Querachse zeichnet sich der Betriebszustand
ab; er ist noch nicht gesetzt.

**Nummerierung** `SEC-<Gruppe>-<Modul>`, beide Teile zweistellig. Die Nummer ist
an die Gruppe gebunden — ein Gruppenwechsel ändert damit die ID. Das steht gegen
die Regel, dass IDs nie neu vergeben werden, und gegen das Muster
`MOD-<BEREICH>-<NR>` aus `1_grundkonzepte/modul.md`. Siehe offene Punkte.

**Herkunft** je Modul: `V0.2` unverändert übernommen · `neu` in dieser Fassung
ergänzt · `verschoben` aus einer anderen Gruppe der V0.2.

## 1 · Sicherheitsplanung und Behördenverfahren

Adressat ist die Behörde, nicht der Betrieb: fremdbestimmte Fristenketten und
eine eigene Nachweislogik. Die Module bewerten das Risiko, erzeugen die
abgestimmte sicherheitstechnische Dokumentation, planen den Umgang mit
Störungen und prüfen Sondertatbestände mit eigenem Rechtsrahmen.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-01-01 | Risikobeurteilung je Veranstaltung | Compliance (Vorschlag) | Muss | — | V0.2 |
| SEC-01-02 | Sicherheitskonzept und Einvernehmen | Compliance (Vorschlag) | Wählen | Ergänzung zum Rahmensicherheitskonzept (Default) · vollumfängliches Sicherheitskonzept · erweiterte Veranstaltungsbeschreibung | V0.2 |
| SEC-01-03 | Notfall- und Szenarienplanung | Compliance (Vorschlag) | Muss | eigenständige Notfallplanung · Ergänzung zum Rahmenkonzept | neu |
| SEC-01-04 | Freigabe sicherheitskritischer Exponate | offen | Kann | Waffen (WaffG) · Gefahrgut und Gefahrstoffe · Maschinen im Betrieb | V0.2 |
| SEC-01-05 | Drohnenflug | offen | Kann | — | V0.2 |
| SEC-01-06 | Sicherheitstechnische Nachbereitung | offen | Muss | interner Erfahrungsbericht · gemeinsame Nachbesprechung mit den Behörden | neu |

## 2 · Perimeter- und Geländeschutz

Schützt die äußere Hülle des Geländes: Wirkung auf Flächen und Sachen statt auf
einzelne Personen, über alle Betriebszustände von Nullbetrieb bis Abbau.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-02-01 | Hallenstreife Laufzeit | Compliance | Muss | Halle · Freigelände | V0.2 |
| SEC-02-02 | Hallenstreife Auf- und Abbau | Compliance | Muss | — | V0.2 |
| SEC-02-03 | Geländeabsicherung und Absperrungen | offen | Muss | Bauzaun und feste Absperrung · mobile Absperrung | V0.2 |
| SEC-02-04 | Zufahrtsschutz (Überfahrtschutz) | offen | Kann | Poller und feste Sperren · mobile Fahrzeugsperren | V0.2 |

Die Videoüberwachung des Geländes stand in V0.2 hier, mit dem Vermerk, dass
eine Setzung nötig ist. Sie steht jetzt in Gruppe 9.

## 3 · Zugangs- und Personenkontrolle

An definierten Übergängen wird in Rechte von Personen und Fahrzeugen
eingegriffen; Befugnisgrundlage ist Hausrecht und Einwilligung. Geschnitten nach
Zielgruppe und Übergang.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-03-01 | Personenkontrolle — Stichprobe mit Spotter | Compliance | Wählen (Grundmodul) | — | V0.2 |
| SEC-03-02 | Personenkontrolle — Torbogen und Handgerät | Compliance | Wählen | — | V0.2 |
| SEC-03-03 | Personenkontrolle — Vollkontrolle | Compliance | Wählen | — | V0.2 |
| SEC-03-04 | Gepäckkontrolle | offen | Kann | Nachschau durch die kontrollierende Person · X-Ray | V0.2 |
| SEC-03-05 | Identitätsmanagement und Ticketkontrolle | Leistung | Muss | — | V0.2 |
| SEC-03-06 | Prüfung personifizierter Tickets | Leistung | Kann | — | V0.2 |
| SEC-03-07 | SDP — Service-Ticketing-Portal | Leistung | Muss | — | V0.2 |
| SEC-03-08 | Zu- und Ausfahrtkontrolle Lieferverkehr | offen | Muss | — | V0.2 |
| SEC-03-09 | Ausschleuskontrolle Abbau | offen | Kann | — | V0.2 |

## 4 · Ordnungs- und Wachdienste

Personalgestellende Dienste mit eigener Bemessung (Postenplan, Qualifikation
nach § 34a GewO). Compliance-Dienst und verkaufte Leistung stehen bewusst
nebeneinander.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-04-01 | Ordnungsdienst | Compliance (Vorschlag) | Muss | — | V0.2 |
| SEC-04-02 | Interventionsdienst | Leistung | Muss | — | V0.2 |
| SEC-04-03 | Standbewachung | Leistung (Vorschlag) | Kann | — | V0.2 |
| SEC-04-04 | Bühnen- und Forenabsicherung | offen | Kann | — | V0.2 |
| SEC-04-05 | VIP- und Personenschutz | Leistung | Kann | — | V0.2 |
| SEC-04-06 | Bestellung und Nachweis des Ordnungsdienstleiters | Compliance (Vorschlag) | Muss | — | neu |

## 5 · Personenstrom und Crowd Management

Konzept- und datengetrieben statt personalgestellend: Kapazitäten nachweisen,
Ströme je Phase und Betriebsart steuern, Dichten überwachen.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-05-01 | Kapazitäts- und Rettungswegnachweis | Compliance (Vorschlag) | Muss | — | V0.2 |
| SEC-05-02 | Personenlenkung und -steuerung | offen | Muss | Einlass · Betrieb · Auslass / Regelbetrieb · Störungsfall | V0.2 |
| SEC-05-03 | Crowd Monitoring (Dichteüberwachung) | offen | Kann | — | V0.2 |
| SEC-05-04 | Querüberwachung Parallelveranstaltung | Leistung | Kann | — | V0.2 |

## 6 · Brandschutz und Rettungswege

Eigener Rechtsrahmen mit eigener Prüfinstanz: Brandschutzdienststelle und
Feuerwehr prüfen und erteilen Einvernehmen, mit eigenen Fristen. Die Module
halten Rettungswege frei, prüfen Brandlasten und Zündquellen auf der Fläche,
halten Löschmittel vor, stellen die Brandsicherheitswache und sichern das
Eröffnungs-Gate.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-06-01 | Freihaltung Flucht- und Rettungswege | offen | Muss | Auf- und Abbau · Laufzeit | V0.2 |
| SEC-06-02 | Brandschutzprüfung Standbau und Dekoration | Compliance (Vorschlag) | Muss | Prüfung nach Standbauantrag · Prüfung vor Ort in P4 | neu |
| SEC-06-03 | Offenes Feuer, Pyrotechnik und Flüssiggas | Compliance (Vorschlag) | Kann | offenes Feuer und Kochvorführung · Flüssiggas auf Ständen · Bühnenpyrotechnik | neu |
| SEC-06-04 | Löschmittel- und Löschwasservorhaltung | Compliance (Vorschlag) | Muss | — | neu |
| SEC-06-05 | Brandsicherheitswache | Compliance | Kann | — | V0.2 |
| SEC-06-06 | Brandschutz-Check vor Eröffnung | Compliance (Vorschlag) | Muss | — | V0.2 |

## 7 · Sanitätsdienst

Behördlich eigenständiges Teilkonzept mit medizinischer Fachlichkeit, eigenem
Bemessungsverfahren und eigener Leitungsrolle.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-07-01 | Sanitätswachdienst | Compliance (Vorschlag) | Muss | — | V0.2 |

## 8 · Sicherheitskommunikation und Lage

Der Querschnitt, der die anderen Gruppen im Störungsfall verbindet: fällt er
aus, wird keine andere Leistung wirksam.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-08-01 | Lagebesprechung der Veranstaltung | Leistung | Muss | — | V0.2 |
| SEC-08-02 | Sicherheitskommunikation | offen | Muss | — | V0.2 |
| SEC-08-03 | Koordinierungsstelle je Veranstaltung | offen | Muss | — | V0.2 |
| SEC-08-04 | Ereignisdokumentation | Compliance (Vorschlag) | Muss | — | neu |

## 9 · Sicherheitstechnische Anlagen

Neue Gruppe. Sie löst den offenen Punkt der V0.2: mit dem Verwerfen der SCU als
Organisationseinheit haben Videoauswertung, Brandmeldeanlage und
Evakuierungstechnik ihren Träger verloren.

**Der Schnitt liegt nicht auf der Anlage, sondern auf ihrer veranstaltungs­-
bezogenen Betriebsbereitschaft.** Die Anlagen selbst sind Betreiberinfrastruktur
mit 365-Tage-Auftrag und deshalb kein Modul — genau die Begründung, mit der V0.2
die SCU verworfen hat. Je Veranstaltung bestellbar und prüfbar ist dagegen:
Anpassung an die Hallenbelegung, Parametrierung, Abnahme vor Eröffnung,
Bedienung während der Laufzeit, Kompensation bei Abschaltung.

| ID | Modul | Modulart | Pflichtstufe | Varianten | Herkunft |
|---|---|---|---|---|---|
| SEC-09-01 | Videoüberwachung und Auswertung | offen | Kann | Bestandsanlage · temporäre Ergänzung | verschoben (V0.2, Gruppe 2) |
| SEC-09-02 | Brandmelde- und Alarmierungstechnik | Compliance (Vorschlag) | Muss | Vollbetrieb · Bereichsabschaltung mit Kompensation | neu |
| SEC-09-03 | Sprachalarmierung und Evakuierungstechnik | Compliance (Vorschlag) | Muss | — | neu |
| SEC-09-04 | Sicherheitsbeleuchtung und Notstromversorgung | Compliance (Vorschlag) | Muss | Bestandsanlage Halle · temporäre Versorgung Freigelände | neu |
| SEC-09-05 | Blitzschutz temporärer Aufbauten | offen | Kann | — | neu |

## Die neuen Module im Einzelnen

| ID | warum es fehlte | Beleg |
|---|---|---|
| SEC-01-03 | V0.2 verweist Szenarien in den Krisenablauf und führt Räumungs- und Überfüllungskonzept als Lieferobjekte „der Notfallplanung" — die Notfallplanung selbst hat keinen Träger. Das Szenario ist kein Baustein, die Leistung es zu erstellen, aktuell zu halten und zu üben schon. | Leitfaden Kap. 3.3.2.2.10.—.12. |
| SEC-01-06 | Nachbereitung ist in V0.2 nicht geführt. Die Security-seitige Auswertung speist das Risikoregister und die nächste Edition; sie dockt an Lessons Learned in P7 an, ist aber eine eigene Leistung mit eigenem Ergebnis. | Leitfaden Kap. 7.1., 7.2.; Playbook Gate P7 → P0 |
| SEC-06-02 | Gruppe 6 deckte Rettungswege, Brandsicherheitswache und Eröffnungs-Gate ab, nicht die Brandlast auf der Fläche: Brandverhalten von Dekoration und Ausstattung, Abstände zwischen Aufbauten. Bei Ausstellerständen der mengenmäßig größte Brandschutzanteil. | Leitfaden Kap. 3.3.2.2.9., .14., Anlage 3 |
| SEC-06-03 | Zündquellen, die der Aussteller oder der Veranstalter selbst einbringt — Kochvorführung, Gasflasche, Bühnenpyrotechnik. Eigener Genehmigungsweg, in V0.2 nicht enthalten. | Leitfaden Kap. 3.3.2.2.14., Anlagen 6b–6f |
| SEC-06-04 | Bereitstellung von Löschgeräten und -mitteln, Löschwasserversorgung, Freihaltung und Nutzbarkeit der Hydranten. Die Nachbereitungsliste des Leitfadens führt fehlende und abgelaufene Feuerlöscher als häufigsten Auflagenmangel. | Leitfaden Kap. 3.3.2.2.14., 7.2. |
| SEC-04-06 | Die Rolle Ordnungsdienstleiter ist nach Grundkonzept kein Modul, und V0.2 hat sie zu Recht gestrichen. Die Bestellung ist aber eine eigene Leistung mit eigenem Nachweis, und sie erfolgt in der Regel extern: bestellt wird eine Person des Dienstleisters, weisungsbefugt gegenüber allen Ordnungsdienstkräften. Ohne dieses Modul hängt die Nachweispflicht an einer Rolle, die im Playbook keinen Steckbrief hat. | § 43 MVStättVO analog; Leitfaden Kap. 3.3.2.2.6. |
| SEC-08-04 | V0.2 verwirft „Lagebild" zu Recht als 365-Tage-Aufgabe. Die veranstaltungsbezogene Protokollpflicht ist davon zu trennen: Entscheidungen, Anweisungen und Maßnahmen im Störungsfall sind nachvollziehbar zu dokumentieren — nach einem Schadensfall die erste Unterlage, nach der Ermittlungsbehörden fragen. | Leitfaden Kap. 6., 6.2.6. |
| SEC-09-01 | Nicht neu, verschoben: In Gruppe 2 stand die Videoüberwachung mit dem Vermerk, dass eine Setzung nötig ist. | V0.2, Gruppe 2 |
| SEC-09-02 | Träger fehlte nach dem Verwerfen der SCU. Die Bereichsabschaltung mit Kompensation ist der praktisch häufige Fall und braucht eine benannte Verantwortung. | V0.2, offener Punkt |
| SEC-09-03 | Gegenstück zu SEC-08-02: dort Wege, Erreichbarkeiten und Wortlaute, hier die Anlage und ihre Betriebsbereitschaft. | Leitfaden Kap. 3.3.2.2.10.; V0.2, offener Punkt |
| SEC-09-04 | Sicherheitsbeleuchtung und Notstrom sind Voraussetzung der Entfluchtung und im Leitfaden Prüfpunkt des Genehmigungsverfahrens; in V0.2 nicht geführt. | Leitfaden Kap. 4.3. |
| SEC-09-05 | Betrifft temporäre Aufbauten im Freigelände — Tower, Bühnen, Videowände. Zuständigkeit gegenüber Abt. 420 ungeklärt, deshalb Modulart offen. | Leitfaden Kap. 3.3.2.2.14. |

## Ausdrücklich kein Modul

Aus V0.2 übernommen und um zwei Fälle aus dem Leitfaden-Durchgang ergänzt.

| Kandidat | warum kein Modul | wo es stattdessen steht |
|---|---|---|
| Ordnungsdienstleiter (die Rolle) | Träger, nicht Leistung — `modul.md` führt Rollen ausdrücklich unter „kein Modul" | Rollenkonzept; die Führungsleistung in SEC-04-01, die Bestellung und ihr Nachweis in SEC-04-06 |
| Lagebild | dauerhafte Bewertungsarbeit, 365 Tage, nicht veranstaltungsbezogen | Voraussetzung im Feld Abhängigkeiten |
| Erstellung Pünktchenplan | Lieferobjekt und Bemessungsverfahren, nicht die Leistungseinheit | Feld Lieferobjekte; Verfahren im Detailkonzept |
| Durchführungskontrolle | Abnahme des bestellten Personals gehört zum bestellenden Modul | Ablaufabschnitt im jeweiligen Modul |
| Demonstrationen | ein Szenario, kein Baustein | Krisenablauf |
| Datenschutzkonformität auf Ständen | anlassbezogene Kontrolle | geht in SEC-04-02 auf |
| SCU — Service Control Unit | Organisationseinheit mit 365-Tage-Auftrag, nicht je Veranstaltung bestellt | Schnittstelle; ihre Leistungen jetzt in Gruppe 9 |
| Shuttlebusse | kein Security-Anteil | Logistik |
| Räumungs- und Überfüllungskonzept | Lieferobjekte, nicht Leistungseinheiten | Lieferobjekte von SEC-01-03 |
| Abstandsflächen zwischen Aufbauten | Prüfkriterium, keine eigene Leistung | Ablaufabschnitt in SEC-06-02 |

## Nicht in diesem Bereich

Der engere Security-Zuschnitt aus V0.2 gilt. Vier Themen, die eine
Sicherheitsbetrachtung im weiteren Sinn wären, liegen außerhalb.

| Thema | Zuständigkeit und Grenze |
|---|---|
| Arbeitsschutz und Verantwortlicher für Veranstaltungstechnik, Standsicherheit fliegender Bauten | Abt. 420. Noch nicht abschließend geklärt — SEC-02-02 nimmt Arbeitsschutzaufgaben wahr, die Zuständigkeit ist gemischt. Betrifft auch SEC-06-02 und SEC-09-05. |
| Verkehrsführung, Parkraum, An- und Abreise, Lieferlogistik | Logistik. Der Security-Anteil an Toren und Zufahrten bleibt in SEC-03-08 und SEC-02-04. |
| Hallen- und Flächenplanung, Aufbaupläne | Expo Realisation und Operations Management. Der sicherheitstechnische Nachweis auf derselben Fläche bleibt in SEC-05-01. |
| Szenarien und Krisenabläufe, Gremien | Krisenablauf beziehungsweise Playbook Teil II. Abgegrenzt davon die durchgeführte Besprechung mit Protokoll — die ist ein Modul (SEC-08-01). |

## Überleitung aus der Leitfaden-Taxonomie

Nachweis, dass beim Zuschnitt auf Security nichts stillschweigend
verschwunden ist. Links die zehn Gruppen der Auswertung des Münchner
Leitfadens, rechts ihr Verbleib.

| Leitfaden-Gruppe | Verbleib |
|---|---|
| 1 Risiko- und Sicherheitsbeurteilung | SEC-01-01; die vier Verfahrensschritte sind Ablaufabschnitte eines Moduls, keine eigenen Module |
| 2 Raumordnung, Kapazität und Wege | Kapazität → SEC-05-01 · Wege → SEC-06-01 · Abschrankung → SEC-02-03 und SEC-04-04 · Abstandsflächen → Prüfkriterium in SEC-06-02 · Aufbauplanung → außerhalb |
| 3 Technische und brandschutztechnische Sicherheit | Brandverhütung → SEC-06-02 und SEC-06-03 · Löschvorhaltung → SEC-06-04 · Brandsicherheitswache → SEC-06-05 · Anlagen → Gruppe 9 · Standsicherheit → außerhalb (Abt. 420) |
| 4 Ordnungsdienstliche Leistungen | Gruppen 2, 3 und 4; Bemessung und Struktur sind Felder von SEC-04-01, Unterstützung der Einsatzkräfte ist Ablaufabschnitt |
| 5 Medizinische Versorgung | SEC-07-01, Bemessung als Parameter |
| 6 Verkehr und Erreichbarkeit | SEC-03-08 und SEC-02-04; der übrige Umfang außerhalb (Logistik) |
| 7 Führung, Gremien und Kommunikation | Gruppe 8; Verantwortlichkeiten → Rollenkonzept · Gremien → Playbook Teil II · Durchsagetexte → Lieferobjekt von SEC-08-02 |
| 8 Ereignis- und Krisenbewältigung | Planungsleistung → SEC-01-03 · Dokumentation → SEC-08-04 · Szenarien und Betriebsarten → Krisenablauf und Betriebszustände-Achse |
| 9 Genehmigung, Nachweis und Kontrolle | SEC-01-02 und SEC-06-06 |
| 10 Nachbereitung und Fortschreibung | SEC-01-06 |

## Mit dem Auftraggeber zu entscheiden

Fünf inhaltliche Einordnungsfragen. Sie entscheiden über Zuschnitt und
Zuständigkeit, nicht über Form.

| # | Frage | betrifft |
|---|---|---|
| 1 | **Gehören die sicherheitstechnischen Anlagen in Security?** Kameras, Brandmelder, Sprachalarmierung und Notlicht sind Betreiberinfrastruktur; der Vorschlag führt ihre veranstaltungsbezogene Betriebsbereitschaft als Modul. Wird das nicht getragen, bleiben diese Leistungen nach dem Verwerfen der SCU ohne Träger — ebenso die Fundsachen, die vierte SCU-Aufgabe, die in keiner Fassung vorkommt. | SEC-09-01 bis SEC-09-05 |
| 2 | **Wer verantwortet Brandschutz am Standbau und Blitzschutz — Security oder Abt. 420?** Die Prüfung von Standbaumaterial, Abständen und Dekoration ist der mengenmäßig größte Brandschutzanteil einer Messe und liegt an der Grenze zur Veranstaltungstechnik. Dieselbe Frage betrifft den Arbeitsschutzanteil der Hallenstreife im Auf- und Abbau. | SEC-06-02, SEC-09-05, SEC-02-02 |
| 3 | **Ist die Brandsicherheitswache Pflicht oder schwellenausgelöst?** Die alte Landkarte führt sie als Pflicht, fachlich greift sie erst bei Verordnung oder Bescheid. Dieselbe Frage bei Exponatfreigabe, Drohnenflug und offenem Feuer — sie hängt daran, ob die Pflichtstufen einen Wert für „ab Schwelle" bekommen. | SEC-06-05, SEC-01-04, SEC-01-05, SEC-06-03 |
| 4 | **Gepäckkontrolle: ein Modul mit zwei Varianten oder zwei Module?** Nachschau und Röntgen unterscheiden sich in Aufbau, Personal und Durchsatz ähnlich stark wie die drei Formen der Personenkontrolle, die als eigene Module geschnitten sind. Zusätzlich: Setzt die Vollkontrolle die Gepäckkontrolle voraus? | SEC-03-04, SEC-03-03 |
| 5 | **Notfallplanung und Nachbereitung: eigene Security-Module oder Teil anderer Bausteine?** Beide sind hier ergänzt, damit die Leistung einen Träger hat. Vertretbar wäre auch, sie im Krisenablauf beziehungsweise in den Lessons Learned von P7 aufgehen zu lassen — dann muss dort benannt sein, wer sie erstellt und fortschreibt. | SEC-01-03, SEC-01-06 |

## Offene Punkte dieser Fassung

- **Nummerierung — Richtung gesetzt, Umsetzung offen.** Die sprechende ID
  `SEC-<Gruppe>-<Modul>` ist gewollt, weil sie Verweise lesbar macht:
  `setzt voraus: SEC-06-02` nennt die Gruppe mit, `MOD-SEC-30` nicht. Solange
  der Gruppenzuschnitt vorläufig ist, sind die IDs hier Arbeitsnummern. Drei
  Regeln gehören dazu, wenn sie scharf gestellt werden: die zweite Ziffer ist
  ein Vergabezähler und keine Position in der Tabelle; frei gewordene Nummern
  werden nie neu vergeben; ein Gruppenwechsel erzeugt eine neue ID, während die
  alte im Register als abgelöst stehen bleibt. Beim Scharfstellen ist das Muster
  `MOD-<BEREICH>-<NR>` in `1_grundkonzepte/modul.md` auf
  `<BEREICH>-<GRUPPE>-<NR>` zu ändern und MOD-SEC-01 zu SEC-03-01 zu überführen
  — als F-Entscheidung mit Begründung.
- **„Gruppe" ist doppelt belegt — erledigt am 16.09.2026.** `modul.md` nannte
  Gruppenrolle das Bündel sich ausschließender Ausprägungen, die Landkarte nennt
  Modulgruppe die Ordnungsebene. Der Begriff Gruppenrolle entfällt: Das Modul
  trägt jetzt `Grundmodul: ja` oder `Alternative zu <Modul-ID>`. „Gruppe"
  bedeutet damit nur noch die Ordnungsebene (E-88).
- **Modulart der neuen Module.** Als Vorschlag gesetzt, wo die Zuordnung
  eindeutig erscheint; offen bei SEC-01-06 und SEC-09-05. Zu setzen im Workshop.
- **Gruppe 9 gegen die Betreiberrolle.** Der Schnitt auf die veranstaltungs­-
  bezogene Betriebsbereitschaft ist ein Vorschlag. Trägt er nicht, fällt die
  Gruppe zurück in die Schnittstelle zur Betreiberorganisation — dann bleibt der
  offene Punkt der V0.2 offen.
- **Zuständigkeit Abt. 420** entscheidet über drei Module: SEC-06-02,
  SEC-09-05 und den Arbeitsschutzanteil von SEC-02-02.
- **Modulzahl je Gruppe.** Gruppe 7 hat ein Modul, Gruppe 3 hat neun. Ob das ein
  Schnittproblem ist oder die Sache so liegt, ist am Fachbereich zu prüfen.
- **Offene Punkte der V0.2 bleiben offen**: Konsolidierung der beiden
  Hallenstreifen, drei Ergebnisse bei SEC-02-02, Vollkontrolle setzt
  Gepäckkontrolle voraus, Modulart von SEC-03-04 und SEC-01-05.
- **Widerspruch zur alten Landkarte in Ebene 3.** `3_instanzen/module/security-module-instanzen/modullandkarte.md`
  führt den Ordnungsdienstleiter als eigenes Modul (Compliance, Pflicht) und die
  Brandsicherheitswache als Pflicht. Beides ist hier anders. Die Einordnungen
  jener Landkarte sind mit E-78 geloggt; die Abweichungen brauchen Revisionszeilen
  im Entscheidungslog, keine stille Änderung.
- **Zählung.** 45 Module: 34 aus V0.2 hier gezählt, 11 neu. V0.2 nennt selbst 33
  — die Differenz liegt vermutlich bei den beiden Hallenstreifen, die dort als
  Konsolidierungskandidat geführt sind.
