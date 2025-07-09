---
title: Busse
date: 2025-07-07 11:20
tags: 
---

----

### Definition
**Buendel** v. Leitungen, d. mehrere Komponenten e. [Computers](computer) ermoeglicht, 
Daten ueber e. **gemeinsame Verbindung** auszutauschen

---

### Funktion
- Zeitlich versetzte Nutzung (**Zeitmultiplex**) reduziert ges.Zahl d. Leitungen
- **Birektionale** Schaltung m. Hilfe v. Adress- u. Steuerleitungen, 
  d. Bustreiber (z.B. TriState) o. el. Schalter (CMOS-Transmission Gates) ansteuern

---

### Interner Datenbus
- A.d. **Maschinenwortbreite** ausgelegt
- K.v. zwei verschiedenen Datenquellen angesteuert w.
- Moegliche Quellen: 
  - Rechenwerksregister  
  - *Externer Datenbus*

---

### Externer Datenbus
- **Nicht** immer a.d. volle Maschinenwortbreite ausgelegt, um Anz. Pins zu minimieren
- Ueber bidirektionale Bustreiber a.d. internen Datenbus angekoppelt

---

### Interner Steuerbus
- **Interne Steuerleitungen** bilden zsm. m.d. Zustandsflags d. [Rechenwerks](rechenwerk) den *internen Steuerbus*

---

### Bustreiber
- Verstaerken Steuersignale u. Adressen f.d. externe Bussystem
- Erhoehen d. Zahl d. anschliessbaren **Schaltglieder**
- Richtung d. Datenuebertragung w. durch **R/W-Steuerleitung** (1 f. Read/0 f. Write) bestimmt
- Dritter Zustand d. Ausgangs: **hochohmiger** Zusand, Ausgang v.d. Busleitung abgekoppelt

---

### Systembus
- Gesamtheit v. **externem Adress-, Daten- u. Steuerbus**
- Realisierung v. Mikrochips



---

![](img/busse_1.png)






----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
