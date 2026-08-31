---
status: zur Bestätigung
stand: 2026-08-31
zweck: Rückfluss aus den drei Sparrings vom 24.08.2026 in Repository und Projektplan
quelle: Transkripte 20260824 (Blueprint, Landkarte, Befüllung); Export MOD-SEC-Test01
---

# Rückfluss aus den Sparrings vom 24.08.2026

> **Historischer Stand — nicht nachträglich geändert.** Diese Tabelle ist das
> Protokoll der Bestätigung vom 29.08.2026 und bleibt so stehen, damit
> nachlesbar ist, was wann entschieden wurde. Vier Zeilen sind seither
> überholt: **C1a** und **C2** durch E-85 (die Gruppenrolle ist unabhängig von
> der Pflichtstufe, eine Wahlpflicht innerhalb von Optional entsteht nicht),
> **C1b** durch E-68 (der Begriff „Pflichtschwelle" ist entfallen), **B4** durch
> E-84 (drei Verantwortungen statt zwei). Der aktuelle Stand steht in
> `../0_meta/entscheidungen.md`.

Kürzel: **T1** Blueprint-Sparring · **T2** Landkarten-Sparring · **T3** Befüllung ·
**EX** Export MOD-SEC-Test01.

Typ: **Ä** Änderung im Repository · **E** Entscheidung nötig ·
**O** offener Punkt / Frage an die Messe · **P** Projektplan.

Spalte `ok?` zum Abhaken. Bestätigte Zeilen sind mit **✔** markiert und tragen
den Beschluss statt des Vorschlags.

## Beschlossen am 29.08.2026

- **Eskalationsstufe** ersetzt „Betriebszustand" im Modulfeld (B2). Das Wort
  Betriebszustand bleibt damit für die zeitliche Achse frei, wie das Haus es
  benutzt.
- **Pflichtstufe** ersetzt „Bindung" als Feldname (C1, C2). Werte: Pflicht,
  Wahlpflicht, Optional.
- Die Rahmensicherheitskonzept-Annahme darf im Entscheidungslog stehenbleiben,
  aber in keiner Konzeptdatei — und nirgends als Begründung (D1).

---

## A · Feldkatalog Ebene 1 — was die erste echte Befüllung ergeben hat

`1_grundkonzepte/modul.md`. Das ist Ebene 1, gilt also für alle Bereiche, nicht nur Security.

| Nr | Typ | Thema | Aus den Sparrings | Repo-Stand heute | Vorschlag | ok? |
|---|---|---|---|---|---|---|
| A1 | Ä | Übergabetest „fachfremd" | T1: „Das Fachfremde muss hier raus. Ich muss es nicht können, aber eine Vertretung muss verstehen, was da drin gemeint ist." | `modul.md` Z. 345 und Vorlage Z. 463 sagen beide „fachfremde Vertretung" | Wort streichen. Neu: „Eine benannte Vertretung kann den Ablauf ohne Rückfrage ausführen." Auch in der Prüfliste der Vorlage | |
| A2 | E | Feld **Ergebnis** trägt zwei Lesarten | T3: „fertig ist wenn" wurde einmal personenbezogen (Person ist durchs Drehkreuz) und einmal veranstaltungsbezogen (Ende der VA) gelesen. MJ: „würde ich auch anpassen … quasi: wann gilt es, wo ist der Geltungsbereich, zeitlich, vielleicht sogar auch räumlich" | `modul.md`: „ein Satz: Fertig ist, wenn …". Der Dauerleistungsfall stand bereits als offener Punkt (E-61), mit dem Vermerk „zeigt der erste Durchgang" | Der Durchgang ist gelaufen, die Regel trägt nicht. Vorschlag: **Ergebnis** bleibt, daneben ein Pflichtfeld **Geltungsbereich** mit zeitlicher und räumlicher Angabe. Bei Dauerleistungen trägt der Geltungsbereich die Aussage | |
| A3 | E | Räumlicher Geltungsbereich fehlt ganz | T3: Personenkontrolle gilt vor dem Einlass; dieselbe Tätigkeit durch die Hallenstreife gilt in der Veranstaltung. Ohne Raumangabe sind die beiden nicht unterscheidbar | Kein Feld für Raum im Katalog | Teil von A2, oder eigenes Feld. Entscheidung: eines oder zwei Felder | |
| A4 | Ä | Feld **Auslöser** greift bei Dauermodulen nicht | T3: „Auslöser ist auch so ein bisschen, wenn es halt losgeht" — im EX steht „Veranstaltung / Wahlpflichtmodul", MJ: „Finde ich auch ein komisches Feld" | `modul.md`: „woran erkennt man, dass es losgeht", Pflicht | Ausfüllhinweis ergänzen: Bei Modulen, die mit der Veranstaltung starten, ist der Auslöser die Phase, nicht ein Ereignis. Alternativ Feld auf `gilt-wenn` stellen statt Pflicht | |
| A5 | E | **Phasenprofil** umbenennen | T3: „Phasenprofil würde ich fast umbenennen in so Deadlines" — Zweck: Lead Committee weiß je Phase, worauf zu achten ist, und zum Gate müssen die Entscheidungen durch sein | `modul.md` Block 2: Phasenprofil, Pflicht, Tabelle | Spalten bleiben, Benennung ändern. Vorschlag: **Phasenprofil und Fristen**, mit einer Spalte „bis wann". Reines Umbenennen wäre nach F-03 keine Ebene-2-Sache — es ist eine Ebene-1-Änderung | |
| A6 | Ä | Feld **Fristen** fehlt weiterhin | T3 liefert den konkreten Fall: „bis wann muss es bestellt sein?" — 14 Tage vor VA genannt, dann „vier Wochen wollen sie es meistens vorher"; MJ: „ich werde es nochmal prüfen mit den Phasen" | Bereits als Rückmeldung in `offene-punkte.md` (E-61) notiert, aber nicht im Katalog | Feld **Fristen** in Block 3 aufnehmen (Spalten liegen in der Vorlage schon vor). Erledigt zugleich A5 | |
| A7 | O | Bestellfrist Sicherheitsdienstleister | T3: 14 Tage vs. 4 Wochen, ungeklärt | — | Frage an Frank: welche Frist gilt, und liegt sie in P2 oder P3? | |
| A8 | Ä | Ablauf „vier bis acht Abschnitte" | EX hat drei Abschnitte, einer davon leer | `modul.md`: 4 bis 8, Pflicht | Untergrenze als Richtwert statt Regel. Kleine Module haben weniger | |
| A9 | Ä | Ablauf „keine Verzweigungen" | EX Abschnitt 1 hat als Ergebnis „Ja/nein" — faktisch eine Verzweigung, und im Gespräch war das die natürliche Formulierung | `modul.md`: „keine Verzweigungen" | Regel schärfen: Ein Prüfergebnis ist keine Verzweigung. Verboten sind nur zwei parallel weiterlaufende Abläufe | |
| A10 | E | **Fortschreibung** als Name vs. Einheit | T3 fragt nach der Rolle, Antwort: „214 Security". EX trägt „Abteilung 214 security" | E-39: Fortschreibung ist ein **Name**, ausdrücklich keine Rolle — „eine Rolle, die niemand konkret besetzt, pflegt nichts" | Entweder Namen nachtragen (Head of Security ist im T1 als Frank Haske benannt) oder E-39 revidieren. Empfehlung: Namen nachtragen, E-39 hält | |
| A11 | Ä | **Vertretung** ist zu eng | T3: Vertretung = Dienstleister; gleichzeitig greift Security Management bei Sicherheitslagen selbst ein (Beispiel Spendensammler) | `modul.md`: „eine Rolle", Pflicht | Ausfüllhinweis: Vertretung ist die Rolle, die im Ausfall einspringt — nicht die Rolle, die zusätzlich eingreifen darf. Letzteres gehört in Handlungsvollmacht | |
| A12 | O | Übergeordnete Quality Gates je Phase | T1 (Marvin): „In der Phase 2 haben wir folgende Quality Gates für Security … wahrscheinlich nicht auf Modulebene, sondern eine Art Modulgruppe oder Portfolio, die auf ein übergeordnetes Security Quality Gate einzahlen" | Es gibt Gates je Phasenübergang in `phasen.md`, aber keine bereichsbezogene Aggregation über Module | Klären, ob das ein eigener Baustein wird oder aus den Phasenprofilen der Module erzeugt wird. Empfehlung: erzeugen, nicht neu pflegen | |

---

## B · Security-Detailkonzept

`2_detailkonzepte/module/security-module-detailkonzept/security-modul.md`.

| Nr | Typ | Thema | Aus den Sparrings | Repo-Stand heute | Vorschlag | ok? |
|---|---|---|---|---|---|---|
| B1 | Ä | **Handlungsvollmacht ohne Rückfrage** — Formulierung | T1: Frank kommt mit dem Erklärsatz nicht klar („Das Format regelt das Aufhören und das Informieren, das Anfangen fehlt" — „sperrig, da kommen wir jetzt nicht hin"). MJ sagt zweimal zu, es neu zu formulieren: „sonst verwirrt es die Kollegen" | Genau dieser Satz steht in `security-modul.md` und wörtlich in E-53 | Feld und Spalten bleiben, der Erklärtext wird neu geschrieben. Kern aus dem Gespräch: Der Impuls kommt aus einem Ereignis, nicht aus einer Rolle — und geregelt wird, wer ohne Rücksprache handeln darf und wo Rücksprache zwingend ist (Beispiele: auslaufendes Hydrauliköl auf dem Ladehof → sofort; eskalierende Demonstration → nur mit Polizei) | |
| B2 ✔ | Ä | **„Betriebszustand" ist doppelt belegt** | T1: Frank versteht darunter die zeitliche Folge — Nullbetrieb, technischer Aufbau, vorgezogener Aufbau, regulärer Aufbau, Laufzeit, Abendveranstaltung, Abbau. MJ meint die Eskalationsachse — „Regelbetrieb, Abstimmung im Koordinierungskreis, bei der Gefahrenabwehrbehörde" | `security-modul.md` und E-52 führen „Verhalten im eskalierten Betriebszustand"; die Zustände sollen aus dem Krisenablauf kommen. BaSiGo, das im Repo als Beleg steht, nennt die **zeitlichen** Zustände „Betriebsarten" — die Hauslesart deckt sich damit | **Beschlossen 29.08.:** Das Feld heißt **Verhalten je Eskalationsstufe**, die Tabellenspalte **Eskalationsstufe**. „Betriebszustand" ist damit frei für die zeitliche Achse. Betrifft `security-modul.md`, die Vorlage und E-50/E-52 (Revision nach F-29) | ✔ |
| B2a | E | Eskalationsstufe gegen Eskalationspfad abgrenzen | — | Block 3 führt bereits „Meldeweg und **Eskalation**", V1.0 die Eskalationspfade EP-01/EP-02 (plus EP-03 als Vorschlag) | Ein **Pfad** ist der Weg der Information, eine **Stufe** der Zustand der Lage. Beide gehören ins Glossar, sonst kehrt die Verwechslung eine Ebene tiefer wieder | |
| B2b | O | Braucht die zeitliche Achse einen Ort? | T1 nennt sieben Zustände, drei davon liegen alle innerhalb von P4 (technischer, vorgezogener, regulärer Aufbau) | Die Phasen P0–P7 sind gröber. Eine feinere Zeitachse gibt es im Repo nicht | Erst klären, wenn ein Modul sie braucht. Nicht auf Verdacht anlegen — aber das Wort ist ab jetzt dafür reserviert | |
| B3 | Ä | Führung je Zustand ist jetzt teilweise bekannt | T1: VStättV-Veranstaltungsleitung (TVK) führt in der Laufzeit; ab 18 Uhr trägt der Ordnungsdienstleiter die Abendveranstaltung; in der Nullphase antwortet Security 214; im Aufbau tendenziell der Veranstaltungsleiter. Marvin: „accountable und responsible trennen" | Kein Material dazu im Repo | Nach `4_workspace/` als Vorarbeit für den Krisenablauf. Nicht ins Detailkonzept, das wäre eine eigene Stufenlogik (E-52 verbietet sie ausdrücklich) | |
| B4 | E | Accountable und Responsible trennen | T1 (Marvin und MJ, ausdrücklich einig): „dass wir wirklich accountable und responsible trennen, auch in dem Modul" | `modul.md` trennt Durchführung (Rolle) und Fortschreibung (Name) — das ist eine andere Trennung. Eine A/R-Trennung innerhalb der Durchführung gibt es nicht | Prüfen, ob **Durchführung** in „verantwortet" und „erbringt" aufgeteilt wird. Bei Security fällt es systematisch auseinander: Planung 214, Durchführung 100 % Dienstleister. Ebene-1-Änderung | |
| B5 | Ä | Beispiel Ausgangskontrolle ist nicht hausgedeckt | T1: „Was wir noch nicht machen, das sind die Ausgangskontrollen … das ist halt schwer umzusetzen. Das ist ein Thema für die Zukunft" | `security-modul.md` erklärt das Feld Handlungsvollmacht am Beispiel „leitet unverzüglich Ausgangskontrollen an allen Ausgängen ein" — aus dem anonymisierten Fremdkonzept | Beispiel ersetzen durch einen Fall aus dem Haus (Ladehof-Beispiel aus T1). Sonst steht im Detailkonzept eine Maßnahme, die es hier nicht gibt | |
| B6 | Ä | Benennungsregel nach vfdb trägt nicht durch | T3: „ich glaube, es wäre gut, dass wir mal andere Namen finden … ich glaube, es ist extrem schwierig". Die Hausnamen sind Pünktchenplan, Hallenstreife, Spotter, SCU, ODL | Ausfüllhinweis Modulname: behördlich etablierte Benennung nach vfdb 13-01 übernehmen | Regel bleibt, aber ergänzen: Wo die Hausbezeichnung eingeführt ist, steht sie als Synonym in der Außensicht und im Glossar. Glossareinträge sind ohnehin fällig — SCU, ODL, TVK, Pünktchenplan, Spotter, SDP, OC, VVT | |
| B7 | Ä | Durchführungskontrolle fehlt als Aussage | T2: „die ganze Planung liegt bei euch, die Durchführung 100 % beim Dienstleister — wir machen hier nur Qualitätskontrolle … Stichproben der Qualität: haben wir das bestellte Personal mit der Qualifizierung bekommen, zahlenmäßig und zeitmäßig?" | `modul.md` grenzt Dienstleistersteuerung ausdrücklich aus („liegt in der Linie") | Das ist keine Dienstleistersteuerung, sondern Abnahme der bestellten Leistung je Veranstaltung. Entweder eigenes Modul oder Abschnitt in den betroffenen Modulen. Entscheiden, bevor die Kollegen befüllen | |

---

## C · Pflichtstufe, Modulart, Landkarte

| Nr | Typ | Thema | Aus den Sparrings | Repo-Stand heute | Vorschlag | ok? |
|---|---|---|---|---|---|---|
| C1 ✔ | Ä | Vokabular der Bindung stimmt nicht überein | T3 definiert im Gespräch neu: „Pflicht heißt, ist bei jeder Veranstaltung so. Wahlpflicht gibt es bei jeder Veranstaltung, aber in unterschiedlichen Varianten. Optional heißt, gibt es bei manchen Veranstaltungen, aber nicht bei allen." Die Landkarte in T2 arbeitet durchgehend mit diesen drei | `modul.md`/E-41 führt vier Werte: `gilt immer`, `gilt auf Bedarf, wenn …`, `Wahlpflicht — Grundmodul`, `Wahlpflicht — Alternative zu …` | **Beschlossen 29.08.:** Das Feld heißt **Pflichtstufe**, die Werte sind **Pflicht / Wahlpflicht / Optional** — das Hausvokabular gilt innen wie außen. Damit gibt es nur noch eine Sprache; das Mapping entfällt | ✔ |
| C1a | **E** | Grundmodul und Alternative brauchen ein eigenes Feld | — | E-41 packt vier Werte in ein Feld und mischt dabei zwei Aussagen: *wie verbindlich* (Pflicht/Wahl/Optional) und *welche Rolle in der Gruppe* (Grundmodul/Alternative) | Mit drei Werten für die Pflichtstufe muss die Gruppenrolle daneben: **bei Wahlpflicht** zusätzlich `Grundmodul` oder `Alternative zu …`. Sauberer als bisher und hält E-41 (Entscheider und Frist stehen genau einmal im Grundmodul). Braucht eine Revision von E-41 | |
| C1b | Ä | Vier „Pflicht"-Wörter nebeneinander | — | Im Repo stehen bereits **Pflichtschwelle** (rechtliches Minimum), **Pflichtfeld** (Katalog) und **Verbindlichkeitsstufe** (Attribut der Rechtsgrundlage, E-57) | **Pflichtstufe** kommt als viertes dazu. Alle vier ins Glossar, sonst verschmilzt Pflichtstufe mit Pflichtschwelle — und genau die beiden dürfen nicht verschmelzen (E-42: das Grundmodul darf nicht unter die Pflichtschwelle fallen) | |
| C2 | **E** | Pflichtstufe ist nicht statisch | T2/T3 mehrfach: Optionales wird zur Pflicht, wenn Risikobewertung, Lagebild, Ordnungsamtsbescheid oder die Ausstellerlage es verlangen. „Das kann durchaus zu jeder Veranstaltung zur Pflicht werden, wenn es eine Risikobewertung oder das Lagebild vorgibt" | `modul.md` deckt nur die Untergrenze ab (das Grundmodul darf nicht unter die Pflichtschwelle fallen) | Regel ergänzen: **Optional** trägt einen benannten Auslöser mit Art — **Zahl**, **Bewertung** oder **Bescheid** (analog zur Auslöseschwelle). Damit ist die Hochstufung dokumentiert, ohne dass die Modulart wechselt | |
| C3 | E | Modulart von Personen- und Gepäckkontrolle | T2 schwankt: Personenkontrolle ist Compliance, weil das Messerverbot geprüft werden muss — oder Leistung, weil die Zutrittskontrolle rechtlich nicht vorgeschrieben ist. Gepäckkontrolle „rutscht hoch", wenn ein Bescheid es verlangt | EX trägt `modulart: Compliance`. E-58(a) verbietet, Compliance und Leistung in einem Modul zu mischen | Sauber ist: Der **Prüfauftrag** (Messerverbot) ist Compliance, die **Kontrollart** ist Ausprägung. Vorschlag: Personenkontrolle = Compliance mit Wahlpflicht-Varianten; Gepäckkontrolle = eigenes Modul, `gilt auf Bedarf, wenn` (Bescheid oder Bewertung). Bestätigen | |
| C4 | O | Dritte Modulart (Enablement) | T1: MJ tendiert zu nein, will die Kategorie aber offenhalten. Marvin nennt die Fremdfirmeneinweisung, Frank ergänzt: nicht nur eigene Nachunternehmer | E-48 offen, E-62 trägt Evidenz dagegen (Unterweisung folgt aus § 42 Abs. 2 VStättVO u. a. → Compliance) | Bleibt offen. Aber: Es gibt jetzt einen Kandidaten aus dem Haus — die veranstaltungsspezifische Dienstleistereinweisung. In `offene-punkte.md` nachtragen und im Workshop entscheiden | |
| C5 | **E** | Schnitt Personenkontrolle / Identitätsmanagement | T3, ausführlich verhandelt: Personenkontrolle ist dem Identitätsmanagement **vorgeschaltet**, vor der Ticketkontrolle. Zwei diskrete Pakete, andere Ausführende, sehr schnell hintereinander, für den Besucher ein Flow. „Es gibt kein Drehkreuz ohne Spotter" — der Spotter ist das Minimum der Personenkontrolle, unabhängig vom ID-Verfahren | Kein Modul im Repo | Als Schnittentscheidung festhalten. Ticketkontrolle ist technisch und Pflicht; die intensivierte Prüfung (personifiziertes Ticket, Abgleich mit Ausweis) ist ein zubuchbares Modul | |
| C6 | E | Gleichnamiger Schritt ist kein Modul | T3: „die tatsächliche Personenkontrolle ist einfach ein Schritt" — sie kommt auch in der Hallenstreife vor | `modul.md` sagt „einzelner Prozessschritt ist kein Modul" und „ein Teilkonzept ist ein Lieferobjekt, kein Modul" — der Fall gleicher Name für Modul und Schritt ist nicht geregelt | Vierte Schnittregel für Security analog zur Teilkonzept-Regel: Ein Ablaufschritt, der in mehreren Modulen vorkommt, wird nicht zum eigenen Modul; unterschieden wird über den Geltungsbereich (siehe A3) | |
| C7 | E | Besucherhöchstzahlen | T3: verortet bei der Personenkontrolle, weil dort gezählt wird — nicht beim Identitätsmanagement. Im Gespräch mit sichtbarer Unsicherheit („Schwierig, das zu klären") | EX trägt es im Zweck | Im Workshop gegenprüfen. Kandidat für ein eigenes Modul Kapazitätsüberwachung — § 1 Abs. 2 VStättVO bemisst die Kapazität normativ, das steht schon in `bemessungsverfahren.md` | |
| C8 | Ä | **Modullandkarte existiert nicht** | T2 hat sie inhaltlich weitgehend erzeugt (siehe Abschnitt F). MJ will sie in den Workshop mitbringen und gegen das Security-Konzept laufen lassen | F-26 sagt: Landkarte gehört nach Ebene 3. `3_instanzen/module/security-module-instanzen/README.md` verweist aber auf Ebene 2. **Widerspruch, und die Datei gibt es nirgends** | Landkarte in Ebene 3 anlegen, README korrigieren. Inhalt aus T2 | |
| C9 | O | Vollständigkeitstest der Landkarte | Übergabedokument, Befund 9: Grafik 6 als Prüfraster (Phasen × Einheiten). T1: MJ will die Landkarte zusätzlich gegen Franks Sicherheitskonzept laufen lassen | Noch nicht gemacht | Beides vor dem Workshop. Das anonymisierte Konzept liegt in `0_meta/quellen/` | |

---

## D · Neue Fakten aus dem Haus — was Repo-Annahmen ändert

Das sind die Punkte, bei denen im Repository etwas steht, das nach den Sparrings nicht mehr stimmt.

| Nr | Typ | Thema | Aus den Sparrings | Repo-Stand heute | Vorschlag | ok? |
|---|---|---|---|---|---|---|
| D1 ✔ | Ä | **Es gibt ein Rahmensicherheitskonzept** | T1, Frank wörtlich: „In der Tat haben wir ein Rahmensicherheitskonzept, das damals erstellt worden ist. Es hatte primär die Geländesicherheit im Fokus … stark safety-getrieben … Wir haben die Gefahrenabwehrpläne in diesem Rahmensicherheitskonzept mit eingebracht und daraus wird dann das veranstaltungsbezogene Sicherheitskonzept generiert" | E-55 hat die Zusatzangabe „Verhältnis zum Rahmensicherheitskonzept" **gestrichen**, ausdrücklich mit der Begründung: „nach Auskunft der Projektleitung gibt es im Haus eher je Veranstaltung ein eigenes Konzept". Dieselbe Annahme steht in `offene-punkte.md` und in `rechtsrahmen.md` | **Beschlossen 29.08.:** Das gestrichene Feld kommt **nicht** zurück — Kopplungsregel 6 (referenzieren statt duplizieren) trägt den Fall unabhängig davon, ob es ein Rahmenkonzept gibt. Der eigentliche Defekt ist, dass E-55 eine Konzeptentscheidung an einer Hausauskunft aufgehängt hat. Drei Stellen, drei Behandlungen: **(a)** E-55 — Begründung austauschen (Kopplungsregel 6 statt Hausauskunft), Revision nach F-29 anhängen; die Annahme darf im Log stehenbleiben, aber nicht als Begründung. **(b)** `offene-punkte.md` — von Frage zu Feststellung: es gibt eins, safety-getrieben, Owner war 420. **(c)** `rechtsrahmen.md` Z. 108 — **raus**, das ist eine Konzeptdatei | ✔ |
| D2 | Ä | Bestellung des Sicherheitsdienstleisters — Widerspruch aufgelöst | T1, Frank: „Wer löst sie aus? Wir lösen sie aus, also im Jaggaer bucht es 410 auf die Kostenstelle … es ist eine Abstimmung zwischen Security und Dienstleister, aber mit maximalem Impuls von TVK". Und: „Die Personalanforderung … wird von 410 beauftragt. Das ist also nicht von uns bestellt, sondern wird durch 410 bestellt" | Übergabedokument, Befund 8: V1.0 sagt zweierlei (Expo Realisation löst aus / Customer Success handhabt), markiert als **blockierend**. In `offene-punkte.md` als CP-2d geführt | Befund ist beantwortet: **410 / TVK bestellt, 214 Security bereitet fachlich vor.** Weder Expo Realisation noch Customer Success. Als Entscheidung (durch Messe) loggen, Befund schließen. EX bildet es bereits so ab | |
| D3 | Ä | Bemessungsverfahren Ordnungsdienst — erhoben | T2: Grundlage ist der Pünktchenplan — Gelände mit Positionen aus 2018/19, gefiltert nach bespielten Hallen und Achsen, auf Basis von Gefährdungs-/Risikoeinschätzung und Lagebild; Ergebnis ist die Bestellung (ODL, Abschnittsleiter, Kontrollkräfte mit Qualifikation, Hallenstreife). Verhandelt mit dem Dienstleister, abgestimmt mit 410 | `bemessungsverfahren.md`, offener Punkt: „Für den Ordnungsdienst existiert kein anerkanntes Bemessungsverfahren. Was das Haus stattdessen benutzt, ist zu erheben" | Erhoben. Als Verfahren eintragen: Positionsbasiert (Pünktchenplan), Eingangsgrößen Hallenbelegung, Eingänge, Besucherprognose, Lagebild; Ergebnisart Richtwert; Abnahme 214 im Einvernehmen mit 410 | |
| D4 | Ä | Bemessung Brandsicherheitswache — extern gesetzt | T2: „da kriegen wir ein Mengengerüst von der Feuerwehr, die schätzt die Veranstaltung je nach belegten Hallen und prognostizierter Besucherzahl ein und gibt uns einen Rahmen vor … und keine Abweichungen davon" | Verfahrenstabelle in `bemessungsverfahren.md` ist leer | Zeile eintragen: Quelle Feuerwehr, Normqualität Behördenauflage, Ergebnisart **Mindestwert**, Abnahme durch die Feuerwehr. Erste gefüllte Zeile überhaupt | |
| D5 | O | Wo die Sicherheitsdokumentation heute liegt | T1, Frank: „Dokumentiert wird das alles in E-Mails und im Security-Postfach … mir wäre es lieber, wenn wir das plastischer, griffiger dokumentieren könnten. Aber so ist halt das Doing hier" | Nicht im Repo | Als Ist-Befund in `offene-punkte.md`. Er begründet den Reifegrad 1 (personengebunden) bei den meisten Modulen und ist zugleich das Nutzenargument gegenüber dem Team | |
| D6 | O | Vier Anlagen des Referenzkonzepts | Nach D1 wahrscheinlich im Rahmensicherheitskonzept enthalten — der Gefahrenabwehrplan ist laut T1 ausdrücklich dort eingebracht | `offene-punkte.md`: „Ob es diese Bestandteile im Haus gibt und wo sie geführt werden, ist offen" | Für den Gefahrenabwehrplan geschlossen. Funkregeln, sicherheitstechnische Anlagen und Glossar bleiben offen | |
| D7 | Ä | SCU — Grenzfall Linie / Veranstaltung | T2: SCU ist 365 Tage besetzt, wird aus dem Security-Budget bestellt, nicht durch TVK. Aber sie übernimmt während der Veranstaltung Aufgaben (Fundsachen, Videoauswertung, Brandmeldeanlage). Im Gespräch am Ende als **Schnittstelle** markiert, nicht als Modul | `modul.md`: „Veranstaltungsübergreifender Prozess der Organisation → Verweis, nicht nachschreiben" | Deckt sich. SCU wird kein Modul, sondern steht als Schnittstelle in den Modulen, die sie berührt. Entscheidung festhalten, sonst kommt sie im Workshop wieder | |
| D8 | E | Zufahrt und Ladehof | T1: „Wenn es ein Tor gibt, dann ist es security-relevant" — Frank und Marvin bestätigen, dass der Security-Anteil nicht wegfällt. Dazu die ungelöste Doppelbesetzung an Tor 5 (gelbe Weste Logistik, rote Weste Security), die Frank „am liebsten auflösen würde", aber vertraglich nicht kann | Übergabedokument, Befund 7: Der Ordner heißt Security, Owner ist „AL Logistik + Security", Ladehof-Themen liegen an einer bereichsinternen Grenze | Bestätigt mit Präzisierung: Der Security-Anteil (welche Tore offen, wie besetzt, Zutritt) bleibt in Security-Modulen; die Verkehrsführung nicht. Doppelbesetzung Tor 5 als offenen Punkt aufnehmen | |

---

## E · Repo-interne Inkonsistenzen

Unabhängig von den Sparrings beim Durchgehen aufgefallen.

| Nr | Typ | Fund | Vorschlag | ok? |
|---|---|---|---|---|
| E1 | Ä | `offene-punkte.md` Z. 127 verweist CP-2d nach `security-module-detailkonzept/uebergabekarte.md`. Diese Datei ist durch **F-26 gestrichen** | Verweis korrigieren. Mit D2 ohnehin fällig | |
| E2 | Ä | `3_instanzen/…/README.md` verweist die Modullandkarte nach Ebene 2, **F-26** legt sie nach Ebene 3 | README korrigieren, Landkarte in Ebene 3 anlegen (C8) | |
| E3 | Ä | `offene-punkte.md` Z. 209 zitiert „**R-23**". Eine R-Reihe gibt es nicht — das Log führt nur F und E | Auf die richtige ID korrigieren oder die Klammer streichen | |
| E4 | Ä | EX trägt `id: MOD-SEC-Test01` — F-24 verlangt `MOD-<BEREICH>-<NR>` | Beim Übertragen in Ebene 3 eine echte Nummer vergeben | |
| E5 | Ä | EX-Frontmatter ist unvollständig gegenüber der Vorlage: `modulname`, `pflichtstufe` (bisher `bindung`), `ausloeser-phase`, `schwerpunkt-phase`, `risikostufe`, `reifegrad-ist/-ziel`, `version`, `pruefintervall`, `dokumentfreigabe` fehlen | Für die Testbefüllung unkritisch. Vor dem Workshop entscheiden, ob die Vorlage das Frontmatter überhaupt zeigt — es hat die Kollegen erkennbar nicht erreicht | |
| E6 | Ä | EX trägt `quelle: Live-Erfassung Sparring 2, 2026-08-25` und `stand: 2026-08-25`; die Sitzungen waren am **24.08.2026** | Datum korrigieren | |
| E7 | Ä | EX: Lieferobjekt Statistik ohne Ablageort — der ist Pflicht | Als Lücke markieren statt leer lassen | |

---

## F · Modullandkarte — Kandidaten aus T2 und T3

Rohstand aus dem Gespräch, nicht validiert. Grundlage für C8.

| Kandidat | Einordnung im Gespräch | Anmerkung |
|---|---|---|
| Personenkontrolle | Compliance, Wahlpflicht | Varianten: Spotter-Stichprobe (Minimum) → Torbogen/Handgerät → 100 % mit Zelt und Zaun. Vorgeschaltet zum Identitätsmanagement |
| Gepäckkontrolle | Leistung, optional — hochstufbar | Eigene Zielrichtung. Varianten: Nachschau durch Kontrollierende → X-Ray |
| Identitätsmanagement / Ticketkontrolle | Pflicht | Immer technisch (Drehkreuz), nur digitale Tickets |
| Prüfung personifizierter Tickets | Leistung, optional | Ticket-plus-Ausweis-Abgleich, aus Frankreich mitgebracht, in Vorbereitung |
| SDP — Service-Ticketing-Portal | Pflicht | Legitimierung von Nicht-Besuchern/Nicht-Ausstellern, außerhalb der Laufzeit |
| Hallenstreife Laufzeit | Compliance, Pflicht | Intensität skaliert (Wahlpflicht über die Menge). Überwacht auch das Rauchverbot |
| Hallenstreife Auf- und Abbau | Pflicht, eigenes Modul | Andere Zielrichtung: Rettungswegfreiheit, Diebstahlprävention. Vertretungstest schlägt an |
| Ordnungsdienstleiter (ODL) | Compliance, Pflicht | Aus VStättV; separat bestellt, nur für die Veranstaltung |
| Brandsicherheitswache | Compliance, Pflicht | Mengengerüst von der Feuerwehr, keine Abweichung |
| Lagebild | 365 Tage, Linie | Grundlage für alles Weitere |
| Lagebesprechung der Veranstaltung | Pflicht | Morgenlage 8:30, standardisiertes Protokoll, im Kriseninterventionsraum. Beim Gastveranstalter dort |
| Erstellung Pünktchenplan | Leistung/Pflicht | Ergebnis ist die Bestellung. Grundlage: Gefährdungseinschätzung und Lagebild |
| Durchführungskontrolle | offen | Qualitätsstichproben beim Dienstleister — siehe B7 |
| VIP- und Personenschutz | Leistung, optional | Auslöser: Schutzpersonen, gefährdete Aussteller |
| Querüberwachung Parallelveranstaltung | Compliance, eher Betreiber | Trennung der Besuchergruppen |
| Demonstrationen | optional | Nur bei Anmeldung; Aufklärung durch die SCU |
| Drohnenflug | Leistung/Auflage, optional | Nachweise, Genehmigung Luftfahrt-Bundesamt |
| Datenschutzkonformität auf Ständen | offen | Videokameras der Aussteller; Aufklärung über AGB, Kontrolle anlassbezogen |
| Interventionsdienst | offen | Anlassbezogenes Eingreifen bei Verstößen (Beispiel Hanfprodukte Biofach) |
| SCU | **kein Modul** | Schnittstelle, siehe D7 |
| Shuttlebusse | **nicht Security** | Logistik |
| Arbeitsschutz / VVT | **nicht Security** | Abteilung 420 |

---

## G · Projektplan

| Nr | Typ | Punkt | Aus den Sparrings | ok? |
|---|---|---|---|---|
| G1 | P | Touchpoint zu zweit | 1. September, 11:00–13:00 | |
| G2 | P | Check-in zu dritt | 17. September, 9:00–10:00, Titel „Check-in Security Modul, Konzept und Workshop Design" | |
| G3 | P | Workshop 1 | 30. September, ganztägig — 9–16 oder 10–17 Uhr. Blocker wird von Frank oder Marvin verschickt, damit die Kollegen mit eingeladen werden | |
| G4 | P | Workshop 2 | Nur als Blocker vormerken, Termin bewusst offen. Dazwischen ein Check-in zum Kalibrieren, gemeinsam mit den Kollegen | |
| G5 | P | Teilnehmerkreis Workshop 1 | Frank, Ralf, Kai (seit 1. August im Haus) plus Marvin und Bereichsleitung. Logistik ausdrücklich **nicht** — erst nach Security, dann über das Process-Programm | |
| G6 | P | Rollen in der Phase | Inhaltliche Befüllung: Fachbereich Security. Fachliche Prüfung und Freigabe der Detailtiefe: Frank. Eskalation und Abnahme: Marvin. Formale Prüfung (Konsistenz, Vollständigkeit): 1789 | |
| G7 | P | Kapazitätsrisiko | Galabau läuft, SPS ist die größte Herbstveranstaltung und bindet Markus. Grober Rahmen: über den Herbst | |
| G8 | P | Zielbild der Phase | Landkarte → so viele Module wie möglich befüllen → Konsolidierung im zweiten Workshop → Redaktion → Security V1. Erreichbar ist Reifegrad 2 (beschrieben); Reifegrad 3 entsteht erst bei einer echten Veranstaltung | |
| G9 | P | Datumsprüfung | Die Terminabstimmung im Transkript ist stellenweise unsauber (Woche vom 7.–10., dann „Zweiter, Dritter", dann „Erster"). G1 bitte gegen deinen Kalender prüfen | |
| G10 | O | Ablageort des Datensatzes | T1: „Hier sollten wir auf jeden Fall noch mal mit IT / AI sprechen, wo das am Ende landet." Hängt am offenen Punkt Ausgabeformat der Vorlage | |

---

## H · Vor dem Workshop zu erledigen

Aus T3 explizit als Nacharbeit benannt, ergänzt um das, was aus den Befunden folgt.

| Nr | Punkt | hängt an | ok? |
|---|---|---|---|
| H1 | Umbenennungen umsetzen: **Pflichtstufe** statt Bindung, **Eskalationsstufe** statt Betriebszustand — in `modul.md`, `security-modul.md`, Vorlage, Frontmatter-Schlüssel; E-41, E-50, E-52, E-55 als Revisionen | B2, C1, D1 | |
| H2 | Pflichtstufe in der Vorlage sichtbar aufnehmen — sie fehlt im Kurzsteckbrief | C1, C1a, E5 | |
| H3 | Feld Ergebnis und Geltungsbereich anpassen | A2, A3 | |
| H4 | Phasenprofil und Fristen zusammenführen | A5, A6 | |
| H5 | Handlungsvollmacht neu formulieren | B1 | |
| H6 | Glossareinträge, die die vier Pflicht-Wörter und Stufe gegen Pfad trennen | B2a, C1b | |
| H7 | Modullandkarte erstellen und gegen Franks Sicherheitskonzept prüfen | C8, C9 | |
| H8 | MOD-SEC-Test01 vollständig ausdifferenzieren als Musterbeispiel — MJ in T3: „gefühlt noch nicht so ganz ready, dass wir in den Workshop gehen" | alles darüber | |
| H9 | Glossareinträge: SCU, OC, ODL, TVK, VVT, Pünktchenplan, Spotter, SDP, Morgenlage | B6 | |
