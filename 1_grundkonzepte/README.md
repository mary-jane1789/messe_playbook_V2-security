# 1_grundkonzepte

Was für alle Bereiche gilt. Jedes Detailkonzept und jedes Modul bezieht sich
hierauf, statt es erneut zu beschreiben.

Ein Grundkonzept pro Datei, flach. Die Herkunft steht im Frontmatter der Datei
(`quelle:`), nicht im Ordnernamen — sie ist eine Angabe, keine Gliederung.

## Was ein Grundkonzept ist

Ein Begriff oder Modell, das bereichsübergreifend gilt **und** gebraucht wird,
um Module und Detailkonzepte überhaupt beschreiben zu können.

Der Gegentest: Nimm es weg — lässt sich ein Modul dann noch schreiben? Bei
Phasen nicht, ein Modul benennt seine Phasen. Bei den Abrechnungsmodellen der
Messe schon, obwohl auch sie bereichsübergreifend gelten. Bereichsübergreifend
allein genügt also nicht.

## Wo die Instanzen liegen

Die Dateien hier sind nicht alle gleich gebaut. Manche beschreiben ein Schema
und seine Ausprägungen zusammen, andere nur das Schema. Damit das sichtbar ist
und nicht mit der Zeit verwischt, deklariert jede Datei es im Frontmatter:

| `instanzen:` | bedeutet | Beispiel |
|---|---|---|
| `inline` | Schema und Ausprägungen stehen in derselben Datei | `phasen.md` — erklärt die Phase und listet P0 bis P7 |
| ein Ordnerpfad | die Ausprägungen liegen in dem genannten Ordner | `ablauf.md` → `2_detailkonzepte/ablauf/` |
| `keine bisher` | das Schema gilt, die Ausprägungen sind noch nicht festgelegt | `gremium.md` — es gibt nur Entwürfe |

`inline` ist richtig, wo die Menge geschlossen und entschieden ist und sich immer
gemeinsam ändert. Ein Ordnerpfad ist richtig, wo Ausprägungen vielfach und
unabhängig voneinander entstehen.

**Verweisrichtung.** Ein Schema zeigt auf den **Ordner** seiner Instanzen, nie
auf einzelne Dateien darin. Der Ordnerpfad bleibt stabil, egal wie viele Dateien
darin liegen; eine Dateiliste müsste bei jeder neuen Instanz angefasst werden.
Damit bleibt die Grundregel gewahrt, dass ein Grundkonzept nicht aufzählt, wer
es benutzt.

**Namen als Signal.** Schema im Singular (`rolle.md`, `gremium.md`, `modul.md`,
`ablauf.md`), entschiedene geschlossene Menge im Plural (`phasen.md`).

## Vorgesehen

| Datei | Inhalt | `instanzen:` | Quelle | Zustand |
|---|---|---|---|---|
| `veranstaltung.md` | Art × Veranstalter × Größe, Unterschiede nach Veranstalter | inline | V1.0 Kap. 1 und 4 | belastbar |
| `phasen.md` | P0–P7 und die Gates an den Übergängen | inline | V1.0 Kap. 2 | belastbar |
| `lead-modell.md` | die drei Lead Rollen und der Lead Committee | inline | V1.0 Kap. 6 | Entwurf, muss ausgestaltet werden |
| `rolle.md` | was eine Rolle ausmacht: strukturell, mit Mandat und Reporting-Linie | keine bisher | V1.0 Kap. 6 | muss ausgestaltet werden |
| `gremium.md` | was ein Gremium ausmacht: Zweck, Mitglieder, Mandat, Entscheidungsfähigkeit, Rhythmus | keine bisher | V1.0 Kap. 7 | Schema festlegbar, Gremien sind Entwürfe |
| `dienstleister.md` | Kategorien und die Einordnung Pflicht / Wahl-Pflicht / Wahl | inline | V1.0 Kap. 10 | Vollständigkeit zu prüfen |
| `modul.md` | was ein Modul ist und wie es beschrieben wird | `3_instanzen/module/` | Modul-Framework | Feldkatalog steht, an keinem echten Modul erprobt |
| `ablauf.md` | was ein Ablauf ausmacht: Auslöser, Schritte, beteiligte Rollen, Ergebnis | `2_detailkonzepte/ablauf/` | neu | zu schreiben |

Angelegt sind `veranstaltung.md` (19.08.2026) sowie `phasen.md` und `modul.md`
(23.08.2026). Was
tatsächlich übernommen wird und in welcher Verdichtung, wird vor der Migration
besprochen. Die Spalte „Zustand" bezieht sich auf V1.0, nicht auf diese Ablage —
offene Punkte stehen in `0_meta/offene-punkte.md`.

Acht Dateien, flach. Unterordner erst, wenn es deutlich mehr werden.

**Auslöser zum Nachdenken über eine Teilung:** Wenn mehr als etwa die Hälfte der
Dateien hier ihre Ausprägungen außerhalb der eigenen Datei hat, ist der Ordner
tatsächlich zwei Dinge und sollte geteilt werden. Heute sind es zwei von acht —
`modul.md` und `ablauf.md`.

## Abgrenzung zum Glossar

Das Glossar sagt, was ein Wort bedeutet. Ein Grundkonzept sagt, was gilt.

Bei „Gate" reicht der Glossareintrag, weil die acht konkreten Gates in
`phasen.md` stehen — das Wort braucht nur eine Definition, die konkreten Fälle
haben schon ein Zuhause. Wo es kein solches Elternkonzept gibt und ein Modul auf
einen konkreten Fall zeigt, braucht es eine eigene Datei. Deshalb ist „Gremium"
eine Datei und „Gate" ein Glossareintrag.

## Nicht hierher

**Ins Glossar:** Gate.

**In den Projektkontext:** Worum geht es, Verankerung im Unternehmen,
Leitprinzipien, Geltungsbereich.

**Als Feld ins Modul, nicht als Konzept:** Risikostufe (`niedrig | mittel | hoch`)
mit der Regel, dass „hoch" eine Pre-mortem-Pflicht auslöst. Nicht alles aus dem
Playbook wird ein Konzept — manches wird ein Feld mit einer Regel.

**In die Abläufe** (`2_detailkonzepte/ablauf/`): Eskalationspfade und
Krise/Triage in den Krisenablauf, Retrospektiven und Pre-mortem in die
Lernschleife, Konfiguration einer Veranstaltung in die Konfiguration. Sie sind
Abläufe, keine Grundkonzepte — das Schema dafür ist `ablauf.md`.

**Nicht übernommen** — bleibt im Playbook V1.0 gültig, wird hier nur nicht
gebraucht: Check-Points, Entscheidungstypen, Risikomanagement als eigenes
Konzept, Abrechnungsmodelle, SLAs, methodische Empfehlung zum Service Blueprint.
