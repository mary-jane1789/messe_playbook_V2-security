---
status: laufend
stand: 2026-08-23
---

# Entscheidungen

Zwei Reihen, weil sie verschiedene Urheber und verschiedene Verbindlichkeit
haben:

- **F** — Format und Repository. Aufbau, Konventionen, Arbeitsweise. Wird von
  1789 entschieden und hier mit Begründung festgehalten.
- **E** — Inhalte. Was aus dem Playbook und dem Modul-Framework übernommen wird,
  wie es benannt und geschnitten ist. Die Spalte `durch` zeigt, wer entschieden
  hat; offene Bestätigungen stehen in `offene-punkte.md`.

## Regeln für dieses Log

**Gebündelt, nicht laufend.** Einträge entstehen einmal am Ende eines
Arbeitstages, nicht während des Gesprächs. Ein Log, das jeden Zwischenschritt
mitschreibt, wird unlesbar.

**IDs werden nie neu vergeben.** Die E-Reihe setzt die Nummerierung aus
Kapitel 9 des Modul-Frameworks fort und beginnt deshalb bei E-14. Die dort
ausgefallenen Nummern E-01, E-06 und E-08 bleiben Lücken. Die F-Reihe beginnt
bei F-01.

**Revisionen werden angehängt, nicht überschrieben.** Wird eine Entscheidung
geändert, kommt ein neuer Eintrag dazu, der auf den alten verweist. Der alte
bleibt stehen.

---

## F — Format und Repository

### 2026-08-19

| ID | Entscheidung | Begründung |
|---|---|---|
| F-01 | Sechs Ordner, vier inhaltliche Ebenen. Der Ort ergibt sich aus vier Fragen in fester Reihenfolge. | Reichweite ist das einzige Zuordnungskriterium, das nicht vom Reifegrad abhängt. Damit ist der Ort bestimmbar, ohne zu diskutieren. |
| F-02 | Dateiformat Markdown durchgehend, Frontmatter für die strukturierten Felder. | Der Inhalt ist Prosa und Tabellen. Markdown ist exportierbar, im Diff lesbar und vom Fach bearbeitbar; das Frontmatter hält die filterbaren Felder maschinell auswertbar. |
| F-03 | Ebene 2 wendet Ebene 1 an und definiert nicht neu. Keine zweite Feldliste; Felder ergänzen ist erlaubt, umbenennen, weglassen oder anders bedeuten nicht. | Felder variieren über die Modulart, nicht über den Bereich. Zwei Feldlisten wären zwei Kataloge — nicht vergleichbar und nicht generierbar. |
| F-04 | Idee und Konkretisierung stehen in derselben Datei. Getrennt wird nur, wo Instanzen vielfach und unabhängig voneinander entstehen. | Zwei Dateien, die immer gemeinsam geändert werden müssen, sind eine zu viel. |
| F-05 | Ebene 1 hält Schemata. Schema im Singular, entschiedene geschlossene Menge im Plural. | Der Dateiname zeigt den Typ, ohne die Datei zu öffnen. |
| F-06 | Jede Datei in Ebene 1 deklariert im Frontmatter `instanzen:` — `inline`, ein Ordnerpfad, oder `keine bisher`. | Ebene 1 mischt Schemata mit und ohne eigene Instanzen. Ohne Deklaration ist nicht erkennbar, ob eine Datei vollständig ist, und die Mischung driftet unbemerkt. |
| F-07 | Ein Schema verweist auf den Ordner seiner Instanzen, nie auf einzelne Dateien darin. | Der Ordnerpfad bleibt stabil; eine Dateiliste müsste bei jeder neuen Instanz angefasst werden. |
| F-08 | Status und Reifegrad stehen im Frontmatter, nicht im Ablageort. | Sonst wandern Dateien beim Reifen von Ordner zu Ordner und jeder Verweis darauf bricht. |
| F-09 | Ebene 3 gliedert nach Baustein, nicht nach Bereich: `module/<bereich>/` und `ablaeufe/`. | Module haben eine Bereichsdimension, Abläufe nicht. Ein Bereich und ein Baustein dürfen nicht auf derselben Ebene stehen. |
| F-10 | Abläufe sind ein eigener Baustein mit Schema in Ebene 1 und eigenem Ordner in Ebene 3. | Retrospektive, Krise und Konfiguration sind weder Modul noch Rolle noch Phase. Ohne eigenen Baustein bleiben sie heimatlos. |
| F-11 | Neue Bereichsordner werden erst angelegt, wenn der Bereich beauftragt ist. | Leere Platzhalter behaupten eine Vollständigkeit, die nicht da ist. |
| F-12 | Entscheidungen und offene Punkte werden getrennt geführt. IDs werden nie neu vergeben. | Verschiedene Lebensdauer. In Kapitel 9 des Frameworks und in Anhang A des Playbooks sind Nummern ausgefallen — beide Listen sind dadurch nicht zitierfähig. |
| F-13 | Dieses Log führt zwei Reihen: F für Format und Repository, E für Inhalte. Einträge entstehen gebündelt am Ende eines Arbeitstages. | Getrennte Urheber und getrennte Verbindlichkeit. Laufendes Mitschreiben macht das Log unlesbar. |
| F-14 | Nichts wird ohne Freigabe übernommen: prüfen, vorlegen, besprechen, migrieren. | Das Playbook V1.0 ist verabschiedet; stille Übernahmen mit Interpretation wären nicht mehr unterscheidbar vom Original. |
| F-15 | Die Projektleitung gibt die leere Steckbrief-Vorlage heraus, das Fach füllt aus, die Projektleitung übergibt den Rücklauf zum Auslesen. Die Datei im Repository ist danach der Datenstand; Word, PDF und Außensicht sind immer Ausgabe. | Zwei Datenstände laufen auseinander. Es kann nur einen geben. |
| F-16 | Beim Übertragen wird nichts ergänzt und nichts verloren: leere Felder bleiben leer und werden markiert, nicht zuordenbare Inhalte gehen in die offenen Punkte oder als Frage zurück. | Still verschwundene Inhalte sind das größere Risiko als falsche — falsche fallen auf. |
| F-17 | Jeder Blattordner ist repositoryweit eindeutig und nennt seinen Typ: `security-module-detailkonzept/`, `security-module-instanzen/`. Die Bausteinebene (`module/`) darf sich wiederholen. | Ein Pfadsegment wie `security/`, das an zwei Stellen vorkommt, sagt allein nicht, wo man ist — nicht in der Suche, nicht im Editor-Tab, nicht im Verweis. Ergänzt F-01. |
| F-18 | Abläufe liegen in Ebene 2, nicht in Ebene 3. **Revidiert F-10 und die Ortsangabe in E-28.** Damit ist die Grenze zwischen den Ebenen geschärft: Ebene 2 sind Konzepte, Ebene 3 sind ausgefüllte Schemata. | Ein Krisenablauf ist ein Konzepttext, kein gefülltes Formular. Die vorherige Zuordnung hätte Ebene 3 zu zwei verschiedenen Dingen gemacht. Folge: Ebene 2 ist nicht mehr nur bereichsspezifisch. |
| F-19 | Ebene 2 und Ebene 3 sind gleich gegliedert: Ebene, dann Baustein, dann die konkrete Sache. **Revidiert F-09.** | Symmetrie zwischen den Ebenen orientiert beim Navigieren. Der Preis ist, dass `module/` zweimal vorkommt; der nummerierte Elternordner macht den Pfad trotzdem eindeutig. |
| F-20 | Dieses Repository ist die Backstage des Playbooks: Es hält die Ergebnisse und zusätzlich die Architektur, Struktur und Methodik, aus denen sie entstanden sind. Das Playbook zeigt nur die Ergebnisse. | Ein Ergebnis ohne seine Herleitung lässt sich nur ersetzen, nicht fortschreiben. Die Weiterentwickelbarkeit des Playbooks hängt daran, dass Schnitt, Feldlogik, Auslassungen und offene Fragen an einem Ort nachlesbar bleiben. |

### 2026-08-23

| ID | Entscheidung | Begründung |
|---|---|---|
| F-21 | Der Referenzrahmen ist die Eigenveranstaltung. Das steht in `README.md` und in `CLAUDE.md`, und es gilt als Schreibregel: Eine Aussage, die nur für Gast oder Partner gilt, sagt das ausdrücklich; ohne Vermerk gilt sie für Eigen. | V1.0 legt die Eigenveranstaltung als Referenzrahmen fest, sagt es aber nur im Abschnitt Versionierung. Ohne Vermerk an sichtbarer Stelle liest jeder Satz im Repository wie eine Aussage über alle Veranstalter-Modelle. |
| F-22 | Grafiken sind keine Wertequelle. Sie belegen Anzahl und Reihenfolge, nicht Werte. | Grafik 5 in V1.0 hat eine gleichmäßig geteilte, damit nichtlineare Zeitachse. Drei ihrer Labels liegen auf Phasengrenzen und widersprechen dort der Übersichtstabelle. Ein Schema ohne maßstäbliche Achse trägt keine Zahlen. |
| F-23 | Quelldateien in `0_meta/quellen/` werden nicht korrigiert. Fehler und veraltete Zählungen werden beim Migrieren umgerechnet, die Quelle bleibt unangetastet. Soll eine korrigierte Fassung entstehen, wird sie als neue Version daneben gelegt. | Eine überschriebene Quelle verliert ihren Wert als Beleg: Es ist danach nicht mehr unterscheidbar, was im Original stand und was wir korrigiert haben. Genau das soll das Feld `quelle` verhindern. |
| F-24 | Modul-IDs folgen dem Muster `MOD-<BEREICH>-<NR>`. Das Präfix `M-` bleibt für Schemata reserviert. | Die ID zeigt den Typ, ohne die Datei zu öffnen. `Modul` war in den Vorquellen doppelt belegt — als Playbook-Baustein und als Leistungsbaustein; getrennte Präfixe machen das Zitieren eindeutig. Beantwortet die bis dahin offene ID-Frage in `konventionen.md`. |
| F-25 | Der Feldkatalog führt fünf feste Spalten: Feld, gilt-wenn, Zone, Pflicht oder optional, Wertebereich. | Aus dem Katalog sollen der leere Steckbrief und später die Darstellung erzeugt werden. Ohne feste Spalten ist er nicht maschinell auflösbar, und `gilt-wenn` ist die Spalte, die das typabhängige Ausblenden von Feldern überhaupt möglich macht. |

---

## E — Inhalte

### 2026-08-19 · Durchgang durch die 16 Kapitel des Playbooks V1.0

| ID | Entscheidung | durch |
|---|---|---|
| E-14 | Die einleitenden Kapitel — Worum geht es, Verankerung im Unternehmen, Leitprinzipien, Geltungsbereich — gehen in den Projektkontext, nicht in ein Grundkonzept. | 1789 |
| E-15 | Veranstaltung wird Grundkonzept, mit allen drei Kategorisierungen und den Unterschieden nach Veranstalter. | 1789 |
| E-16 | Phasen wird Grundkonzept, P0 bis P7, mit den Gates an den Übergängen. | 1789 |
| E-17 | Gate wird Glossareintrag, kein eigenes Grundkonzept. Die konkreten Gates stehen in `phasen.md`. | 1789 |
| E-18 | Check-Points werden nicht übernommen. Sie sind dieselbe Art Ding wie die Übergaben eines Moduls — und nicht dasselbe wie Gates: ein Gate ist eine Bedingung an einem Phasenübergang, ein Check-Point eine Übergabe zwischen Rollen, meist innerhalb einer Phase. | 1789 |
| E-19 | Die methodische Empfehlung zum Service Blueprint wird nicht übernommen. | 1789 |
| E-20 | Rollen werden auf zwei Grundkonzepte aufgeteilt: `lead-modell.md` und `rolle.md`. | 1789 |
| E-21 | Gremium wird als Schema aufgenommen. Die konkreten Gremien sind Entwürfe und werden nicht festgeschrieben. | 1789 |
| E-22 | Eskalationspfade werden kein eigenes Grundkonzept, sondern Teil des Krisenablaufs. | 1789 |
| E-23 | Entscheidungstypen werden nicht übernommen. | 1789 |
| E-24 | `dienstleister.md` wird Grundkonzept — Kategorien und die Einordnung Pflicht / Wahl-Pflicht / Wahl. Vollständigkeit der Kategorien ist mit der Messe zu klären. | 1789 |
| E-25 | Abrechnungsmodelle werden nicht übernommen. Kein Modul braucht sie, um beschrieben zu werden; die Verrechnungseinheit ist ein Feld im Modul. | 1789 |
| E-26 | SLAs werden nicht übernommen. Dienstleistersteuerung liegt in der Linie, nicht im Modul. | 1789 |
| E-27 | Risikomanagement wird kein Grundkonzept. Die Risikostufe wird ein Feld im Modul (`niedrig / mittel / hoch`), „hoch" löst eine Pre-mortem-Pflicht aus. | 1789 |
| E-28 | Konfiguration, Krisenablauf und Lernschleife werden Abläufe in Ebene 3. Alle drei sind Entwürfe. Damit sind Krise und Triage, Retrospektiven und das Pre-mortem eingeordnet. | 1789 |

### 2026-08-19 · Migration `veranstaltung.md`

| ID | Entscheidung | durch |
|---|---|---|
| E-29 | `veranstaltung.md` ist übertragen (V1.0 Kap. 1 und 4): die drei Achsen Art, Veranstalter, Größe; Veranstalter gegen Betreiber; die drei Veranstalter-Modelle; die vier Regeln aus Kap. 4; der Add-on-Grundsatz. Nicht übernommen: Ticketpreise, Beispielveranstaltungen, Segmentcharakterisierung, Grafik 3 und 4, die Add-on-Beispiele. Konkretisiert E-15. | 1789 |
| E-30 | Die Werte der Größenklassen sind Richtwerte, keine Schwellen. Die Einstufung nimmt die für die Veranstaltung verantwortliche Rolle vor. | 1789 |

### 2026-08-23 · Migration `phasen.md`

| ID | Entscheidung | durch |
|---|---|---|
| E-31 | Die Phasenzählung ist P0 bis P7. V1.0 ist damit Source of Truth; das Modul-Framework wird angepasst, nicht umgekehrt. An der Quelle nachgeprüft: P0–P7 steht an 13 Stellen, darunter alle vier tragenden. Die drei abweichenden Stellen sind zweimal derselbe Zahlendreher im Satz zur Zusammenlegung („acht Phasen, benannt P0 bis P6" — das sind sieben) und einmal ein Label aus der Zählung vor der Zusammenlegung („nach P8", gemeint ist die Nachbereitung, also P7). | 1789 |
| E-32 | Die Umrechnung vom Modul-Framework auf V1.0 lautet: P0, P1 und P2 bleiben, P3 bis P8 minus eins. Alte P2 und alte P3 gehen in die neue P2 auf; 3−1 = 2 trifft das, deshalb genügt eine Regel ohne Fallunterscheidung. Betroffen sind neun Stellen im Framework. | 1789 |
| E-33 | `phasen.md` ist übertragen (V1.0 Kap. 2, Geltung aus Kap. 4): P0 bis P7 mit Name, Zeitfenster und Primär-Träger, die acht Gates einschließlich P7 → P0, dazu ein kurzer Abschnitt, wozu das Phasenmodell dient. Nicht übernommen: der Absatz „Warum acht Phasen", die Warum/Was/Wer/Wie-Blöcke der acht Phasensektionen, die zwei Stränge in P2, Bestellweg und Abrechnungsmodelle, die Check-Points, die Befundlisten je Phase, Risikoschwerpunkte, Besucherstrom, Grafik 5 und 6. Konkretisiert E-16. | 1789 |
| E-34 | Die Phasen sind ein Gerüst zur Orientierung und zur Steuerung. Eine Phase ist ein Zeitabschnitt, keine Leistung, und wird nicht von einem Bereich getragen. Die Spalte Primär-Träger enthält weiche Deskriptoren: Sie sagt, welche Bereiche eine Phase prägen, und ist keine RACI-Zuordnung — aus ihr folgt weder Accountability noch Responsibility. | 1789 |
| E-35 | Vier Zeitfenster weichen bewusst von der Übersichtstabelle in V1.0 ab und sind in der Datei vermerkt: P3 beginnt bei T0 −2 Monate statt −1 Monat, damit P2 und P3 aneinander anschließen. P5 ist mit `T0 bis letzter Laufzeittag` bemessen, mit der typischen Laufzeit von 2 bis 3 Tagen, maximal 5, als Richtwert. P6 hängt am Ende der Laufzeit, nicht an T0 — die Tabellenlesart hätte den Abbau in die Laufzeit gelegt. Bei P7 ist ergänzt, dass die Phase bei größeren Veranstaltungen auch Monate dauert. | 1789 |
| E-36 | Das Gate P1 → P2 ist als prüfbarer Zustand formuliert: „Briefing für die operativen Bereiche ist von den Leads abgenommen." V1.0 nennt an der Stelle eine Tätigkeit, anders als die übrigen sieben Gates. Der V1.0-Wortlaut steht in der Datei daneben. | 1789 |
| E-37 | Das Gate P6 → P7 bleibt in der Tabelle stehen, obwohl V1.0 für Eigenveranstaltungen ausdrücklich kein formales Gate verlangt. Die Bedingung für den Gastfall wird wörtlich übernommen, die Leerstelle für Eigen als offen markiert. Weder gestrichen noch gefüllt: Streichen bräche die V1.0-Aussage „an jedem Phasenübergang ein Gate", Füllen wäre eine plausible Vervollständigung. | 1789 |

### 2026-08-23 · Migration `modul.md`

| ID | Entscheidung | durch |
|---|---|---|
| E-38 | `modul.md` ist übertragen (Modul-Framework V0.2): Definition und glossarfähige Langfassung, der Schnitt nach Ergebnis und Verantwortung, die fünf Bedingungen, die Liste dessen, was kein Modul ist, die drei Abgrenzungen, die zwei Einordnungen Modulart und Bindung, Modul/Variante/Parameter mit dem Werkstatt-Test, Übergaben, der Feldkatalog in fünf Blöcken, die abgeleitete Außensicht mit den Kopplungsregeln, Lebenszyklus mit Statuskette, Definition of Done und Reifegraden. Nicht übernommen: die dreizehn Bedarfe als Herleitung (bleiben in der Quelldatei), der Rechtsrahmen mit Paragraphen und Fristen (geht ins Security-Detailkonzept), die Formalschreibweise für einen späteren Konfigurator, Literatur und Benchmark-Begründungen, das Wort „Grundgerüst". Setzt E-27 um: die Risikostufe ist ein Feld mit `niedrig \| mittel \| hoch` und löst bei `hoch` eine Pre-mortem-Pflicht aus. | 1789 |
| E-39 | Die Verantwortung für ein Modul wird in zwei Felder geteilt. **Durchführung** ist eine Rolle mit benannter Vertretung und verantwortet die Erbringung bei der Veranstaltung. **Fortschreibung** ist eine namentlich genannte Person und verantwortet das Modul über die Zeit. Die namentliche Nennung weicht bewusst vom Grundsatz des Frameworks ab, dass im Playbook nur Rollen vorkommen: Eine Rolle, die niemand konkret besetzt, pflegt nichts. Ohne Durchführungsverantwortung entsteht kein Modul, ohne Fortschreibungsverantwortung wird kein Steckbrief freigegeben. | 1789 |
| E-40 | „Freigabe" bedeutete im Steckbrief drei verschiedene Dinge und ist entzerrt: **Zustimmung** (wer inhaltlich einverstanden sein muss, darf mehr als eine Stelle nennen), **Startbedingung** und **Abbruchkriterien** (darf der Einsatz beginnen, wann wird er abgebrochen), **Dokumentfreigabe** (wer diesen Steckbrief in dieser Version freigegeben hat). Das Wort „Freigabe" kommt danach genau einmal vor. | 1789 |
| E-41 | Die Wahlpflicht wird nicht als eigene Katalogeinheit zwischen den Modulen geführt, sondern über ein Grundmodul. Das Feld Bindung hat vier Werte: `gilt immer`, `gilt auf Bedarf, wenn …`, `Wahlpflicht — Grundmodul`, `Wahlpflicht — Alternative zu …`. Das Grundmodul trägt Entscheider, Entscheidungsfrist und die Liste der Alternativen; die Alternative trägt nur den Rückverweis. Damit stehen Entscheider und Frist genau einmal und laufen nicht auseinander, und es entsteht kein neuer Dingtyp in der Ablage. | 1789 |
| E-42 | Grundmodul ist die einfachste Variante, die mit dem geringsten Ressourceneinsatz auskommt. Grenze: Es darf nicht unter eine Pflichtschwelle fallen. Wo Recht oder Risikoeinstufung eine Mindestausprägung verlangen, gilt diese und nicht die Vorbelegung. Sonst führt eine nicht getroffene Entscheidung zur schwächeren Ausprägung — bei sicherheitsrelevanten Modulen der gefährlichere Fall. | 1789 |
| E-43 | Ein Feld für die Umkehrbarkeit von Entscheidungen entsteht nicht. Stattdessen trägt die **Entscheidungsfrist** die praktische Folge — bis wann entschieden sein muss, verbindlich gemeint — und das Feld **Zustimmung** die von V1.0 verlangte Doppelfreigabe. Die Aussage aus V1.0, solche Entscheidungen seien „grundsätzlich nicht reversibel", ist damit bewusst verkürzt und steht als solche in `offene-punkte.md`. | 1789 |
| E-44 | Das Kriterium „ein Ergebnis" ist neu formuliert: Auf die Frage „Was liegt am Ende vor?" gibt es eine Antwort, nicht zwei. Die Prüfhilfe des Frameworks („ein Satz ohne und") wandert in die Ausfüllhinweise der Steckbrief-Vorlage — sie ist eine Mechanik, keine Aussage. | 1789 |
| E-45 | Das Feld **Ressourcenbedarf** wird aufgenommen und ist Pflicht: internes Personal und Budget je Phase. Im Framework war es nur ein Kandidat. | 1789 |
| E-46 | Es werden keine Beispiele ins Repository übernommen, solange keine echten aus dem Haus vorliegen. Alle Modulbeispiele des Frameworks sind ausdrücklich hypothetisch und stammen aus der Recherche. Folge: Die Ausfüllhinweise der Steckbrief-Vorlage müssen die Erklärlast allein tragen. | 1789 |
| E-47 | Struktur des Risikoregisters und Berichtsformat werden nicht übernommen. Das Framework rechnet an der Stelle mit beidem; die Risikofelder im Steckbrief genügen. Ergänzt E-27. | 1789 |
| E-48 | Die dritte Modulart für Befähigungsleistungen wird jetzt nicht entschieden, sondern mit der Messe geklärt — zusammen mit der Frage, ob Übungs- und Trainingsformate Module sind oder in die Linie gehören. Ohne echte Kandidaten aus dem Haus ist die Frage nicht beantwortbar, und die Modulart steuert, welche Felder Pflicht sind. Bis dahin gelten zwei Arten: Compliance und Leistung. | 1789 |
| E-49 | Dies ist das Grundkonzept und gilt für alle Bereiche. Ein Bereichs-Detailkonzept darf Felder ergänzen, aber keine umbenennen, weglassen oder anders bedeuten lassen. Das Feld gehört ins Grundkonzept, der bereichsspezifische Inhalt ins Detailkonzept. Wendet F-03 auf den Feldkatalog an. | 1789 |
