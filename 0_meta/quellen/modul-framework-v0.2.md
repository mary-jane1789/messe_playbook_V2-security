# Modul-Framework

**Was ein Modul ist** — Definition, Typisierung, Anatomie
**Status:** V0.2, konsolidiert, nicht freigegeben · **Stand:** 2026-08-18
**Bezug:** Kalkulation Tranche 2, AP 2.1 · **Pilotbereich:** Security · **Anspruch:** Blueprint für alle späteren Bereichsmodule
**Schwesterdokument:** `modul-vorgehen` (Schnittregeln, Workshops, Kick-Off-Vermittlung, Sparring-Prüffragen)

> Alle Modulbeispiele in diesem Dokument sind als `[hypothetisch]` gekennzeichnet. Sie stammen aus der Recherche, nicht aus dem Haus, und werden nach dem Vorbefüllungstermin mit dem Leiter Security durch echte Module ersetzt.

---

## 1 · Kernaussage

**Module werden nicht entlang der Phasen und nicht entlang der Aufbauorganisation geschnitten.**

Beides ist der naheliegende Weg — das Phasenmodell P0–P8 liegt fertig da, die Teams sind gesetzt — und beides erzeugt Module, die niemand allein verantworten kann. Wer entlang des Prozessflusses zerlegt, produziert Bausteine, die nur in Reihe funktionieren. Wer entlang der Teams zerlegt, zementiert die Silos, die das TOM gerade auflösen soll.

Der empirische Beleg liegt im Haus: Ein Sicherheitsmodul beginnt in der strategischen Konzeption, wird in der Feinplanung bestellt, in der Laufzeit erbracht und in der Nachbereitung ausgewertet. Es liegt **quer** zu den Phasen. Das ist keine Ausnahme, sondern der Normalfall — und damit das Argument gegen den Phasenschnitt.

---

## 2 · Warum das Framework so aussehen muss

### 2.1 Bedarfe aus dem Projekt

| # | Bedarf | Quelle | Konsequenz |
|---|---|---|---|
| B-01 | **Vertretungsfähigkeit** — Abläufe funktionieren, „weil Horst das seit 20 Jahren so macht" | SR-05 | Übergabetest als Abnahmekriterium: Eine Vertretung muss ohne Rückfrage arbeiten können |
| B-02 | **Gemeinsame Sprache** — „Was bedeutet fertig?" ist unbeantwortet | IST-Beschreibung | Definition of Done je Modul, nicht je Person |
| B-03 | **Keine Kennzahlen** — „Wir hatten null KPIs, wo wir das dann festmachen" | SR-01 | Selbstprüfungskennzahl als Feld des Moduls — nicht als Controlling-Instrument (siehe 2.3) |
| B-04 | **Krisenmanagement ohne Klassifikation und Meldelogik** | SR-03 | Meldeweg, Eskalation, Kritikalität sind Pflichtfelder bei Compliance-Modulen |
| B-05 | **Neue Bausteine ohne Pre-/Post-mortem** (Security-Check im Flughafenmodus bei Enforce Tec) | SR-06 | Änderung am Modul löst Risikoprüfung aus; Änderungslogik ist Teil des Moduls |
| B-06 | **Keine strukturierte Retrospektive** | SR-08 | Rückkopplungspunkt je Modul: wohin fließt die Erkenntnis |
| B-07 | **Kein Verzugsmonitoring** | SR-09 | In-Process-Messung statt Ergebniszahlen |
| B-08 | **Übergabe SOD → Expo Realisation** bei Security-Planung; Logistik bleibt in SOD | Status-quo P3 | Übergaben werden explizit modelliert — die Bruchstelle liegt *innerhalb* des Bereichs |
| B-09 | **Duale Adressierung** — außen Schaufenster, innen Werkstatt | AP 2.1 | Zwei Sichten, **eine** Datenquelle |
| B-10 | **Das Fach befüllt selbst**, 1789 liefert Template und Moderation | AP 2.4 | Ohne Beratungsbegleitung befüllbar: gestaffelte Felder, Ausfüllhinweise, Beispielmodul |
| B-11 | **Abgrenzung zum CPFP** | Projektsteckbrief | Module beschreiben Vorgehen je Veranstaltung, nicht Prozesse der Organisation |
| B-12 | **Skalierbarkeit** über Portfolio und weitere Bereiche | AP 2.1 | Ein gemeinsames Andock-Interface für alle Bereiche, kein bereichsspezifisches Sonderformat |
| B-13 | **Kein SPOC, direkte Drähte** unterlaufen definierte Wege | SR-03, SR-07 | Übergabemedium ist Pflichtfeld — sonst passiert die Übergabe über den kürzesten Weg |

### 2.2 Bedarfe von außen (nicht verhandelbar)

Der Pilotbereich ist der am stärksten fremdbestimmte Bereich des Hauses. Das Framework nimmt diese Vorgaben auf, statt eine eigene Ordnung darüberzulegen.

- **Rechtsrahmen VStättVO:** Sicherheitskonzept und Ordnungsdienst ab 5.000 Besucherplätzen im Einvernehmen mit den Behörden (§ 43), Brandschutzordnung und jährliche Unterweisung (§ 42), Brandsicherheitswache ab definierten Schwellen (§ 41), ständige Anwesenheit und Pflicht zur Betriebseinstellung (§ 38). → Es gibt Module, deren Existenz und Mindestinhalt nicht unterschreitbar sind.
- **Behördliche Anschlussfähigkeit:** Das vfdb-Merkblatt 13/01 definiert faktisch bereits eine Modulstruktur (Ordnungsdienst-, Sanitätsdienst-, Räumungs-, Verkehrs-, Kommunikationskonzept) mit Fristenlogik: Entwurf 6 Wochen, Endfassung 4 Wochen vor Beginn. → **Wo die Benennung deckungsgleich ist, wird die behördlich etablierte übernommen.** Eine eigene Nomenklatur erzeugt Reibung im Genehmigungsverfahren.
- **Verkaufbare Leistung:** Bewachung, Standwache, Sanitätsdienst, Slotbuchung sind an Aussteller verkaufte Leistungen mit Preis, Verrechnungseinheit, Bestellfrist, Spätbestellzuschlag und Stornoregel. → Die Außensicht ist nicht Marketingbeiwerk, sondern vertragsrelevant.

### 2.3 Drei Abgrenzungen

Was ein Modul ist, klärt sich zur Hälfte daran, was es *nicht* ist. Diese drei Sätze sind zugleich das Rückgrat der Kick-Off-Argumentation:

1. **Modul ≠ Prozess.** Ein Prozess **folgt dem Fluss** — über Bereichsgrenzen hinweg. Ein Modul **folgt der Verantwortung** und endet dort, wo eine andere beginnt; der Prozess läuft weiter. Beides ist orthogonal, nicht konkurrierend: ein Prozess kreuzt viele Module, ein Modul kommt in vielen Prozessen vor. Das CPFP kartiert die Prozesse (Makro), das Playbook die Module (Mikro).
   *Praktische Folge für das Befüllen:* Was andere Verantwortliche tun, steht nicht als Ablaufschritt, sondern als **Übergabe**. Der Ablauf ist ein Feld des Moduls — nicht sein Gegenstück zum Prozess. Zusätzlich gilt: keine Verzweigungen im Ablauf (Unterschiede sind Variante oder Parameter), und Steuerungstiefe statt Ausführungstiefe (4–8 Abschnitte, je Abschnitt eine Rolle und ein Ergebnis).
2. **Modul ≠ Dienstleistersteuerung.** Auswahl, Vertrag, SLA und Qualitätssteuerung der ServicePartner liegen in der Linie. Das Modul **liefert die Anforderung**, die Linie beschafft und steuert. Nutzen des Playbooks hier: Anforderungen werden leichter vermittelbar, weil sie erstmals schriftlich und begründet vorliegen.
3. **Modul ≠ Controlling-Objekt.** Kennzahlen im Modul dienen der **Selbstprüfung des ausführenden Teams** (In-Process-Measures). Sie sind kein Instrument der Leistungsbewertung durch die Führung. Ergebnis-/Outcome-Kennzahlen existieren, aber auf Veranstaltungs- und Portfolioebene im Grundgerüst — nicht im Modulsteckbrief.

Die dritte Abgrenzung ist durch die Recherche gestützt, nicht nur eine Setzung: Kennzahlen-Dysfunktion (Ridgway 1956, Goodhart) entsteht überwiegend dort, wo Kennzahlen nach oben berichtet werden. Eine Selbstprüfungskennzahl hat keinen Manipulationsdruck.

**Eine Grenze der dritten Abgrenzung** *(zur Bestätigung im Sparring)*: Bei Compliance-Modulen ist die Abweichung von einer Frist oder einer Behördenauflage nichts, was das Team mit sich selbst klärt. Sie ist **meldepflichtig an eine benannte Rolle** — unabhängig von Kennzahlen. Das ist kein Controlling, sondern Weitergabe von Haftung.

### 2.4 Begriffe (gesetzt)

`Modul` ist im bisherigen Repository doppelt belegt — der Arbeitsplan führt `M-01…M-08` als „M-Module". Gesetzt gilt ab dem neuen Repository:

- **Schema** = abstraktes Förmchen, Präfix `M-` (Glossarbegriff existiert)
- **Modul** = Leistungsbaustein eines Bereichs, Präfix `MOD-<BEREICH>-<NR>`, z. B. `MOD-SEC-04`
- **Grundgerüst** = die geteilte Grundlage, an die alle Module andocken (Kap. 6)

*Vorbehalt:* Die Ordnerlogik des neuen Repositories und der Ablageort dieses Frameworks (Modellschicht, nicht Schema, nicht Instanz) sind mit dem inhaltlich Verantwortlichen durchzugehen. Die Ordnermodelle in Projekt-Instruktion und Konventionsdatei des Altrepositories widersprechen sich.

---

## 3 · Definition

### 3.1 Merksatz

> **Ein Modul ist keine Gliederungsebene des Playbooks, sondern die kleinste eigenständig verantwortbare Leistungseinheit des Bereichs — mit einem Namen, einem Owner, einem definierten Ergebnis, prüfbaren Übergabepunkten und zwei abgeleiteten Sichten: einem Schaufenster nach außen und einer Werkstatt nach innen.**

### 3.2 Langfassung (glossarfähig)

> **Modul** — Eine dauerhaft benannte, eigenständig verantwortbare Leistungseinheit eines operativen Bereichs. Sie erbringt ein definiertes Ergebnis für einen benannten Adressaten, ist über Veranstaltungen hinweg wiederverwendbar, wird über standardisierte Übergabepunkte in die Veranstaltungsdurchführung eingebunden und wird in einer Innensicht (Erbringung) und einer daraus abgeleiteten Außensicht (Leistungsversprechen bzw. Nachweis) beschrieben.

### 3.3 Die fünf Konstitutivkriterien

Ein Kandidat ist erst ein Modul, wenn **alle fünf** erfüllt sind:

| | Kriterium | Prüffrage |
|---|---|---|
| **K1** | **Ein Ergebnis** | Lässt sich das Ergebnis in einem Satz ohne „und" benennen? |
| **K2** | **Ein Owner** | Gibt es genau eine Funktion, die es Ende-zu-Ende verantwortet? |
| **K3** | **Wiederverwendbar** | Kommt es bei mehr als einer Veranstaltung in gleicher Grundgestalt vor? |
| **K4** | **Definierte Übergaben** | Sind Eingang und Ausgang mit Objekt, Übergabemedium, Auslöser und Rolle beschreibbar? |
| **K5** | **Eigener Treiber** | Gibt es einen Grund, *warum* es ein eigener Baustein ist — Rechtspflicht, Varianzträger, Verkaufbarkeit, Personenrisiko, gezielte Weiterentwicklung? |

„Kleinste" im Merksatz ist durch K1 und K2 begrenzt: die kleinste Einheit, die **noch** ein Ergebnis ohne „und" und einen Owner trägt. Nicht kleiner — sonst entstehen Splitter, die einzeln nichts leisten.

### 3.4 Was kein Modul ist

| Kein Modul | Warum | Wohin dann |
|---|---|---|
| **Phase** (P0–P8) | Zeitabschnitt, nicht Leistung. Module wirken *in* Phasen und laufen quer dazu | Grundgerüst |
| **Rolle** (TVK, Ordnungsdienstleiter, Notfallmanager) | Träger, nicht Leistung | Grundgerüst / Rollenmodell |
| **Einzelner Prozessschritt** („Postenplan freigeben") | zu fein; erzwingt synchrone Änderung anderswo | Ablaufabschnitt *innerhalb* eines Moduls |
| **Dokument oder Vorlage** (Risikoregister, Statusbericht) | Lieferobjekt, nicht Leistungseinheit | Lieferobjekte des Moduls |
| **Organisationseinheit** („Team Logistics & Security") | scheitert am Stabilitätstest bei der nächsten Reorganisation | Owner-Feld |
| **End-to-End-Prozess der Organisation** | Zuständigkeit CPFP | Verweis, nicht nachschreiben |
| **Dienstleisterauswahl und -steuerung** | liegt in der Linie | Modul liefert nur die Anforderung |
| **Querschnittsmechanik** (Terminologie, Berichtsformat, Eskalationslogik) | hängt mit fast allen Modulen zusammen | Grundgerüst |
| **Parameterwert** („70 statt 40 Kräfte je Schicht") | ändert nur einen Wert | Parameter des Moduls (Kap. 5) |

---

## 4 · Zwei Achsen: Modulart und Bindung

Ein Modul wird auf zwei unabhängigen Achsen eingeordnet. Die Trennung ist wichtig, weil sonst *was ein Modul ist* mit *ob es für eine Veranstaltung gilt* vermischt wird.

**Achse 1 — Modulart.** Bestimmt, welche Felder Pflicht sind.

| | **A · Compliance** | **B · Leistung** | **C · Enabler** *(offen, siehe E-09)* |
|---|---|---|---|
| Zweck | Rechtliche/normative Pflicht erfüllen, Nachweis erbringen | Leistung für Kunden oder internen Auftraggeber erbringen | Befähigung, ohne die A und B nicht funktionieren |
| Adressat | Behörde, Geschäftsleitung (Haftung) | Aussteller, Gastveranstalter, interner Auftraggeber | eigene Organisation |
| Außensicht | **Nachweissicht** | **Katalogsicht** | Befähigungssicht |
| Zusatzpflichtfelder | Rechtsgrundlage, Auslöseschwelle, Nachweisart, Fristen, Freigabeinstanz | Preis/Verrechnungseinheit, Bestellweg, Vorlauf- und Stornofrist, Mitwirkung, Servicezeiten | Zielgruppe, Turnus, Nachweis |
| Beispiel `[hypothetisch]` | Sicherheitskonzept, Räumungskonzept | Standwache, Slotmanagement | — |

**Achse 2 — Bindung je Veranstaltung.** Bestimmt, ob es gilt.

| | Pflicht | **Wahlpflicht** | Optional |
|---|---|---|---|
| **A Compliance** | Brandschutzorganisation | Einlasskontrolle: Stichprobe **oder** Vollkontrolle — beides zulässig, eines muss gewählt werden | — |
| **B Leistung** | — | Zufahrt: Slot buchen **oder** Sondergenehmigung außerhalb des Zeitfensters | Standwache, VIP-Schutz |
| **C Enabler** | Einweisung vor Einsatz *(rechtlich gefordert — deshalb eher A, siehe E-09)* | — | Übungsformat *(oder Linie? siehe E-10)* |

*Alle Beispiele `[hypothetisch]`.*

**Präzisierung zu Compliance-Modulen:** Nicht „nicht tailorbar", sondern — **die Bindung darf nicht unter die Rechtsschwelle, die Ausprägung darf variieren.** Das ist die Aussage, die im Genehmigungsverfahren trägt.

### 4.1 Wahlpflicht-Gruppe

Wahlpflicht ist eine Beziehung **zwischen** Modulen, keine Eigenschaft eines Moduls. Sie wird deshalb als eigene kleine Katalogeinheit geführt — sonst stehen Entscheider und Frist in jeder Alternative getrennt und laufen auseinander.

| Feld | Beispiel `[hypothetisch]` |
|---|---|
| ID / Name | `WP-02` Kontrolltiefe Einlass |
| Alternativen (Module) | `MOD-SEC-03` Stichprobenkontrolle · `MOD-SEC-04` Vollkontrolle |
| Grundlage der Wahl | Risikoeinstufung der Veranstaltung, Behördenabstimmung |
| **Entscheider** | Leitung Security, im Einvernehmen mit Veranstaltungsleitung |
| **Entscheidungszeitpunkt** | bis T-10 Wochen (vor Erstellung Sicherheitskonzept, T-6) |
| **Vorbelegung, falls nicht entschieden** | Stichprobenkontrolle — Abweichung meldepflichtig |

Die Vorbelegung ist der Punkt, der in der Praxis zählt: Eine Wahl, die niemand trifft, wird stillschweigend zur Vorbelegung — und im Sicherheitsbereich ist die unbewusste Vorbelegung der gefährlichere Fall. Der Entscheidungszeitpunkt macht zugleich den bislang fehlenden Hard Cut vor P4 (SR-02) an einem konkreten Ort verhandelbar.

---

## 5 · Modul, Variante, Parameter

Drei Ebenen, saubere Zuordnung — anschlussfähig an die im Haus bereits gebrauchte Konfigurations-Metapher („jede Veranstaltung ist eine Konfiguration aus rund 50 Parametern"):

1. **Modulkatalog** — welche Bausteine existieren (bereichsweit, stabil).
2. **Modulauswahl je Veranstaltung** — welche gelten (Bindung, Achse 2).
3. **Parametrisierung** — mit welchen Werten der gewählte Baustein läuft.

### 5.1 Der Werkstatt-Test

> Können dieselben Menschen mit **derselben Anleitung** beide Ausprägungen ausführen? → **Variante.**
> Bräuchte eine Vertretung **zwei verschiedene Anleitungen**? → **Zwei Module.**

| Fall `[hypothetisch]` | Einordnung | Begründung |
|---|---|---|
| Stichprobe vs. Vollkontrolle | **zwei Module** | andere Rollen, andere Flächen (Rückstau, Warteschlange), andere Bemessung, andere Nachweise |
| Nachtwache vs. Tagwache | **Variante** | gleiche Anleitung, anderes Zeitfenster |
| Sanitätsdienst mit 6 statt 3 Kräften | **Parameter** | gleiche Rollen, gleiche Abläufe, andere Zahl |

Der Test ist bewusst an den Übergabetest der Definition of Done gekoppelt (B-01): Wer die Vertretungsfähigkeit als Maßstab nimmt, entscheidet Modulgrenzen aus der Praxis heraus und nicht am Reißbrett.

### 5.2 Im Steckbrief steht Klartext

| Im Steckbrief | Bedeutung |
|---|---|
| **Gilt: immer** | ohne Ausnahme aktiv |
| **Gilt: entweder–oder** → Verweis auf Wahlpflicht-Gruppe | eine von mehreren Ausprägungen ist zu wählen |
| **Gilt: auf Bedarf, wenn …** | aktiv bei benanntem Auslöser |
| **Setzt voraus:** … | ein anderes Modul muss ebenfalls aktiv sein |
| **Nicht gemeinsam mit:** … | schließt ein anderes Modul aus |

**Tailoring-Regeln werden als Bedingung formuliert, nicht als Ablauftext:** *„Veranstaltung mit mehr als 5.000 Besucherplätzen ⇒ Sicherheitskonzept gilt immer, Freigabe im Einvernehmen mit der Behörde, Entwurf T-6 Wochen."* So ist die Regel prüfbar und für einen späteren Konfigurator anschlussfähig.

### 5.3 Formalisierung (für Repository und späteren Konfigurator)

Die Klartextfassung entspricht der Grammatik von Feature-Modellen: `mandatory` · `optional` · `alternative (XOR)` · `or` · `requires` · `excludes` · Attribute mit Wertebereich. Diese Notation gehört in die maschinenlesbare Ablage — **nicht in den Steckbrief und nicht in den Workshop.**

---

## 6 · Grundgerüst

Was mit fast allen Modulen zusammenhängt, ist kein Modul, sondern Grundgerüst. Alle Module docken über **dasselbe** Interface daran an — das ist die Voraussetzung dafür, dass der Security-Blueprint auch für die nächsten Bereiche trägt (B-12).

Das Grundgerüst ist nicht homogen. Es enthält Dinge mit unterschiedlicher Änderungslogik, und diese Unterscheidung entscheidet darüber, wie sie gepflegt werden:

| Gruppe | Inhalt | Änderungslogik |
|---|---|---|
| **Setzungen** | Phasenmodell P0–P8, Veranstaltungstypologie und Trägerschaft, Terminologie | Einmal entschieden, dann stabil. Änderung nur per formaler Entscheidung — und wirkt auf alle Module |
| **Governance** | Gremien, Entscheidungs- und Meldewege, Eskalationslogik, Berichtsformat, Risikoregister-Struktur | Lebendig, ändert sich mit der Organisation (Nachfolgen, neue Gremien). Braucht einen Owner |
| **Formvorgaben** | Steckbrief-Format, Namenskonventionen, Definition of Done, Reifegradmodell | Redaktionelle Entscheidung, versioniert |

Die Trennung folgt einem Befund aus der Benchmark-Recherche: Im EASA-Aerodrome-Manual ist das Änderungsverfahren **Teil A des Handbuchs**, nicht Anhang. Wer die Änderungslogik nicht mitschreibt, hat nach zwei Jahren ein Dokument, dem niemand traut.

*Zur Visualisierung (später, Präsentation): Module als waagerechte Balken über der Phasenachse P0–P8, darunter das Grundgerüst als Band aus drei Schichten. Das Bild zeigt in einem Blick, dass Module quer zu den Phasen liegen und alle auf derselben Grundlage stehen.*

### 6.1 Übergaben

Jede Modulgrenze wird mit vier Angaben beschrieben. Übergaben in Dienstleistungen sind soziale Ereignisse, nicht mechanische Passformen — sie brauchen ein benanntes Trägermedium und eine verantwortliche Rolle, sonst passieren sie über den kürzesten Weg: den direkten Draht (SR-03, SR-07).

| Feld | Beispiel — Übergabe Security-Planung → Bestellung (B-08) |
|---|---|
| **Übergabeobjekt** | Umsetzungsvorschlag Postenbesetzung |
| **Übergabemedium** | Bestellgrundlage im Standardformat *(Beispiele: Formular im Bestellsystem · Plan · Protokoll · Besprechung)* |
| **Auslöser** | Abschluss Feinplanung, T-x Wochen |
| **Rollen (gebend → nehmend)** | Security-Planung (SOD) → TVK (Expo Realisation) |

---

## 7 · Der Steckbrief

**Grundprinzip: eine Datenquelle, zwei Sichten.** Die Innensicht ist der führende Datensatz. Die Außensicht ist eine gefilterte, in Nutzen übersetzte Ansicht darauf — kein zweites, parallel gepflegtes Dokument. Kein Nutzenversprechen außen ohne Zusage innen.

**Zwei Ausbaustufen.** Nicht alles auf einmal:

- **● Kurzsteckbrief** (Block 1 + 2) — entsteht im WS 2, davon kann das Team bereits arbeiten.
- **Vollsteckbrief** — wächst beim Befüllen und bei der ersten Anwendung im Alltag.

Zehn gefüllte Felder sind mehr wert als dreißig halbe. **Typabhängig ausblenden:** Ein Leistungs-Modul sieht Block 3 in Kurzform, ein Compliance-Modul sieht keine Preisfelder.

Durchgehendes Beispiel: `MOD-SEC-04 Einlasskontrolle mit Vollkontrolle` `[hypothetisch]`.

### Block 1 · Kern — damit überhaupt jemand handeln kann

| | Feld | Was gemeint ist | Beispiel |
|---|---|---|---|
| ● | **Modul-ID** | eindeutiger Schlüssel | `MOD-SEC-04` |
| ● | **Modulname** | substantivisch, ergebnisorientiert; nie Verb, nie Tool-, nie Abteilungsname | „Einlasskontrolle mit Vollkontrolle" |
| ● | **Modulart** | A Compliance / B Leistung / C Enabler | A |
| ● | **Ergebnis — „Fertig ist, wenn …"** | der eine Satz ohne „und" | „Alle Besucher haben das Gelände über kontrollierte Zugänge betreten, der Kontrollnachweis liegt vor." |
| ● | **Zweck / Schutzziel** | wovor schützt es wen | „Verhindern, dass verbotene Gegenstände auf das Gelände gelangen. Schutzziel: Menschen." |
| ● | **Owner + Vertretung** | eine Funktion, Ende-zu-Ende | „Leitung Security; Vertretung: Notfall- und Krisenmanager" |
| ● | **Auslöser** | woran erkennt man, dass es losgeht | „Entscheidung in Wahlpflicht-Gruppe `WP-02` fällt auf Vollkontrolle" |
| ● | **Ablauf in Abschnitten** | 4–8 Abschnitte, je Auslöser → Tätigkeit → Ergebnis; keine Mikroschritte | „1 Kontrollkonzept erstellen · 2 Postenplan ableiten · 3 Bedarf an Linie übergeben · 4 Einweisung durchführen · 5 Kontrollbetrieb · 6 Protokoll und Debrief" |
| ● | **Lieferobjekte** | was am Ende vorliegt, mit Ablageort | „Kontrollkonzept, Postenplan, Einweisungsnachweis, Kontrollprotokoll" |

### Block 2 · Zusammenspiel — damit es an die Nachbarn anschließt

| | Feld | Was gemeint ist | Beispiel |
|---|---|---|---|
| ● | **Phasenprofil** | eine Zeile je beteiligter Phase: Phase · was passiert · Ergebnis am Phasenende · führende Rolle. Dazu zwei Marker: **Auslöser-Phase** und **Schwerpunkt-Phase** | „P0 Risikoeinstufung (Auslöser-Phase) · P3 Konzept und Postenplan · P5–P7 Kontrollbetrieb (Schwerpunkt-Phase) · P8 Auswertung" |
| ● | **Übergaben rein / raus** | je Grenze: Objekt · Übergabemedium · Auslöser · Rollen (Kap. 6.1) | „raus: Postenbedarf → Linie, Bestellformular, T-8 Wochen, Security-Planung → Einkauf/TVK" |
| ● | **Beteiligte Rollen** | wer wirkt in welchem Abschnitt mit | „Ordnungsdienstleiter (Abschnitt 4–5), TVK (3), Veranstaltungsleitung (1)" |
| ● | **Abhängigkeiten** | Setzt voraus / Nicht gemeinsam mit / Wahlpflicht-Gruppe | „Wahlpflicht-Gruppe `WP-02`; setzt voraus: Warteflächen- und Rückstaukonzept" |

### Block 3 · Sicherheit und Nachweis — was belegt sein muss, was schiefgehen kann

| Feld | Was gemeint ist | Beispiel |
|---|---|---|
| **Rechtsgrundlage / Auflagenbezug** | Paragraph, Norm, Auflage im Genehmigungsbescheid | „§ 43 VStättVO; Auflage 7 des Bescheids" |
| **Nachweise & Dokumentation** | was aufbewahrt wird, wie lange, inkl. Änderungsdokumentation „von wem, wann" | „Kontrollprotokoll, Einweisungsliste, Planstand mit Änderungsvermerk" |
| **Meldeweg & Eskalation** | wer erfährt was, über welchen Weg, in welcher Stufe; zwei unabhängige Erreichbarkeitswege. **Abweichung von Rechtspflicht oder Behördenauflage ist meldepflichtig an eine benannte Rolle** *(zur Bestätigung, siehe 2.3)* | „Vorfall → Ordnungsdienstleiter → SCU → Notfallmanager; Auflagenabweichung → Leitung Security" |
| **Qualifikations-Gate vor Einsatz** | welcher Nachweis muss **vor** Dienstbeginn vorliegen (ja/nein). Nicht: Anforderungsprofil an den Dienstleister — das liegt in der Linie | „Sachkundenachweis § 34a und dokumentierte Einweisung liegen vor: ja/nein" |
| **Freigabe / Quality Gate** | Kriterien für „darf starten", Abbruchkriterien, dokumentierte Abweichung (Begründung, Befristung, Genehmiger) | „Begehung vor Öffnung abgeschlossen; Abbruch, wenn Rückstau die Verkehrsfläche erreicht" |
| **Risiken** | was regelmäßig schiefgeht, mit Gegenmaßnahme | „Rückstau bei Spitzenandrang; Ausfall von Kräften am Morgen" |

### Block 4 · Anpassung — wie es je Veranstaltung variiert

| Feld | Was gemeint ist | Beispiel |
|---|---|---|
| **Bindung** | immer / entweder–oder / auf Bedarf, wenn … (Kap. 5.2) | „entweder–oder → `WP-02`" |
| **Varianten** | Ausprägungen, die mit derselben Anleitung laufen | „Tag- und Nachtschicht" |
| **Parameter** | was sich nur im Wert unterscheidet, mit Wertebereich | „Anzahl Kontrollspuren 4–12; Kräfte je Schicht" |
| **Bemessungsregel** | Schlüsselzahl oder Algorithmus, mit Quelle | „Kontrollspuren nach erwartetem Andrang je 15-Minuten-Intervall" |
| **Ressourcenbedarf** *(Kandidat — Entscheidung im Sparring)* | internes Personal je Phase, Budget | „P3: 4 PT Planung; P5–P7: durchgehende Präsenz" |

Zum Kandidatenfeld: In Kombination mit dem Phasenprofil wird beim Übereinanderlegen aller Module erstmals sichtbar, dass viele Module gleichzeitig in P4/P5 ihren Peak haben — die Stressphase als Bild statt als Klage (SR-02). Gegenargument: Jedes Feld kostet Befüllungsaufwand, und das größte Risiko des Templates ist Überfrachtung (B-10).

### Block 5 · Lernen und Pflege — damit es nicht veraltet

| Feld | Was gemeint ist | Beispiel |
|---|---|---|
| **Selbstprüfungskennzahl** | **max. 2**, In-Process, dienen dem ausführenden Team — keine Berichtskennzahl (2.3) | „Einweisungsquote vor Dienstbeginn; Anteil Kontrollspuren einsatzbereit zur Öffnung" |
| **Nachbereitung & Rückkopplung** | Debrief-Fragen und wohin die Erkenntnis fließt | „Debrief mit Ordnungsdienstleiter; Änderungen in Kontrollkonzept und Bemessungsregel" |
| **Offene Lücken** | was fehlt, ehrlich benannt | „Bemessung bei kombinierten Veranstaltungen unklar" |
| **Reifegrad** | Ist und **Ziel** (Kap. 8.3) | „Ist 2 Beschrieben · Ziel 3 Angewendet" |
| **Version, Stand, Prüfintervall, freigegeben durch** | inkl. Kadenz: Compliance-Module häufiger als der Rest | „V0.3, 2026-09, Prüfung je Veranstaltung, freigegeben: Leitung Security" |

### 7.1 Außensicht — abgeleitet, nicht neu erfunden

| Feld | Regel |
|---|---|
| Name in Adressatensprache + Synonyme | Übersetzung des Modulnamens |
| Teaser: ein Satz Nutzen | aus Ergebnis und Zweck |
| Adressat | Aussteller, Gastveranstalter, interner Auftraggeber — oder Behörde (Nachweissicht) |
| Typischer Anlass („wenn Sie …") | aus dem Auslöser |
| Enthaltene Leistung | aus dem Ablauf |
| **Nicht enthalten / Abgrenzung** | Pflichtfeld — häufigste Reklamationsursache |
| Was wir von Ihnen brauchen | aus Übergaben und Ablauf |
| Servicezeiten / Einsatzfenster | aus dem Phasenprofil |
| Ausprägungen zur Wahl | aus Bindung und Varianten |
| Bestellweg, Vorlauffrist, Storno *(nur Typ B)* | Praxisstandard der Vergleichshäuser |
| Preis / Verrechnungseinheit *(nur Typ B)* | ohne definierte Einheit kein Preis |
| Ansprechpunkt und Weg bei Reklamation | schließt die SPOC-Lücke (SR-07) |
| Stand / Version / freigegeben durch | identisch mit Innensicht |

Bei **Compliance-Modulen** ist die Außensicht eine **Nachweissicht**: gleiche Struktur, Adressat ist Behörde bzw. Geschäftsleitung; Preis- und Bestellfelder entfallen, an ihre Stelle treten Auflagen-, Mitwirkungs- und Erfüllungsnachweis.

### 7.2 Kopplungsregeln

1. Ein Owner gibt beide Sichten gemeinsam frei.
2. Jede Zusage außen hat innen eine Grundlage. Kein Servicelevel im Schaufenster ohne Messpunkt in der Werkstatt.
3. Jede Mitwirkungspflicht außen ist innen ein Ablaufabschnitt mit Termin. Bestellfrist außen = Vorlauf-Gate innen.
4. Änderungen laufen **innen zuerst**, außen wird neu erzeugt.
5. Verständlichkeitsprüfung als Freigabekriterium: Zwei Leser müssen die Leistungsbeschreibung im gleichen Sinne verstehen (Maßstab des Vergaberechts).
6. **Referenzieren statt duplizieren:** Bestehende Sicherheits- und Einsatzkonzepte werden verlinkt, nicht nachgeschrieben. Das Modul enthält dann Verweis, Owner und Prüfstand.

Die ausführlichen Ausfüllhinweise gehören in das **Steckbrief-Template**, nicht in dieses Dokument — sonst steht dasselbe zweimal da.

---

## 8 · Lebenszyklus

### 8.1 Statuskette

`Entwurf` → `Geprüft` (Vier-Augen-Review und Übergabetest bestanden) → `Freigegeben` → `In Überarbeitung` → `Abgelöst`

*Abgrenzung:* Eine Verprobung an einer echten Veranstaltung ist **nicht Teil dieser Beauftragung**. Ein Modul erreicht innerhalb des Projekts den Status `Freigegeben` auf Basis von Review und Übergabetest — nicht auf Basis eines gelaufenen Einsatzes.

Davor eine **Definition of Ready:** Passt der Kandidat in ein bestehendes Modul? Sind K1–K5 erfüllt? Wer ist Owner? **Ohne Owner kein Entwurf.**

### 8.2 Definition of Done

- [ ] Alle Felder der jeweiligen Ausbaustufe gefüllt **oder** als offene Lücke markiert — keine leeren Felder ohne Vermerk
- [ ] Ergebnis in einem Satz ohne „und" formulierbar
- [ ] Vier-Augen-Review dokumentiert, Reviewer ≠ Autor (bei Compliance-Modulen verpflichtend)
- [ ] **Übergabetest bestanden:** Eine fachfremde Vertretung kann den Ablauf ohne Rückfrage ausführen
- [ ] Übergaben beidseitig bestätigt — die empfangende Rolle hat gegengezeichnet
- [ ] Mindestens eine Selbstprüfungskennzahl benannt
- [ ] Bindung formuliert, auch wenn sie „gilt immer" lautet
- [ ] Im Modulindex registriert, Ablageort und Version gesetzt
- [ ] Bei Compliance-Modulen: Rechtsgrundlage, Nachweisart, Freigabeinstanz belegt

### 8.3 Reifegrade

| | Stufe | Woran man es sieht |
|---|---|---|
| 1 | **Personengebunden** | Funktioniert, ist aber nicht dokumentiert — hängt an Einzelpersonen (Ausgangszustand, SR-05) |
| 2 | **Beschrieben** | Steckbrief vorhanden, Owner benannt — aber je Veranstaltung individuell ausgelegt |
| 3 | **Angewendet** | Wird aus dem Standard getailort, Gates nachweisbar, Vertretung funktioniert, das Team prüft sich an definierten Punkten selbst |
| 4 | **Fortgeschrieben** | Erkenntnisse aus Veranstaltungen ändern nachweisbar den Standard |

**Was innerhalb des Projekts erreichbar ist:** Stufe 2 „Beschrieben" für alle bearbeiteten Module. Stufe 3 „Angewendet" entsteht erst, wenn der Standard bei einer Veranstaltung tatsächlich benutzt wird — also nach Projektende. Das ist keine Lücke, sondern die Definition der Stufen.

Zwei Leitplanken: **Zielstufe je Modul explizit festlegen** — für viele Module ist 3 der richtige Endpunkt, nicht 4. Und Bewertung im gemeinsamen Termin, nicht per Selbstauskunft. Reifegradmodelle scheitern regelmäßig, weil sie als Bewertungs- statt Entwicklungsinstrument benutzt werden.

---

## 9 · Offene Entscheidungen zum Framework

| # | Frage | Empfehlung |
|---|---|---|
| **E-02** | Schnittachse: Ergebnis, Prozess oder Akteur? | Ergebnis — und konsequent durchhalten |
| **E-03** | Compliance- und Leistungs-Module in einem Format? | Gemeinsamer Kern + typspezifische Pflichtfelder (Kap. 4) |
| **E-04** | Außensicht abgeleitet oder eigenständiges Artefakt? | abgeleitet — sonst zwei divergierende Wahrheiten |
| **E-05** | Wo endet Modul, wo beginnt CPFP? | An der Veranstaltungsgrenze (Kap. 2.3). Im Kick-Off zu setzen |
| **E-07** | Preise in der Außensicht sofort? | Erst Mengen und Einheiten transparent, Preisführung danach |
| **E-09** | Braucht die Typologie Modulart **C Enabler**? | Prüffrage: Gibt es mindestens zwei Kandidaten, die weder Rechtspflicht noch verkaufbare Leistung sind und trotzdem einen Owner brauchen? Wenn nein: C entfällt, zwei Arten genügen |
| **E-10** | Übungsformate: Modul oder Linie? | Ungeklärt. Jährliche Unterweisung und auflagenbasierte Räumungsübung sind Pflicht; freiwillige Trainingsformate womöglich Personalentwicklung |
| **E-11** | Feld **Ressourcenbedarf** aufnehmen — und in welcher Auflösung? | Aufnehmen, sobald das Vorbefüllen zeigt, dass es beantwortbar ist |
| **E-12** | Meldepflicht bei Abweichung von Rechtspflicht/Auflage (Kap. 2.3) | Aufnehmen. Kein Controlling, sondern Haftungsweitergabe |
| **E-13** | Ordnerlogik des neuen Repositories und Ablageort des Frameworks | Mit dem inhaltlich Verantwortlichen durchzugehen |

---

## Quellen

**Modularität und Schnitt** · Parnas, *On the Criteria To Be Used in Decomposing Systems into Modules* — http://sunnyday.mit.edu/16.355/parnas-criteria.html · Ulrich & Eppinger, *Product Architecture* — https://my.liuc.it/MatSup/2014/A78601/Ulrich%20-%20Eppinger-%20Prod_Arch_design%20MIT.pdf · Module Drivers / MFD — https://en.wikipedia.org/wiki/Modular_Product_Architecture · Baldwin & Clark, *Design Rules* — https://direct.mit.edu/books/monograph/1856/Design-Rules-Volume-1The-Power-of-Modularity · DSM, Modul- und Interface-Identifikation — https://www.designsociety.org/download-publication/27704/module_and_interface_identification_and_definition_%E2%80%93_a_comprehensive_approach_using_dsm · Granularitäts-Anti-Muster — https://www.oreilly.com/content/microservices-antipatterns-and-pitfalls/

**Service-Modularität und Produktisierung** · Voss & Hsuan — https://wrap.warwick.ac.uk/id/eprint/54807/ · Dekompositionsachsen — https://link.springer.com/article/10.1186/s12913-021-07267-6 · de Blok et al., Service-Interfaces — https://onlinelibrary.wiley.com/doi/abs/10.1016/j.jom.2014.03.001 · Schools of Thought in Service Modularity — https://www.academia.edu/27690969/SCHOOLS_OF_THOUGHT_IN_SERVICE_MODULARITY · Service Productisation — https://osuva.uwasa.fi/server/api/core/bitstreams/5bd36eee-f563-4d5b-8ec7-65f6e11a9969/content · Service Blueprinting, line of visibility — https://servicedesigntools.org/tools/service-blueprint · Feature-Modelle — https://www.isa.us.es/featuremodelanalysis/concepts · Hvam, Product Variant Master — https://backend.orbit.dtu.dk/ws/files/4903251/EvalofPVMver9.pdf

**Modulare Dokumentation** · Red Hat Modular Documentation — https://redhat-documentation.github.io/modular-docs/ · DITA Informationstypen und conref — https://docs.oasis-open.org/dita/v1.2/os/spec/archSpec/dita_technicalContent_InformationTypes.html · Diátaxis — https://diataxis.fr/start-here/ · Google SRE Playbooks — https://sre.google/workbook/on-call/ · Carbon Component Checklist — https://carbondesignsystem.com/contributing/component-checklist/

**Security und Veranstaltung (DE)** · § 43 VStättVO — https://dejure.org/gesetze/VStaettVO/43.html · MVStättVO (ARGEBAU) — https://www.is-argebau.de/Dokumente/4231724917250.pdf · vfdb-Merkblatt 13/01 — https://www.vfdb.de/media/doc/merkblaetter/MB_13_01_sicherheitskonzept.pdf · BaSiGo-Sicherheitsbausteine — https://basigo.vfsg.org/index.php?title=Hauptseite · Muster-Sicherheitskonzept Hannover — https://www.hannover.de/content/download/545450/file/Muster_SiKo_Vers.%203_14-11-2018.pdf · Leitfaden Großveranstaltungen Hessen — https://innen.hessen.de/sites/innen.hessen.de/files/2021-08/leitfaden_sicherheit_bei_grossveranstaltungen.pdf · § 34a GewO — https://www.gesetze-im-internet.de/gewo/__34a.html · DIHK-Merkblatt Bewachungsgewerbe — https://www.dihk.de/resource/blob/2480/fd3b81202233a1493b7a94ad74caba87/recht-merkblatt-bewachungsgewerbe-unterrichtung-oder-sachkundepruefung--data.pdf · Technische Richtlinien (Beispiel) — https://www.duesseldorfcongress.de/wp-content/uploads/2024/12/Technische-Richtlinien-Messe-Duesseldorf-2025_de.pdf · Bestellformular Bewachung (Attributstruktur) — https://www.security-essen.de/media/neue-medien/serviceformulare/allgemein/2024/standservice/d2-bewachung-guardservice-2024.pdf · AGB Serviceleistungen — https://media.koelnmesse.io/koelnmesse/redaktionell/global/downloads/fuer-aussteller/agb-serviceleistungen.pdf · Green Guide, Safe Capacity — https://sgsa.org.uk/physical-factors/calculating-safe-capacity/p-and-s-factors/

**Katalog, Kennzahlen, Reifegrad** · ITIL Portfolio vs. Catalogue — https://blog.invgate.com/service-portfolio · Service Offering — https://www.itsmprofessor.net/2019/04/what-is-service-offering.html · SLA/OLA-Checkliste — https://wiki.de.it-processmaps.com/index.php/Checkliste_SLA_OLA · FIM-Leistungssteckbrief — https://fimportal.de/assets/leistungen_qs_kriterien.pdf?version=2 · Leistungsbeschreibung, § 121 GWB — https://dejure.org/gesetze/GWB/121.html · Ridgway, dysfunktionale Kennzahlen — https://maaw.info/ArticleSummaries/ArtSumRidgway56.htm · Goodhart's Law — https://kpitree.co/guides/frameworks/goodharts-law · Leading Indicators im Arbeitsschutz — https://benchmarkgensuite.com/ehs-blog/leading-vs-lagging-indicators-in-ehs/ · Prozessreife (CMMI) — https://www.tutorialspoint.com/cmmi/cmmi-maturity-levels.htm · Kritik an Reifegradmodellen — https://www.si-labs.com/en/articles/maturity-model/ · Definition of Done — https://www.it-agile.de/agiles-wissen/agile-arbeit/was-ist-eine-definition-of-done/ · EASA Aerodrome Manual, Änderungslogik — https://sassofia.com/blog/summary-of-the-easa-compliant-aerodrome-manual-based-on-amc3-adr-or-e-005/

---

*Nicht freigegeben. Offene Punkte in Kap. 9 sind Entscheidungen des Auftragnehmers, nicht Annahmen dieses Dokuments.*
