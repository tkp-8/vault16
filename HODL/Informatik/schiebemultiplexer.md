---
title: Schiebemultiplexer
date: 2025-07-07 11:25
tags: 
---

----

### Definition

(Engl: Shifter)\
Eine **logische Schaltung**, die:
 
- aus **mehreren Datenquellen** eine auswaehlt
- zusaetzlich erlaubt, d. ausgewaehlten Daten **bitweise zu verschieben**

---

### Einsatzbereich

- In [ALU](alu) o. [Rechenwerken](rechenwerk)
- Vereinfacht **Multiplikation u. Division**

---

### Aufbau

![](img/schiebemultiplexer_1.png)
- E. Eingang i.m.d. internen [Datenbus](busse) verbunden
- Bei d. anderen Eingaengen: Datenleitungen einerseits um e. Stelle nach **links** verschoben, andererseits um e. Stelle nach **rechts**
- Zwei Steuerleitungen: waehlt gewuenschte Positionierung e. ALU-Operanden aus
- Bit w. entweder v. links o. rechts nachgeschoben (Eingaenge **Left Input**, LI, **Right Input**, RI)
- Herausfallendes Bit steht je nach Schieberichtung an den Ausgaengen (**Left Output**, LO, **Right Output**, RO)
- Oft **Carry Flag**, um entweder d. Herausfallende Bit zwischenzuspeichern o.d. Inhalt d. Carry Flags nachzuschieben

Rotation:
- Wenn d. Schiebe-Eingaenge m.d. zugehoerigen Ausgaengen **verbunden** w., *rotieren* d. Bits um e. Stelle



----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
