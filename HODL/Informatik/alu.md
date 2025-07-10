---
title: ALU
date: 2025-07-07 11:22
tags: 
---

----

### Definition 
- *ALU* (Arithmetic Logic Unit)
- El. Bestandteil, d. zwei Registerinhalte *logisch* o. *artithmetisch* miteinander verknuepft
- Bestandteil d. [Rechenwerks](rechenwerk) 

---

### Addition

**Halbaddierer (HA)**\
Schaltnetz, d. zwei einstellige Dualzahlen addiert, Summe u. Uebertrag bildet (zwei Eingaenge)

**Volladdierer (VA)**\
Schaltnetz, d. drei Bit addieren k., um d. Uebertrag d. naechst niedrigsten Stelle mitzuaddieren (drei Eingaenge)

**Ripple-Carry Addierer**\
Schaltnetz f.d. Addition mehrstelliger Dualzahlen
![](img/alu_1.png)

---

### Zweierkomplement 
Darstellung d. **Vorzeichens** e. Dualzahl\

- Hoechstwertiges Bit bestimmt Vorzeichen:
  - 0: positiv 
  - 1: negativ

**Bildung d. Zweierkomplements**\

1. Bildung d. Einerkomplements $\bar{A}$ (Invertierung) aus Dualzahl $A$
2. Addition e. 1 zum Einerkomplement $(\bar{A}+1)$
$$
\begin{align*}
  A+(\bar{A}+1)&=0 \text{ , da }(n+1)\text{ste Stelle gestrichen}\\
  \Leftrightarrow \bar{A}+1&=-A
\end{align*}
$$

**Darstellbarer Wertebereich**
$$
  -2^{n-1} \text{ bis } +2^{n-1}-1 
$$






----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
