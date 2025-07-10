---
title: Status-Flags
date: 2025-07-07 11:25
tags: 
---

----

### Definition
Einzelne **Bits** innerhalb d. [Statusregisters](statusregister), d. bestimmte Eigenschaften
d. letzten **Rechenergebnisses** anzeigen

---

### Bestimmung von Status-Flags
Ausgaenge $f_{N-1},\ldots ,f_{0}$ bilden d. **Ergebnisbus** d. [ALU](alu) (vgl. [Datenpfade](datenpfade))\
Belegung **dieser Bits** u.d. Belegung d. **Uebertrags** $c_N$ bilden d. Status-Flags

1. *Carry $C$*: Uebertrag i.d. hoechsten Stelle, $C=c_N$
2. *Zero $Z$*: alle Bits v. $F$ sind Null, $Z=\overline{f_{N-1}\lor f_{N-2}\lor \ldots \lor f_{0}}$
3. *Minus $M$*: negatives Vorzeichen bei [Zweierkomplement](alu)-Darstellung, $M=f_{N-1}$
4. *Overflow (bzw. Underflow) $V$*: d. Ergebnis i. zu gross (klein), um mit $N$-Bit-Wortbreite dargestellt zu w., $V=c_N\oplus c_{N-1}$





----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
