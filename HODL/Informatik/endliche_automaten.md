---
title: Endliche Automatenend
date: 2025-05-06 08:36
tags: 
---

----

### Definition 
##### Endlicher Automat
Modell zur Darstellung eines **Zustandsueberganssystems** mit begrenztem Speicher


##### Sprache des Automaten
$L(M)$: Menge aller [Woerter](woerter), die der Automat $M$ akzeptiert\
**[Regulaere Sprachen](regulaere_sprachen):** [Sprachen](sprachen) fuer die es einen endlichen Automaten gibt

##### $w$-Lauf
Wenn der Lauf sich auf die Eingabe $w$ bezieht\
**akzeptierender** Lauf/**verwerfender** Lauf

---

### Konzept
- Beschreibung der Verarbeitung von Sprachen
- Schwerpunkt ist Erkennen korrekter Woerter

---

### Eigenschaften
- Loesen des **Wortproblems** von bestimmten formalen Sprachen
- **Eingabe:** [Wort](woerter), **Ausgabe:** Wahrheitswert, ob Eingabe ein Element der zugehoerigen Sprache
- EA **akzeptiert**/**verwirft** das Eingabewort
- Lesen des Wortes erfolgt nur **zeichenweise**
- EA kann waehrend der Verarbeitung endlich viele **Zustaende** annehmen
- **Zustandsuebergang** haengt vom aktuellen Zeichen der Eingabe ab (Ausnahme $\varepsilon$-Uebergaenge)
- **Endzustaende** bestimmen den Ausgabewert

---

### Berechnungsmodelle
[DEA](dea): Immer **eindeutiger** Folgezustand

[NEA](nea): **Mehrere** oder **keine** Folgezustaende moeglich

[Potenzautomat](potenzautomat): Konstruiert aus einem **NEA** ein **DEA**

---

### Zustandsdiagramm

![](img/ea_1.png)

----

----
**Backlinks:**
- [📂Formale_Sprachen&Automaten](📁Formale_Sprachen&Automaten)
