---
status: laufend
stand: 2026-08-31
zweck: Einstieg für die nächste Sitzung — Inhalte aus Playbook V1.0 ins Repository übertragen
---

# Übergabe: Migration der V1.0-Inhalte

> **Achtung, Teilstand.** Dieses Dokument beschreibt die Migration mit Stand
> 26.08.2026. Seither hat der erste echte Durchgang durch die Steckbrief-Vorlage
> den Feldkatalog verändert — Feld `Ergebnis` und Feld `Auslöser` sind
> gestrichen, `Geltungsbereich` und `Fristen` sind neu, `Phasenprofil` heißt
> `Deadlines`, `Bindung` heißt `Pflichtstufe`, das Feld
> „Verhalten im eskalierten Betriebszustand" heißt „Verhalten je
> Eskalationsstufe", und es gibt drei Verantwortungen statt zwei (R · A · F).
> **Maßgeblich sind `1_grundkonzepte/modul.md` und
> `0_meta/entscheidungen.md` ab E-63.** Wo dieses Dokument alte Feldnamen
> benutzt, gelten die neuen.
>
> Neu entstanden sind außerdem die Modullandkarte und das erste befüllte Modul
> in `3_instanzen/module/security-module-instanzen/`. Der Rücklauf, der zu den
> Änderungen geführt hat, steht in `rueckfluss-sparrings-2026-08-24.md`.

> **Teilweise überholt seit dem 29.08.2026.** Die Sparrings vom 24.08.2026 haben
> Befund 8 (Bestellweg) beantwortet und die Annahme in E-55 widerlegt; dazu sind
> Felder des Katalogs gestrichen, umbenannt und ergänzt worden. Was gilt, steht
> in `0_meta/entscheidungen.md` ab E-63 und in
> `4_workspace/rueckfluss-sparrings-2026-08-24.md`. Dieses Dokument bleibt für
> die noch offenen Migrationsschritte gültig — `dienstleister.md`, `rolle.md`,
> `gremium.md`, `lead-modell.md`, `ablauf.md` und die drei Abläufe.

## Wo du bist

Das Repository-Skelett steht und ist committet. Übertragen sind
`veranstaltung.md`, `phasen.md` und `modul.md`; dazu ist das Security-Detail-
konzept vorgezogen entstanden (siehe unten). Was aus dem Playbook V1.0 und dem Modul-Framework
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

~~Erst nach `modul.md`.~~ **Vorgezogen und am 26.08.2026 angelegt** — siehe
„Abweichung von der Reihenfolge" unten. Es besteht aus drei Dateien statt der
fünf des Platzhalters (F-26): `security-modul.md` mit den vier Zusatzangaben,
den Ausfüllhinweisen und den Schnittregeln, dazu `rechtsrahmen.md` und
`bemessungsverfahren.md` mit Struktur, aber ohne Zeilen (E-60).

Modul-Framework Kap. 2.2 ist damit verteilt: die Benennungsregel nach vfdb und
die Außensicht stehen in `security-modul.md`, Normen, Schwellen und Fristen in
`rechtsrahmen.md`. Die Normzeilen selbst sind noch nicht eingetragen.

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

**1 · Phasenzählung — an der Quelle nachgeprüft, erledigt am 23.08.2026.**
P0–P7 steht an 13 Stellen, davon vier tragend: Grafik 5 (S. 10, acht Kästen),
Übersichtstabelle (S. 10–11), Gate-Tabelle (S. 11, acht Übergänge), acht
Phasensektionen (S. 12–22). Dazu Kap. 4 (S. 24), Kap. 5 (S. 25), Grafik 8
(S. 30), Kap. 7 (S. 28), Kap. 13 (S. 38), Kap. 15 (S. 43–44), Überschrift und
Inhaltsverzeichnis.

Abweichend nur drei Stellen, und es sind keine konkurrierenden Systeme:

- S. 9 „acht Phasen, benannt **P0 bis P6**" — in sich widersprüchlich, P0 bis P6
  sind sieben. Zahlendreher im Satz, der die Zusammenlegung beschreibt.
- S. 4 „durchgehender Neu-Nummerierung **P0 bis P6**" — derselbe Dreher an
  derselben Aussage. Beide Vorkommen hängen an der Zusammenlegung, nirgends sonst.
- S. 46 Grafik 11, „nach **P8**" — Vor-Merge-Label. Vor der Zusammenlegung gab es
  neun Phasen P0–P8, Nachbereitung war P8. Gemeint ist P7.

→ **P0–P7 ist gesetzt, V1.0 ist Source of Truth.** Das Modul-Framework v0.2
rechnet mit der Vor-Merge-Zählung P0–P8 und wird umgerechnet.

**Umrechnungsregel: P0, P1, P2 bleiben. P3 bis P8 minus eins.** Alte P2
(Verkaufszeitraum Services) und alte P3 (Feinplanung) gehen in die neue P2 auf;
3−1 = 2 trifft das, deshalb genügt eine Regel. Frühere Fassung dieses Befunds
sagte „ab P4 um eins verschoben" — es ist ab P3.

Neun Stellen im Framework sind betroffen:

| Zeile | jetzt | wird |
|---|---|---|
| 16, 103, 205, 211 | `P0–P8` | `P0–P7` |
| 35 | „Übergabe SOD → Expo Realisation … Status-quo P3" | `P2` — deckt sich mit CP-2d in P2 |
| 154 | „den bislang fehlenden Hard Cut vor P4 (SR-02)" | `vor P3`, **und** inhaltlich: V1.0 hat SR-02 als Vollständigkeitscheck ohne harten Cut-off entschieden, Gate P2 → P3 |
| 257 | „P0 · P3 Konzept und Postenplan · P5–P7 Kontrollbetrieb · P8 Auswertung" | `P0 · P2 · P4–P6 · P7` |
| 281 | „P3: 4 PT Planung; P5–P7: durchgehende Präsenz" | `P2` … `P4–P6` |
| 283 | „Peak in P4/P5" | `P3/P4` |

Die Quelldatei in `0_meta/quellen/` bleibt als Beleg unangetastet; die Korrektur
greift beim Schreiben von `modul.md`.

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

**5 · „Freigabe" bedeutete im Steckbrief drei verschiedene Dinge — gelöst am
23.08.2026.** Framework Kap. 4 „Freigabeinstanz" (wer verantwortet inhaltlich),
Block 3 „Freigabe / Quality Gate" (darf der Einsatz starten), Block 5
„freigegeben durch" (Dokumentfreigabe). In `modul.md` heißen die drei jetzt
**Zustimmung**, **Startbedingung** und **Abbruchkriterien**, und
**Dokumentfreigabe**. Das Wort „Freigabe" kommt genau einmal vor.

**6 · Reversibilität — anders gelöst als vorgeschlagen, 23.08.2026.** V1.0
Kap. 9 setzt für sicherheitskritische Entscheidungen zwei Dinge: Freigabe durch
BL SOD **plus** die relevante fachliche Einheit, und „grundsätzlich nicht
reversibel". Ein Feld `reversibilität` ist **nicht** entstanden. Stattdessen:
die **Entscheidungsfrist** im Wahlpflicht-Grundmodul trägt die praktische Folge
(bis wann muss entschieden sein, und diese Frist ist verbindlich gemeint), das
Feld **Zustimmung** trägt die Doppelfreigabe, weil es mehr als eine Stelle
nennen darf. Die V1.0-Aussage zur Nichtumkehrbarkeit steht als bewusste
Verkürzung in `0_meta/offene-punkte.md`.

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

1. ~~**`veranstaltung.md`**~~ — erledigt am 19.08.2026, liegt in
   `1_grundkonzepte/veranstaltung.md` (E-29, E-30). Offene Punkte daraus stehen
   in `0_meta/offene-punkte.md`, die Wording-Frage in
   `4_workspace/fragen-an-ma.md`.
   ~~**`phasen.md`**~~ — erledigt am 23.08.2026, liegt in
   `1_grundkonzepte/phasen.md`. P0–P7 mit Zeitfenster und Primär-Träger, die acht
   Gates, dazu der Abschnitt „Wozu das Phasenmodell". Befund 1 ist an der Quelle
   nachgeprüft und oben ersetzt. Vier Abweichungen von V1.0 sind entschieden und
   in der Datei vermerkt: Bezugspunkt P6, Endpunkt P5, Beginn P3 bei T0 −2
   Monate, Gate P1 → P2 als prüfbarer Zustand. Primär-Träger sind als weiche
   Deskriptoren ohne RACI-Wirkung festgelegt.
2. ~~**`modul.md`**~~ — erledigt am 23.08.2026, liegt in
   `1_grundkonzepte/modul.md`. Feldkatalog in fünf Blöcken mit den fünf Spalten,
   Definition, fünf Bedingungen, zwei Einordnungen, Außensicht, Lebenszyklus.
   Sechs Abweichungen vom Framework sind entschieden und in der Datei als
   Setzung erkennbar: das Ergebniskriterium neu formuliert; Owner aufgeteilt in
   Durchführung (Rolle) und Fortschreibung (Name); „Freigabe" entzerrt in
   Zustimmung, Startbedingung und Dokumentfreigabe; Bindung mit vier Werten und
   Grundmodul-Regel statt separater Wahlpflicht-Gruppe; Entscheidungsfrist statt
   Reversibilität; Ressourcenbedarf aufgenommen. Keine Beispiele übernommen.
   Risikoregister-Struktur und Berichtsformat fallen weg.
3. **`dienstleister.md`**, mit der Vollständigkeitsfrage an die Messe.
4. **`rolle.md`, `gremium.md`, `lead-modell.md`.** Schemata, kurz, mit offenen
   Punkten statt geglätteter Entwürfe.
5. **`ablauf.md`**, dann die drei Abläufe. Der **Krisenablauf** ist inzwischen
   vorrangig: Das Security-Detailkonzept braucht die Betriebszustände (E-52).
6. **`glossar.md`, `projektkontext.md`** laufend mitziehen.
7. ~~Erst danach das Security-Detailkonzept.~~ — **vorgezogen, erledigt am
   26.08.2026** (E-50 bis E-62).

## Abweichung von der Reihenfolge

Das Security-Detailkonzept ist vor den Punkten 3 bis 6 entstanden, weil ein
Termin mit Bereichsleitung und Leitung Security anstand und dafür ein
befüllbares Format gebraucht wurde.

Was das kostet, offen benannt: Das Detailkonzept verweist an drei Stellen ins
Leere.

- Das Feld **Verhalten im eskalierten Betriebszustand** braucht Betriebszustände,
  die im Krisenablauf zu setzen sind. Der ist nicht geschrieben.
- **Rollenbezeichnungen** in Übergaben und Zuständigkeiten sind provisorisch,
  solange `rolle.md` fehlt.
- Der Hinweis, dass das Modul nur die Anforderung liefert und die Linie
  beschafft, hängt an `dienstleister.md`.

Diese Verweise sind als hängend gekennzeichnet und nicht plausibel gefüllt. Beim
Schreiben der fehlenden Dateien ist gegen das Detailkonzept abzugleichen.

## Was am Ende des Tages passiert

Das Entscheidungslog wird **gebündelt am Ende eines Arbeitstages** geschrieben,
nicht laufend. Zwei Reihen: `F-` für Format und Repository mit Begründung,
`E-` für Inhalte mit der Spalte `durch`. Revisionen werden angehängt, der alte
Eintrag bleibt stehen.

Diese Datei liegt in `4_workspace/` und wird gelöscht, wenn die Migration durch
ist — nicht als zweite Fassung liegengelassen.
