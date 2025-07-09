---
title: Interrupts
date: 2025-07-07 11:24
tags: 
---

----

### Definition
Signal a.d. [Prozessor](prozessor), d. ihn auffordert, seine akt. Taetigkeit **kurz zu unterbrechen**
**Interrupt Service Routine, ISR:** Als Reaktion a.e. Interrupt verzweigt d. Prozessor z.e. Programmteil,
d.a.d. eingetretene Ereignis reagiert

---

### Unterschied zu [Unterprogrammen](unterprogramme)
**Unterprogramme:** CALL-Befehl Ausloeser\
**Interrupts:** Intern o. extern erzeugte (Hardware)Signale Ausloeser

---

### Anwendungen
##### [Ein-/Ausgabe](io)
- Moeglichkeit: Busy-Waiting (Staendige Abfrage d. Zustands d. I/O)
- Wesentlich guenstiger: *Interrupt**-gesteuerte I/O
  - [Prozessor](prozessor) w. nur dann unterbrochen, w.d. I/O-Baustein bereit i., Daten zu senden o. zu empfangen

##### Betriebssystem
- I. Multitasking-Systemen schaltet d. Prozessor staendig zw. versch. Benutzern (bzw. Prozessen) um
- Nach Ablauf e. **Zeitscheibe** w. Zuteilung d. CPU durch e. *Interrupt* aufgerufen

##### Software-Interrupts
- Def: [Maschinenbefehl](maschinenbefehl), d.d. gleiche Wirkung h. wie durch Hardware ausgeloeste *Interrupts*

##### Traps und Exceptions
- **Fehler** w. durch e. geeignete Hardware erkannt, d.e. besonderen Interrupt ausloest
- Bsp:
  - Divide by Zero
  - Illegal Instruction
  - Speicherdefekt

---

### Verarbeitung eines Interrupts
[Einzelner_Interrupt](einzelner_interrupt)
[Mehrere_Interrupts](mehrere_interrupts)







----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
