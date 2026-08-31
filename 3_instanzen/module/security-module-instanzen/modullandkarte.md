---
status: entwurf
stand: 2026-08-31
quelle: Landkarten-Sparring und Modulbefüllung am 24.08.2026; Einordnungen bestätigt durch die Projektleitung am 29.08.2026
---

# Modullandkarte Security

Das Register der Security-Module: welche es gibt, wie sie eingeordnet sind, und
was ausdrücklich **kein** Modul ist.

**Was hier steht, ist Katalog, nicht Konzept.** Welche Felder ein Modul hat und
was die Einordnungen bedeuten, steht in `../../../1_grundkonzepte/modul.md` und
im Detailkonzept. Hier steht nur, welche Bausteine existieren.

**Stand der Validierung.** Die Einordnungen stammen aus dem Sparring vom
24.08.2026 und sind mit der Projektleitung durchgegangen. Sie sind **nicht** mit
dem Fachbereich validiert — das ist Aufgabe des ersten Workshops. Zwei
Prüfungen stehen noch aus: der Abgleich gegen das anonymisierte
veranstaltungsbezogene Sicherheitskonzept in `../../../0_meta/quellen/`, und der
Vollständigkeitstest über die Phasenachse.

## Die zwei Achsen

**Modulart** sagt, *was* es ist: `Compliance` oder `Leistung`.
**Pflichtstufe** sagt, *ob* es für eine Veranstaltung gilt: `Pflicht`,
`Wahlpflicht` oder `Optional`.

Sie sind unabhängig. Ein Leistungsmodul kann Pflicht sein, weil die Messe es
gesetzt hat; ein Compliance-Modul kann in Ausprägungen zur Wahl stehen.

**Konsistenzregel für dieses Register.** Eine Gruppe sich ausschließender
Ausprägungen besteht aus mindestens zwei Modulen — Grundmodul plus mindestens
eine Alternative, jede mit eigener Modul-ID und eigenem Eintrag hier. Bei
`Wahlpflicht` gilt zusätzlich: Steht dort nur ein Modul, ist entweder die
Pflichtstufe falsch oder es fehlen Einträge, denn eine Ausprägung muss laufen.
Eine Gruppe kann auch innerhalb von `Optional` stehen; dann gilt bei
Nichtentscheidung keine der Ausprägungen. Der Gegenfall in beiden Fällen: Ein
einzelnes Modul, dessen Ausprägungen mit derselben Anleitung laufen, ist keine
Gruppe, sondern ein Modul mit einer Varianten-Tabelle.

## Module

| Modul | Modulart | Pflichtstufe | Anmerkung |
|---|---|---|---|
| Personenkontrolle — Stichprobe mit Spotter | Compliance | Wahlpflicht · **Grundmodul** | `MOD-SEC-01`, befüllt. Einfachste Ausprägung: Spotter beobachtet die ankommende Menge und veranlasst stichprobenartig Kontrollen. Gilt, solange nichts anderes entschieden ist. Dem Identitätsmanagement räumlich vorgeschaltet |
| Personenkontrolle — Torbogen und Handgerät | Compliance | Wahlpflicht · Alternative zu MOD-SEC-01 | Technische Detektion an besetzten Positionen. Anderer Aufbau, anderes Personaltableau, andere Bemessung. Modul-ID noch nicht vergeben |
| Personenkontrolle — Vollkontrolle | Compliance | Wahlpflicht · Alternative zu MOD-SEC-01 | Alle Personen, über Zelt und Zaun geführt. Maximale Ausprägung mit eigener Infrastruktur. Modul-ID noch nicht vergeben |
| Gepäckkontrolle | Leistung | Optional | Eigene Zielrichtung, nicht Teil der Personenkontrolle. Ausprägungen: Nachschau durch die kontrollierende Person, X-Ray. Verlangt ein Bescheid sie, ist das nach der Schwellenregel ein eigenes Modul — noch nicht geschnitten |
| Identitätsmanagement und Ticketkontrolle | Leistung | Pflicht | Immer technisch über das Drehkreuz; es werden nur digitale Tickets verkauft |
| Prüfung personifizierter Tickets | Leistung | Optional | Abgleich Ticket gegen Ausweis. Aus Frankreich mitgebracht, im Haus in Vorbereitung |
| SDP — Service-Ticketing-Portal | Leistung | Pflicht | Legitimierung von Personen, die weder Besucher noch Aussteller sind. Außerhalb der Laufzeit |
| Hallenstreife Laufzeit | Compliance | Pflicht | Veranstaltungssicherheit während der Öffnungszeit; überwacht auch das Rauchverbot. Die Zahl der Streifen skaliert, das ist ein Parameter |
| Hallenstreife Auf- und Abbau | Compliance | Pflicht | Eigenes Modul, nicht dieselbe Streife: andere Zielrichtung (Rettungswegfreiheit, Diebstahlprävention), andere Einweisung. Der Vertretungstest schlägt an |
| Ordnungsdienstleiter | Compliance | Pflicht | Aus der VStättV. Separat bestellt, nur für die Veranstaltung |
| Brandsicherheitswache | Compliance | Pflicht | Das Mengengerüst kommt von der Feuerwehr und lässt keine Abweichung zu |
| Lagebesprechung der Veranstaltung | Leistung | Pflicht | Morgenlage vor Veranstaltungsbeginn im Kriseninterventionsraum, mit standardisiertem Besprechungsprotokoll. Bei Gastveranstaltungen führt der Gastveranstalter sie |
| Interventionsdienst | Leistung | Pflicht | Anlassbezogenes Eingreifen bei Verstößen in der Veranstaltung — von unzulässigen Ausstellungsstücken bis zu Datenschutzverstößen auf Ständen |
| VIP- und Personenschutz | Leistung | Optional | Auslöser sind Schutzpersonen oder gefährdete Aussteller. Teils mit eigenem Werkschutz des Kunden, dann Abstimmung nötig |
| Querüberwachung Parallelveranstaltung | Leistung | Optional | Trennung der Besuchergruppen bei gleichzeitigen Veranstaltungen. Fällt überwiegend in die Betreiberrolle |
| Drohnenflug | Leistung | Optional | Prüfung der Nachweise: Pilotenqualifikation, Drohnengröße, Genehmigung des Luftfahrt-Bundesamts |

## Kein Modul

Ausdrücklich geprüft und verworfen. Sie stehen hier, damit sie im Workshop nicht
erneut als Kandidat auftauchen.

| Kandidat | warum kein Modul | wo es stattdessen steht |
|---|---|---|
| Lagebild | Dauerhafte Bewertungsarbeit ohne Anfang und Ende, 365 Tage im Jahr, nicht veranstaltungsbezogen. Es liegt kein Ergebnis vor, das je fertig wäre | Voraussetzung im Feld „Abhängigkeiten" der Module, die es brauchen |
| Erstellung Pünktchenplan | Der Pünktchenplan ist das Lieferobjekt, das zur Bestellung führt, und zugleich das Bemessungsverfahren — nicht die Leistungseinheit selbst | Feld „Lieferobjekte" und `../../../2_detailkonzepte/module/security-module-detailkonzept/bemessungsverfahren.md` |
| Durchführungskontrolle | Die Abnahme des bestellten Personals ist Teil des Moduls, das bestellt hat. Sie herauszulösen würde die Verantwortung von der Leistung trennen | Ablaufabschnitt im jeweiligen Modul |
| Demonstrationen | Ein Szenario, kein Baustein | `../../../2_detailkonzepte/ablauf/krisenablauf.md`, sobald er geschrieben ist |
| Datenschutzkonformität auf Ständen | Aufklärung läuft über Hausordnung und AGB, die Kontrolle ist anlassbezogen | geht im Interventionsdienst auf |
| SCU — Service Control Unit | Organisationseinheit mit 365-Tage-Auftrag, aus dem Security-Budget bestellt, nicht je Veranstaltung | Schnittstelle in den Modulen, die sie berührt — Fundsachen, Videoauswertung, Brandmeldeanlage, Evakuierungstechnik |
| Shuttlebusse | Kein Security-Anteil; der Zweck ist Besucherkomfort | Logistik |

## Nicht in diesem Bereich

| Thema | Zuständigkeit |
|---|---|
| Arbeitsschutz und Verantwortlicher für Veranstaltungstechnik | Abteilung 420. **Noch nicht abschließend geklärt** — die Hallenstreife im Auf- und Abbau nimmt Arbeitsschutzaufgaben wahr, die Zuständigkeit ist gemischt |
| Verkehrsführung, Parkraum, Anfahrt | Logistik. Der Security-Anteil an Toren und Zufahrten — welche offen sind, wie sie besetzt sind, wer hineindarf — bleibt in Security-Modulen |

## Offene Punkte der Landkarte

- **Modul-IDs und Steckbriefe der beiden Alternativen der Personenkontrolle.**
  Dass es eigene Module sind, ist entschieden — der Werkstatt-Test schlägt an:
  Spotter-Stichprobe, Torbogen und Vollkontrolle unterscheiden sich in Ablauf,
  Aufbau und Personaltableau so weit, dass eine Vertretung drei verschiedene
  Anleitungen bräuchte. Offen sind Nummern und Inhalt.
- **Gepäckkontrolle — Varianten oder zwei Module?** Nachschau durch die
  kontrollierende Person und X-Ray unterscheiden sich in Aufbau und Personal
  ähnlich stark wie die Ausprägungen der Personenkontrolle. Sind es zwei Module,
  bilden sie eine Gruppe innerhalb von `Optional`: Nachschau als Grundmodul,
  X-Ray als Alternative. Beide bleiben Optional — wird nichts gebucht, gilt
  keine der beiden. Die Form dafür gibt es (E-85); zu entscheiden ist nur der
  fachliche Schnitt.
- **Überlappung Vollkontrolle und Gepäckkontrolle.** Die maximale Ausprägung der
  Personenkontrolle wurde im Sparring einschließlich Gepäckprüfung beschrieben.
  Nach Bedingung 1 — ein Ergebnis, nicht zwei — bleiben es zwei Module, und die
  Vollkontrolle setzt die Gepäckkontrolle voraus. Zu bestätigen.
- **Besucherhöchstzahlen.** Im Gespräch bei der Personenkontrolle verortet, weil
  dort gezählt wird. Kandidat für ein eigenes Modul zur Kapazitätsüberwachung —
  § 1 Abs. 2 VStättVO bemisst die Kapazität normativ.
- **Gepäckkontrolle bei behördlicher Auflage.** Nach der Schwellenregel ein
  eigenes Modul. Ob es gebraucht wird, entscheidet der Workshop.
- **Vollständigkeit.** Weder gegen das Sicherheitskonzept noch über die
  Phasenachse geprüft.
