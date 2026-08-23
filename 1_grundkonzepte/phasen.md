---
status: entwurf
stand: 2026-08-23
quelle: Playbook V1.0, Kap. 2; Geltung über die Veranstalter-Modelle Kap. 4
instanzen: inline
---

# Phasen

Eine Veranstaltung durchläuft acht Phasen, P0 bis P7. Die Zeitachse ist relativ
zum ersten offiziellen Laufzeittag (T0). Die Grenzen sind weich: Aktivitäten
laufen parallel oder ziehen sich durch, Zeitfenster können überlappen. An jedem
Phasenübergang steht ein Gate.

Die Phasenstruktur gilt für alle Veranstalter-Modelle. Der Veranstalter
verändert die Rollenbesetzung, nicht die Struktur (siehe `veranstaltung.md`).
Bemessung und Besetzung sind an der Eigenveranstaltung ausgerichtet; wo V1.0
für Gastveranstaltungen abweicht, ist das an der Stelle vermerkt.

## Wozu das Phasenmodell

Die Phasen sind ein Gerüst zur Orientierung und zur Steuerung. Die Trennung ist
konzeptionell: Sie ordnet Verantwortungen und Qualitätsstandards einem
Zeitabschnitt zu.

Eine Phase ist ein Zeitabschnitt, keine Leistung. Getragen wird sie nicht von
einem Bereich — Verantwortung wird auf das Gerüst gemappt, nicht aus ihm
abgeleitet. Ein Modul benennt die Phasen, in denen es wirkt.

## Die acht Phasen

| Phase | Name | Zeitfenster | Primär-Träger |
|---|---|---|---|
| P0 | Strategische Konzeption | T0 −12 bis −9 Monate | Brand & Marketing |
| P1 | Sales + Marketing | T0 −9 bis −6 Monate | Sales + Brand & Marketing |
| P2 | Feinplanung | T0 −6 bis −2 Monate | Customer Success + Operations Management + Expo Realisation + Logistics & Security |
| P3 | Realisierung (Heiße Phase) | T0 −2 Monate bis −1 Tag | Operations Management |
| P4 | Aufbauphase | T0 −3/4 Tage bis T0 | Expo Realisation + ServicePartner |
| P5 | Laufzeitphase | T0 bis letzter Laufzeittag | Customer Success + Operations Management + Logistics & Security |
| P6 | Abbauphase | Ende der Laufzeit +1 bis +2 Tage | ServicePartner + Logistics & Security |
| P7 | Nachbereitung | T0 +1 bis +4 Wochen | Operations Management |

**Primär-Träger sind weiche Deskriptoren.** Die Spalte sagt, welche Bereiche eine
Phase prägen. Sie ist keine RACI-Zuordnung: aus ihr folgt weder Accountability
noch Responsibility. Der Kapiteltext nennt in einzelnen Phasen weitere Bereiche
mit benannter Aufgabe, die hier nicht stehen — in P0 liefert Logistics & Security
das Sicherheits-Grundkonzept zu, in P4 verantwortet Logistics & Security den
Ladehof und Customer Success den Aufbau der Eigenbedarfs-Flächen, in P5
troubleshootet Expo Realisation auf der Fläche.

### Zu den Zeitfenstern

- **P3.** V1.0 nennt `T0 −1 Monat bis −1 Tag`. Der Beginn ist auf T0 −2 Monate
  vorgezogen, damit P2 und P3 aneinander anschließen.
- **P4.** „−3/4 Tage" heißt drei bis vier Tage vor T0.
- **P5.** Typisch 2 bis 3 Laufzeittage, maximal 5. Das Ende ist nicht relativ zu
  T0 bemessen.
- **P6.** Bezugspunkt ist das Ende der Laufzeit, nicht T0. Die Übersichtstabelle
  in V1.0 notiert `T0 +1 bis +2 Tage`; der Kapiteltext zu P6 bemisst dieselbe
  Phase ab dem Ende der Laufzeit.
- **P7.** Bei größeren Veranstaltungen dauert die Phase auch Monate.
- Zwischen P6 und P7 liegen die Zeitfenster nicht aneinander an. Die Werte sind
  Richtwerte, keine Kalenderintervalle.

## Die acht Gates

Ein Gate definiert, was vorliegen muss, bevor die nächste Phase beginnt.

| Übergang | Gate-Kriterien |
|---|---|
| P0 → P1 | Security-/Logistik-Check; Checkliste; Briefing des Lead Committees; Ernennung des Lead Committees |
| P1 → P2 | Briefing für die operativen Bereiche ist von den Leads abgenommen |
| P2 → P3 | Hallenplan im Tool OrgaNice erfasst; Cross-Check in OrgaNice durchgeführt |
| P3 → P4 | Finale Hallenplanung liegt vor |
| P4 → P5 | Standabnahme durch Veranstaltungstechniker; Feuerwehr-/Brandschutz-Check |
| P5 → P6 | Abbaubesprechung |
| P6 → P7 | Bei Gastveranstaltungen: Rückabnahme durch TVK. Bei Eigenveranstaltungen ist keine Bedingung benannt — offen. |
| P7 → P0 | Lessons Learned — schließt den Kreis zur nächsten Edition |

Die operative Ausgestaltung je Gate — Checklisten-Inhalte, Verantwortliche,
Dokumentationsort — ist noch nicht festgelegt.

Zu P1 → P2: V1.0 formuliert das Kriterium als Tätigkeit („Informationen über die
Sales-Kampagnen an die operativen Bereiche weitergeben"). Hier steht die als
Zustand prüfbare Fassung.
