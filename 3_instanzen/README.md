# 3_instanzen

Die ausgefüllten Module — je Modul eine Datei, gefüllt nach der Feldliste aus
`1_grundkonzepte/modul.md`.

Gegliedert nach Baustein, wie Ebene 2:

```
3_instanzen/
└── module/
    └── <bereich>-module-instanzen/
```

Neue Bereichsordner werden angelegt, wenn der Bereich beauftragt ist. Kommt ein
weiterer Baustein zu eigenen Instanzdateien — etwa Gremien oder Rollen, sobald
sie festgelegt sind — bekommt er neben `module/` einen eigenen Ordner.

Die Zwischenebene `module/` hat zwei Gründe: Sie hält die Gliederung symmetrisch
zu Ebene 2, und `modul.md` kann auf **einen** stabilen Ordner zeigen statt auf
eine Liste, die mit jedem Bereich wächst.

## Abgrenzung zu Ebene 2

Dort stehen **Konzepte**, hier stehen **ausgefüllte Schemata**. Ein Krisenablauf
ist ein Konzepttext und liegt in Ebene 2; ein Modulsteckbrief ist ein gefülltes
Formular und liegt hier.

Getrennt wird überhaupt nur, wo Instanzen vielfach und unabhängig voneinander
entstehen — zu verschiedenen Zeiten, mit verschiedenen Ownern, jede für sich
änderbar. Bei Phasen ist das nicht so, deshalb stehen P0 bis P7 in `phasen.md`
selbst. Ob ein Schema seine Ausprägungen hier hat, steht in seinem Feld
`instanzen:`.
