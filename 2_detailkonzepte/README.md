# 2_detailkonzepte

Wo ein Grundkonzept aus Ebene 1 ausdetailliert wird.

Gegliedert nach Baustein, wie Ebene 3:

```
2_detailkonzepte/
├── module/
│   └── <bereich>-module-detailkonzept/
└── ablauf/
    ├── konfiguration.md
    ├── krisenablauf.md
    └── lernschleife.md
```

Bereichsordner unter `module/` werden angelegt, wenn der Bereich beauftragt ist —
nicht vorher. Abläufe sind nicht bereichsspezifisch, deshalb steht `ablauf/`
daneben und nicht darin.

Unter `module/` liegen Ordner, weil ein Bereichs-Detailkonzept aus mehreren
Dateien besteht. Unter `ablauf/` liegen Dateien, weil ein Ablauf eine ist.

## Abgrenzung zu Ebene 3

Hier stehen **Konzepte**, dort stehen **ausgefüllte Schemata**. Ein Krisenablauf
ist ein Konzepttext; ein Modulsteckbrief ist ein gefülltes Formular nach der
Feldliste aus Ebene 1.

## Was in einem Bereichs-Detailkonzept steht

Dieselben drei Fragen wie in `1_grundkonzepte/modul.md`, mit den Antworten
dieses Bereichs:

- **Was ist ein Modul dieses Bereichs?** Welche Treiber hier dominieren,
  welche Vorgaben von außen seine Existenz erzwingen.
- **Woran erkennt man eines?** Die Modullandkarte: welche Kandidaten geprüft
  wurden, was dabei herauskam, und wie die Grenzfälle entschieden wurden.
- **Wie wird eines beschrieben?** Ausfüllhinweise, Bemessungsregeln,
  Beziehungen zwischen den Modulen des Bereichs.

## Anwenden, nicht wiederholen

Ebene 2 wendet Ebene 1 an. Sie definiert nicht neu.

Die harte Grenze: **keine zweite Feldliste.** Welche Felder Pflicht sind,
steuert die Modulart, nicht der Bereich. Ein Bereich darf Felder ergänzen —
aber keine aus Ebene 1 umbenennen, weglassen oder anders bedeuten lassen.

Der Test vor jedem neuen Satz hier: **Stimmt er beim nächsten Bereich auch?**
Wenn ja, gehört er nach `1_grundkonzepte/`.
