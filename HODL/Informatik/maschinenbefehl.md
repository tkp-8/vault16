---
title: Maschinenbefehl
date: 2025-07-08 04:12
tags: 
---

----

### Definition
(Auch: Makrobefehl)\
Codierte **Anweisung** a.d. [CPU](prozessor), e. spezifische **Operation** auszufueren\
Besteht a. *[Opcode](opcode)* u. *Adressfeld*

---

### Befehlsformate
##### Ein-Wort-Befehle
- Wenn d. Operanden i. Rechenwerkregistern stehen
- [CISC](cisc) u. [RISC](risc)
- (Opcode, Adressfeld)

##### Mehr-Wort-Befehle 
- Wenn d. Operanden o. Daten direkt i. [Speicher](speicher) abgelegt sind
- Befehl a. zwei o. derei Maschinenwoertern
- Ausschliesslich bei [CISC](cisc)
- Bsp. Format: (Opcode, Adresse 1. Op, Adresse 2. Op, Adresse Ergebnis)

---

### Beziehung zu [Mikrobefehlen](mikrobefehle)
- E. Maschinenbefehl -> umgesetzt durch **mehrere Mikrobefehle**
- Mikrobefehle steuern
  - Registertransfer
  - [ALU](alu)-Operationen
  - Buszugriffe
- Umsetzung erfolgt durch [Leitwerk](leitwerk) d. CPU
  - entweder **fest verdraht** 
  - oder [mikroprogrammiert](mikroprogrammierung)



----

----
**Backlinks:**
- [Opcode](/opcode)
