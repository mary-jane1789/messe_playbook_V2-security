---
status: laufend
stand: 2026-08-19
zweck: Einstieg für die nächste Sitzung — Inhalte aus Playbook V1.0 ins Repository übertragen
---

# Übergabe: Migration der V1.0-Inhalte

## Wo du bist

Das Repository-Skelett steht und ist committet (`5879335`, noch nicht gepusht).
Inhaltlich ist es leer. Was aus dem Playbook V1.0 und dem Modul-Framework
übernommen wird, ist je Kapitel entschieden und in `0_meta/entscheidungen.md`
unter E-14 bis E-28 festgehalten.

**Zuerst lesen:** `CLAUDE.md`, `0_meta/konventionen.md`,
`0_meta/entscheidungen.md`, `0_meta/offene-punkte.md`, und die `README.md` der
Ebene, in der du arbeitest. Sie erklären den Aufbau; dieses Dokument wiederholt
das nicht.

**Quellen liegen im Repo:** `0_meta/quellen/operations-playbook-v1.0.pdf`
(48 Seiten, verabschiedet 07.07.2026) und
`0_meta/quellen/modul-framework-v0.2.md` (nicht freigegeben, 18.08.2026).
Das Sparring-Deck „Was ist ein Modul?" und das Schwesterdokument
`modul-vorgehen` liegen nicht vor.

## Arbeitsweise — nicht verhandelbar

**Prüfen, vorlegen, besprechen, migrieren.** Keine Datei wird ohne Freigabe
geschrieben. Der Weg je Zieldatei: Kapitel lesen, Verdichtung vorschlagen,
Rückfragen klären, dann schreiben.

**Vorlegen heißt kurz.** Je Zieldatei ein knapper Vorschlag: was hineinkommt,
was bewusst wegfällt, wo eine Lücke ist. Keine Langdokumente — die
Projektleitung hat mehrfach klargemacht, dass Volumen das Problem ist, nicht die
Lösung.

**Nichts ergänzen, nichts verlieren.** Wo V1.0 eine Lücke hat, wird sie in
`0_meta/offene-punkte.md` notiert und nicht plausibel gefüllt. Was sich keinem
Ziel zuordnen lässt, geht als Frage zurück.

**Belegstelle Pflicht.** Jede Datei trägt im Frontmatter `quelle:` mit Kapitel.
Kein Satz im Repository ohne Kapitelverweis nach V1.0.

**Verdichtungsmaßstab.** Nicht „was steht im Kapitel", sondern: *Was braucht ein
Modul, um beschreibbar zu sein?* Alles darüber hinaus bleibt im Playbook.

**Ton.** Deutsch, sachlich. Keine Nutzenargumentation in Konzeptdateien — sie
beschreiben, was gilt, nicht warum es gut ist. Im Gespräch direkt, ohne
Zustimmungsfloskeln.

## Zielzuordnung

### 1_grundkonzepte/

| Zieldatei | V1.0 | Was dort steht, worauf zu achten ist |
|---|---|---|
| `veranstaltung.md` | Kap. 1, 4 | Drei unabhängige Achsen: **Art** (Kongress, Corporate Event, Messe B2B, Messe B2C), **Veranstalter** (Eigen, Gast, Partner), **Größe** (klein/mittel/groß mit Schwellen für Aussteller, Besucher, Brutto-qm). Dazu die Unterscheidung Veranstalter gegen Betreiber und die vier Regeln aus Kap. 4 (Veranstalter-Rolle bei Gast, Gewerke-Einordnung, Ticket-System-Isolation, Partner-Hoheit). Die Größenschwellen sind laut V1.0 teils Annahmen und mit der Messe zu bestätigen. |
| `phasen.md` | Kap. 2 | P0 bis P7 mit Name, Zeitfenster relativ T0 und Primär-Träger. Dazu die acht Gates einschließlich P7 → P0. Ohne Herleitung, ohne die Warum-Absätze. **Phasenzählung prüfen, siehe Befund 1.** |
| `lead-modell.md` | Kap. 6 | Customer Lead, Technical Lead, Operations Lead als drei Verantwortungsdimensionen, nicht drei Personen. Lead Committee. VStättV-Veranstaltungsleitung an Technical Lead geknüpft. Lead-Rollen-Doppelung bei Gastveranstaltungen. Der Operations Lead trägt laut V1.0 heute keine gleichberechtigte Verantwortung — als offener Punkt kennzeichnen, nicht glätten. |
| `rolle.md` | Kap. 6 | **Nur das Schema.** Rollen sind strukturell, Personen situativ; Detailrollen ordnen sich Lead Rollen zu; Reporting-Linie gehört zur Rolle. Keine Rollenliste — konkrete Rollen entstehen in Modulen und Abläufen. `instanzen: keine bisher`. |
| `gremium.md` | Kap. 7 | **Nur das Schema:** Zweck, Mitglieder, Ernennung, Rhythmus, Mandat, Stand. Die drei konkreten Gremien werden **nicht** festgeschrieben — sie sind Entwürfe (E-21). `instanzen: keine bisher`. |
| `dienstleister.md` | Kap. 10 | Drei Tiers, sieben Kategorien, und je Kategorie die Einordnung Pflicht / Wahl-Pflicht / Wahl. Für die Modularbeit zählt vor allem die Einordnung; die Tiers sind mitzunehmen, aber nicht der Kern. Vollständigkeit mit der Messe klären. |
| `modul.md` | Modul-Framework | Der Hauptbrocken. Aufteilen, nicht kopieren: Kap. 1, 2.3, 3.1–3.4, 4, 4.1, 5, 5.1, 5.2, 6, 6.1, 7 (Blöcke 1–5), 7.1, 7.2, 8.1–8.3. **Nicht** hierher: Kap. 2.1 (die Bedarfe B-01 bis B-13) und Kap. 2.2 (Rechtsrahmen — der gehört ins Security-Detailkonzept, siehe unten). Der Feldkatalog braucht feste Spalten: Feld, gilt-wenn, Zone, Pflicht oder optional, Wertebereich. **Drei Korrekturen einbauen, siehe Befunde 5 und 6.** |
| `ablauf.md` | neu | Existiert in keiner Quelle. Selbst schreiben: was einen Ablauf ausmacht — Auslöser, Schritte, beteiligte Rollen, Ergebnis, Rückkopplung. Bewusst knapp; drei Instanzen rechtfertigen kein Framework. |

### 2_detailkonzepte/ablauf/

| Zieldatei | V1.0 | Inhalt |
|---|---|---|
| `konfiguration.md` | Kap. 15 | Eine Veranstaltung als rund 50 Parameter. Parameter-Datensatz: Kategorie (Technologie, Maßnahme, Konzept, Schlüsselperson, Dienstleister, Infrastruktur, Format), Name und Wert, Risikostufe, Delta zur Vorveranstaltung, Pre-mortem-Pflicht. Vier Governance-Schritte: erstellen → Commitment → Aktivierung → Review. Drei Review-Zeitpunkte: vor P0, vor P3, nach P7. Wechsel einer Schlüsselperson wird automatisch Risikostufe hoch. |
| `krisenablauf.md` | Kap. 8, 14 | EP-01 Standardpfad, EP-02 Beschwerdepfad, dazu der Krisenpfad. Übergang Risiko → Krise als Triage-Entscheidung des Notfall- und Krisenmanagers, Grundsatz „im Zweifel höher einstufen". SCU als 24/7-Einheit. TS-01 bis TS-04 mit Zeitfenstern und Pflicht-Information. Reaktionszeiten in V1.0 durchgehend `tbd` — so übernehmen. **Siehe Befund 3 zu EP-03.** |
| `lernschleife.md` | Kap. 16 | Fünf Formate: Einzel-VA-Retro, Phasen-Retro (Light), Portfolio-Retro, Post-mortem (Krise), Pre-mortem (neue Bausteine). Grundsatz: jede Retrospektive erzeugt Output, „keine Änderung" ist zulässig, muss aber dokumentiert werden. Governance-Schleife Konfiguration → Commitment → Aktivierung → Review. Keines der Formate ist etabliert — als offenen Punkt kennzeichnen. |

### 2_detailkonzepte/module/security-module-detailkonzept/

Erst nach `modul.md`. Quelle ist **Modul-Framework Kap. 2.2**, das hierher
wandert und nicht ins Grundkonzept gehört: VStättVO §§ 38, 41, 42, 43 mit
Auslöseschwellen, § 34a GewO, vfdb-Merkblatt 13/01 mit Fristenlogik (Entwurf
T-6 Wochen, Endfassung T-4) und dessen Konzeptstruktur, verkaufbare Leistungen.
Dazu Modullandkarte, Wahlpflichtgruppen, Übergabekarte, Bemessungsregeln.

### 0_meta/

| Zieldatei | V1.0 | Inhalt |
|---|---|---|
| `glossar.md` | Kap. 2 | Gate — Bedingung an einem Phasenübergang, abgegrenzt gegen den Check-Point. Weitere Begriffe kommen dazu, wenn sie beim Übertragen gebraucht werden. |
| `projektkontext.md` | Vorspann | Worum geht es, Verankerung im Unternehmen, Leitprinzipien (fünf), Geltungsbereich mit den drei Abgrenzungen, Versionierung. |

### Als Feld, nicht als Konzept

Die **Risikostufe** wird ein Feld im Modulsteckbrief mit dem Wertebereich
`niedrig | mittel | hoch` und der Regel, dass „hoch" eine Pre-mortem-Pflicht
auslöst (E-27). Die Werte und die Regel stammen aus Kap. 13 und 15. Die sieben
Risikokategorien werden **nicht** übernommen.

## Befunde aus V1.0, die beim Übertragen greifen

**1 · Phasenzählung ist dreifach inkonsistent.** Dominant und tragend ist
**P0–P7** (Übersichtstabelle Kap. 2, Grafik 5, Grafik 8, Gate-Tabelle, und
Kap. 4: „Die Phasenstruktur P0 bis P7 gilt für alle Veranstalter-Modelle").
Abweichend: „durchgehender Neu-Nummerierung P0 bis P6" im Abschnitt
Versionierung, „acht Phasen, benannt P0 bis P6" im Einleitungssatz von Kap. 2,
und „nach P8" in Grafik 11. Das Modul-Framework rechnet durchgehend mit P0–P8.
→ **P0–P7 setzen.** Zwei Folgen im Framework: Das Phasenprofil-Beispiel in
Block 2 ist ab P4 um eins verschoben, und „Hard Cut vor P4 (SR-02)" in Kap. 4.1
bezeichnet die falsche Phase — V1.0 hat den Punkt als
„Vollständigkeitscheck vor P3, Gate P2 → P3" entschieden.

**2 · „Modul" ist in V1.0 dreifach belegt.** Als Playbook-Kapitel (die drei
Welle-2-Module Kommunikation und Kollaboration, KPI, Tailoring und Skalierung),
als Leistungsbaustein (Kap. 1, Add-ons), und in Kap. 15 als das, was eine
Konfiguration füllt. Beim Zitieren aufpassen. Im Repository gilt: `M-` für
Playbook-Bausteine (gesperrt), `MOD-` für Leistungsbausteine.

**3 · `EP-03` wird referenziert, aber nie definiert.** Kap. 12 verlangt in jedem
SLA einen „Eskalationspfad (verweist auf EP-01, EP-02 oder EP-03)". Definiert
sind nur EP-01 und EP-02; der Krisenpfad in Kap. 14 trägt keine ID.
→ Vorschlag: Krisenpfad wird EP-03. Betrifft `krisenablauf.md`.

**4 · Anhang A ist nach laufender Nummer nicht zitierfähig.** Die Zählung
springt: 1–13, 18–21, 22–26, 27–29, 30–31, 33–35. Die Positionen 14–17 und 32
fehlen, die Überschriften-Zählungen stimmen jeweils. Beim Übertragen offener
Punkte den Wortlaut mitnehmen, nicht die Nummer.

**5 · „Freigabe" bedeutet im Steckbrief drei verschiedene Dinge.**
Framework Kap. 4 „Freigabeinstanz" (wer verantwortet inhaltlich), Block 3
„Freigabe / Quality Gate" (darf der Einsatz starten), Block 5 „freigegeben durch"
(Dokumentfreigabe). Beim Bau des Feldkatalogs entzerren — Vorschlag: Block 3
heißt `start-gate-und-abbruchkriterien`.

**6 · Ein Feld fehlt: `reversibilität`.** V1.0 Kap. 9 setzt für
sicherheitskritische Entscheidungen zwei Dinge, die im Steckbrief keinen Platz
haben: Freigabe durch BL SOD **plus** die relevante fachliche Einheit, und
„grundsätzlich nicht reversibel". Ohne das Feld beschreibt der Steckbrief eine
Entscheidung als rücknehmbar, die es laut Playbook nicht ist.

**7 · Security ist in V1.0 keine eigene Einheit.** Durchgängig „Logistics &
Security" unter einem AL, zuständig für Ladehof, Slot-Management, Anfahrt und
Parkraum **und** für Postenplan, Schichten, Kontrollumfang. Der Ordner heißt
trotzdem Security, weil das der beauftragte Modulbereich ist; Owner ist
`AL Logistik + Security`, und die Ladehof-Themen liegen an einer
bereichsinternen Grenze.

**8 · Widerspruch bei der Security-Bestellung.** Kap. 2, P2, Strang B sagt
zweierlei: „Logistics & Security … übergeben [den Umsetzungsvorschlag] an Expo
Realisation (Check-Point CP-2d). Die eigentliche Bestellung löst Expo
Realisation aus." Und: „Customer Success … handhabt die Security-Bestellung."
CP-2d in Kap. 3 stützt die erste Lesart. Das ist eine Fachfrage, blockierend
für die Übergabekarte im Security-Detailkonzept.

**9 · Grafik 6 ist ein brauchbares Prüfraster.** Das leere Service-Blueprint-
Template — acht Phasen als Spalten, acht Einheiten als Zeilen (Kunde, Customer
Success, Expo Realisation, Operations Management, Logistics & Security,
ServicePartner, Andere, Systeme). Die Methode selbst wird nicht übernommen
(E-19), das Raster taugt aber für den Vollständigkeitstest der Modullandkarte:
Security-Kandidaten in die Zeile Logistics & Security über die Phasenachse
eintragen, leere Zellen sind Lücke oder begründete Nichtzuständigkeit.

**10 · E-Nummern im Framework haben Lücken.** Kap. 9 führt E-02 bis E-13,
E-01, E-06 und E-08 fehlen. Deshalb beginnt die E-Reihe im Entscheidungslog bei
E-14. Bei der Migration des Frameworks werden dessen E-Nummern unverändert
übernommen.

## Was nicht übernommen wird

Bleibt im Playbook V1.0 gültig, wird hier nur nicht gebraucht: **Check-Points**
(dieselbe Art Ding wie Modul-Übergaben, E-18), **Entscheidungstypen** (E-23),
**Risikomanagement als eigenes Konzept** (E-27), **Abrechnungsmodelle** (E-25),
**SLAs** (E-26), **methodische Empfehlung zum Service Blueprint** (E-19). Die
einleitenden Kapitel gehen in den Projektkontext (E-14).

Wer beim Übertragen versucht ist, eines davon doch hereinzuholen: Der Maßstab
ist der Gegentest. Nimm es weg — lässt sich ein Modul dann noch schreiben?

## Reihenfolge

1. **`veranstaltung.md` und `phasen.md`.** Belastbar beschrieben, keine offenen
   Punkte, und alles Weitere verweist darauf. Guter Einstieg, weil man am
   Ergebnis sieht, ob Verdichtungsmaßstab und Frontmatter tragen.
2. **`modul.md`.** Der Hauptbrocken und der Engpass für alles in Ebene 2 und 3.
   Das Aufteilen des Frameworks ist gleichzeitig sein Test: Felder, die sich
   nicht attributieren lassen, sind unklar formuliert.
3. **`dienstleister.md`**, mit der Vollständigkeitsfrage an die Messe.
4. **`rolle.md`, `gremium.md`, `lead-modell.md`.** Schemata, kurz, mit offenen
   Punkten statt geglätteter Entwürfe.
5. **`ablauf.md`**, dann die drei Abläufe.
6. **`glossar.md`, `projektkontext.md`** laufend mitziehen.
7. Erst danach das Security-Detailkonzept.

## Was am Ende des Tages passiert

Das Entscheidungslog wird **gebündelt am Ende eines Arbeitstages** geschrieben,
nicht laufend. Zwei Reihen: `F-` für Format und Repository mit Begründung,
`E-` für Inhalte mit der Spalte `durch`. Revisionen werden angehängt, der alte
Eintrag bleibt stehen.

Diese Datei liegt in `4_workspace/` und wird gelöscht, wenn die Migration durch
ist — nicht als zweite Fassung liegengelassen.
