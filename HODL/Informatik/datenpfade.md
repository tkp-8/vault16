---
title: Datenpfade
date: 2025-07-10 01:06
tags: 
---

----

### Definition
Eine Sammlung aus [Rechenwerken](rechenwerk) (z.B [ALU](alu), [Schiebemultiplexer](schiebemultiplexer)), 
d. Datenverarbeitungsoperationen, [Register](prozessorregister) u. [Busse](busse) ausfuehren

---

### Datenpfadstrukturen

##### Rechenwerk einer [Ein-Adress-Maschine](datenzugriffsarchitektur)
![](img/datenpfade_1.png)
- ALU u. Registerfeld m. **einem** internen (bidirektionalen) Datenbus verbunden

Nachteil: 
Abarbeitung e. [Maschinenbefehls](maschinenbefehl) erfordert **drei Taktzueklen**:
1. Erster Operand i. Hilfsregister
2. Zweiter Operand i. Hilfsregister
3. Ergebnis d. Verknuepfung v. F(unction)-Ausgang d. ALU ins Register File

##### Rechenwerk einer Zwei-Adress-Maschine

- Erfordert nur zwei Taktzyklen f.d. selben Befehl, da Register A u. B gleichzeitig geladen w.k.

##### Rechenwerk einer Drei-Adress-Maschine

![](img/datenpfade_2.png)
- Typisch fuer [RISC-Prozessoren](risc)
- Ein Taktzyklus f.d. selben Befehl, da f.d. Operanden u.f.d. Ergebnis eigene Datenbusse bereitstehen
- **Register-ALU** (RALU)



----

----
**Backlinks:**
- [Rechenwerk](/rechenwerk)
