---
status: laufend
stand: 2026-08-23
---

# Offene Punkte

Was noch entschieden werden muss, bevor es im Repository als gesetzt gilt.
Je Punkt: Frage, Stand der Klärung.

Entschiedenes steht in `entscheidungen.md`, nicht hier. Ein Punkt wandert
dorthin, wenn er entschieden ist.

## Zu klären mit der Messe

**Sind die Dienstleisterkategorien vollständig?** V1.0 Kap. 10 führt sieben
Kategorien und drei Tiers. Nachfragen, ob die Liste vollständig ist und ob die
Einordnung Pflicht / Wahl-Pflicht / Wahl je Kategorie so gilt.

**Gremien.** Es gibt bisher nur Entwürfe. Das Schema ist festlegbar, die
konkreten Gremien nicht. Zu klären, welche Gremien tatsächlich gelten sollen —
der Lead Committee ist laut V1.0 nicht etabliert, weil die dritte Lead Rolle
fehlt.

**Benennung der Veranstaltungsarten.** Warum wird die Messe auf der Achse Art
nach B2B und B2C getrennt, ist eine Partnermesse eine eigene Art, und verwendet
die Messe die Begriffe B2B und B2C oder Eigenmesse und Gastmesse? Reine
Wording-Frage, gesammelt in `../4_workspace/fragen-an-ma.md`.

**Gate P6 → P7 bei Eigenveranstaltungen.** V1.0 Kap. 2 setzt das Gate „nur bei
Gastveranstaltungen" (Rückabnahme durch TVK) und sagt für Eigenveranstaltungen
ausdrücklich, es sei „kein formales Gate erforderlich". Da die Eigenveranstaltung
der Referenzrahmen ist, hat damit genau der Regelfall einen Übergang ohne
Bedingung. Zu klären: Ist das gewollt, oder gehört eine Bedingung hin? Kandidat
aus dem Kapiteltext, nicht von V1.0 als Gate gesetzt: Security-Übergabe an die
Hausverwaltung und Inventar-Übergabe im Clean-Cut.

**Primär-Träger in P0.** Die Übersichtstabelle nennt für P0 nur Brand &
Marketing, der Kapiteltext lässt Logistics & Security das Sicherheits-
Grundkonzept zuliefern, und das Gate P0 → P1 verlangt einen Security-/Logistik-
Check. Ein Security-Modul mit Auslöser-Phase P0 hat damit in seiner Auslöser-
Phase keinen Träger. Mit der Festlegung, dass Primär-Träger weiche Deskriptoren
ohne RACI-Wirkung sind, entschärft — für die Modulbemessung aber zu bestätigen.

**Braucht die Modulart eine dritte Kategorie?** Ein Modul ist entweder eine
Pflicht aus dem Recht oder eine Leistung, die an Aussteller oder einen internen
Auftraggeber verkauft wird. Offen ist, ob es eine dritte Art für
Befähigungsleistungen braucht — Dinge, die keines von beidem sind, aber trotzdem
jemanden brauchen, der sie verantwortet. Die Frage an die Messe: Gibt es bei
Security mindestens zwei solche Bausteine? Kandidaten sind Übungen und
Einweisungen, aber ein Teil davon ist rechtlich verlangt und wäre damit ohnehin
Pflicht. Wenn nein, genügen zwei Arten und das Modell wird einfacher. Die
Modulart steuert, welche Felder Pflicht sind — die Frage ist also nicht
folgenlos.

**Übungs- und Trainingsformate — Modul oder Linie?** Jährliche Unterweisung und
auflagenbasierte Räumungsübung sind Pflicht und damit Modulkandidaten.
Freiwillige Trainingsformate könnten Personalentwicklung sein und in die Linie
gehören. Hängt mit der Frage nach der dritten Modulart zusammen.

**Richtwerte der Größenklassen.** Die Werte gelten als Richtwerte, die
Einstufung nimmt die verantwortliche Rolle vor (E-30). In V1.0 sind die
Quadratmeter als Annahme und die Aussteller- und Besucherwerte als geschätzte
Hypothesen markiert; ob die Richtwerte in dieser Höhe taugen, ist zu bestätigen.

## Grundkonzepte, die noch ausgestaltet werden müssen

**Lead-Modell.** Die drei Lead Rollen sind in V1.0 Kap. 6 benannt, aber der
Operations Lead trägt laut Playbook heute keine gleichberechtigte Verantwortung.

**Rolle.** Schema muss geschrieben werden. Die konkreten Rollen entstehen dort,
wo sie vorkommen — in Modulen und Abläufen.

**Ablauf.** Schema ist neu und noch nicht geschrieben: Auslöser, Schritte,
beteiligte Rollen, Ergebnis.

**Doppelung Lead Committee.** Er kommt im Lead-Modell, im Schema Gremium und in
der Konfiguration vor (dort gibt er das Commitment). Die Beschreibung gehört ins
Lead-Modell, die anderen verweisen darauf.

## Abläufe — Zuschnitt und Inhalt

Alle drei sind Entwürfe:

**Konfiguration.** Vier Schritte laut V1.0 Kap. 15. Offen: wie Modul und
Parameter genau zusammenhängen — welche Felder eines Moduls in der Konfiguration
als Parameter erscheinen.

**Krisenablauf.** Nimmt die Eskalationspfade auf. Offen sind die
Triage-Kriterien und Zeitschwellen; V1.0 Kap. 14 führt sie selbst als offenen
Punkt (SR-03).

**Lernschleife.** Keines der fünf Retrospektive-Formate aus V1.0 Kap. 16 ist
etabliert, die Moderation ist nicht geklärt.

## Weiter offen

**Wohin verweist das Steckbrief-Feld „Meldeweg und Eskalation"?** In
`modul.md` verweist es auf `2_detailkonzepte/ablauf/`. Der Krisenablauf dort ist
noch nicht geschrieben; der Verweis zeigt bis dahin auf den Ordner.

**CP-2d darf nicht verlorengehen.** Die Check-Points sind nicht übernommen.
CP-2d ist die einzige in V1.0 belegte Security-Übergabe:
Security-Umsetzungsvorschlag (Postenplan, Schichten) von Logistics & Security an
Expo Realisation. Gehört in `2_detailkonzepte/module/security-module-detailkonzept/uebergabekarte.md`.

**Umrechnung des Modul-Frameworks auf P0–P7.** Das Framework v0.2 rechnet
durchgehend mit der Vor-Merge-Zählung P0–P8. V1.0 ist Source of Truth, die
Umrechnungsregel lautet: P0, P1, P2 bleiben, P3 bis P8 minus eins. Betroffen sind
neun Stellen (Zeilen 16, 35, 103, 154, 205, 211, 257, 281, 283). Die Quelldatei
in `quellen/` bleibt als Beleg unangetastet; die Korrektur greift beim Schreiben
von `modul.md`. Zusätzlich inhaltlich zu korrigieren: „Hard Cut vor P4 (SR-02)"
(Zeile 154) — V1.0 hat SR-02 als Vollständigkeitscheck vor P3 und Gate P2 → P3
entschieden, ausdrücklich ohne harten Cut-off.

**Geltungsbereich in den Projektkontext.** Der Referenzrahmen Eigenveranstaltung
steht bisher in `README.md` und `CLAUDE.md`. Er gehört zusätzlich in den
Geltungsbereich in `projektkontext.md`, wenn die einleitenden Kapitel aus V1.0
dort übertragen werden (E-14).

**Die Schnittregeln fehlen.** `1_grundkonzepte/modul.md` sagt, was ein Modul
ist. Wie man in der Praxis entscheidet, wo eines aufhört, stand im
Schwesterdokument des Modul-Frameworks (`modul-vorgehen`), das nicht vorliegt.
Bisher ist der Werkstatt-Test der einzige Ersatz: Bräuchte eine Vertretung zwei
verschiedene Anleitungen, sind es zwei Module. Ob das für die Schnittarbeit
genügt, zeigt sich beim ersten echten Modul.

**Das Modul-Framework ist an keinem echten Modul getestet.** Alle Beispiele im
Framework sind ausdrücklich hypothetisch und stammen aus der Recherche, nicht
aus dem Haus. Sie sind deshalb nicht ins Repository übernommen. Der Feldkatalog
in `modul.md` ist damit vollständig, aber unerprobt — der erste Durchgang mit
dem Leiter Security ist gleichzeitig sein Test.

**Umkehrbarkeit von Entscheidungen.** V1.0 Kap. 9 sagt, sicherheitskritische
Entscheidungen seien „grundsätzlich nicht reversibel". Im Steckbrief steht dafür
kein eigenes Feld. Stattdessen trägt die Entscheidungsfrist die praktische Folge
(bis wann muss entschieden sein), und das Zustimmungsfeld die Doppelfreigabe.
Das ist eine bewusste Verkürzung der V1.0-Aussage, damit sie nachlesbar bleibt.

**Herleitung des Modul-Frameworks.** Das Framework begründet auf zwei Seiten,
warum es so aussieht — dreizehn Bedarfe aus dem Projekt, je mit der Konsequenz
für das Format. Sie sind nicht in `modul.md` übernommen und bleiben in der
Quelldatei `quellen/modul-framework-v0.2.md`, die diese Funktion hat.

**Modul-Framework Kap. 2.2** — VStättVO, vfdb 13/01, verkaufbare Leistungen.
Vorschlag: nach `2_detailkonzepte/module/security-module-detailkonzept/`, weil beim nächsten Bereich nichts davon gilt.

**Ausgabeformat der Steckbrief-Vorlage.** Der Weg ist entschieden (R-23), das
Format nicht. Dazu kommt: Weil keine Beispiele ins Repository übernommen sind,
muss die Vorlage die Ausfüllhinweise allein tragen. Sie wird damit wichtiger als
bisher geplant.

**Workflow für Dokumente, Inputs und Kundeninteraktionen.** Fehlt bisher; als
Entwurf notiert in `../4_workspace/workflow-dokumente-inputs-kundeninteraktionen.md`.
Offen ist zuerst der Ort — Konvention in `0_meta/` oder Ablauf in
`2_detailkonzepte/ablauf/`.

### Aus Veranstaltung (V1.0 Kap. 1 und 4), dort selbst als offen markiert

- RACI-Delta je Phase bei Gast und Partner. Bisher nur als Grundsatz formuliert.
- Claim-Komplexität bei Gast: wer hat bestellt, wer geliefert, wem wird in
  Rechnung gestellt.
- Begriffliche Abgrenzung Ticket-System gegen Gast-Shop (Gast-OSC).
- Zuordnung von „Imagine World" in der Typologie.
- Strategische Relevanz von Messe B2C × Eigen und × Partner.

## Lücken im Playbook V1.0

Nicht Verdichtungsfragen, sondern fehlende Inhalte:

- Triage-Kriterien und Zeitschwellen je Stufe (Kap. 14)
- keines der Retrospektive-Formate in der Praxis etabliert (Kap. 16)
- der Lead Committee ist nicht etabliert (Kap. 7)
- **Größenklassen nach unten offen** (Kap. 1). Die Spalten sind im Original als
  Untergrenzen geschrieben („> Aussteller"). Eine Veranstaltung unterhalb der
  Klasse klein fällt in keine Klasse. Für die Bemessung von Modulen relevant.
- **Ende von P5 ist nicht relativ T0 bemessen** (Kap. 2). Die Übersichtstabelle
  nennt „Eröffnung bis letzter Tag"; die Dauer (2 bis 3 Laufzeittage, maximal 5)
  steht nur im Kapiteltext. P6 hängt an diesem Endpunkt und ist damit ebenfalls
  nicht T0-relativ bemessen.
- **Bezugspunkt von P6 widersprüchlich** (Kap. 2). Übersichtstabelle: `T0 +1 bis
  +2 Tage`. Kapiteltext: „1 bis 2 Tage nach Ende der Laufzeit". Die
  Tabellenlesart legt den Abbau in die Laufzeit. Für `phasen.md` ist die
  Kapiteltext-Lesart übernommen; V1.0 bleibt an der Stelle uneindeutig.
- **Gate P6 → P7 ohne Bedingung für den Referenzfall** (Kap. 2). Siehe oben unter
  „Zu klären mit der Messe".
- **Gate P1 → P2 als Tätigkeit formuliert** (Kap. 2). „Informationen über die
  Sales-Kampagnen an die operativen Bereiche weitergeben" ist kein prüfbarer
  Zustand, anders als die übrigen sieben Gates. In `phasen.md` durch eine als
  Zustand prüfbare Fassung ersetzt, der V1.0-Wortlaut steht dort daneben.
- **Zeitfenster von P6 und P7 schließen nicht aneinander an** (Kap. 2). P6 endet
  rund T0 +4 bis +5 Tage, P7 beginnt bei T0 +1 Woche. Die Lücke zwischen P2 und
  P3 ist geschlossen (P3 beginnt bei T0 −2 Monate); diese bleibt offen.
- **Phasenzählung dreifach notiert** (Kap. 2 Einleitungssatz und Versionierung:
  „P0 bis P6"; Grafik 11: „nach P8"). P0 bis P7 ist gesetzt, siehe
  `entscheidungen.md`. Die drei abweichenden Stellen bleiben in V1.0 stehen und
  sind beim Zitieren zu beachten.
- **Keine Regel, wenn die drei Größenwerte auseinanderfallen** (Kap. 1). V1.0
  sagt, sie korrelieren „typischerweise", verlangt aber die Einordnung in genau
  eine Klasse. Mit der Einstufung durch die verantwortliche Rolle (E-30)
  entschärft, aber nicht geregelt.
