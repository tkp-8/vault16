---
title: Datenzugriffsarchitektur
date: 2025-07-10 00:29
tags: 
---

----

### Definition  
Teil d. [Rechenwerks](rechenwerk) e. [Prozessors](prozessor) u. beschreibt, aus welchen Quellen 
d. **Operanden** f. arithmetisch-logische Operationen stammen u. wohin d. **Ergebnisse**
geschrieben w.

---

### X-Adressen-Maschinen
Form der *Datenzugriffsarchitektur*, b.d. [Maschinenbefehle](maschinenbefehl) **X Speicher- o. Registeradressen enthalten**

---

### Registerarchitektur
M. spricht v.e. *Registerarchitektur*, wenn i. Rechenwerk adressierbare **Datenregister** vorhanden s.
- Datenregister bilden **Register-Block/Register-File**
- Ein-/Zwei-/Drei-Adresse-Maschinen <- bestimmt v.d. Zahl d. **internen Daten- u. Adressbusse**, d.d. Registerblock m.d. [ALU](alu) u.d. [Speicher](speicher) verbinden
- Zahl d. Adressen, d.i.e. Befehl angegeben koennen, gibt keine Auskunft ueber d. **Hardware-Implementierung** -> man sollte v.e. **X-Adress-Befehlssatz** sprechen 

---

### Stapelarchitektur
Anstelle e. Register-Files w. hier e. [Stapel](stapel) benutzt, um Operanden o. Ergebnisse zu speichern
- A.d. Prozessor **integrierter** LIFO-Speicher
- **Null-Adress-Befehe** benutzen Daten, d. oben a.d. Stapel liegen, als Operanden o. als Adressen (fuer Hauptspeicher)
- Ergebnix -> **Top of Stack** (TOS)
- Berechnung e. arithmetischen Ausdrucks i.d. **umgekehrten Polnischen Notation** (Reverse Posish Notation, RPN)






----

----
**Backlinks:**
- [Rechenwerk](/rechenwerk)
