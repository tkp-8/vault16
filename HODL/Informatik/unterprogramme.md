---
title: Unterprogramme
date: 2025-07-08 10:50
tags: 
---

----

### Definition
(Engl: Subroutine)\
**Abgeschlossenes Teilprogramm**, d.e. bestimmte Aufgabe uebernimmt

---

### Funktion
- Mehrmals verwendete Funktionen k. als *Unterprogramme* zusammengefasst w.
- **Modularisierte** Programmierung
- Eingabewert als **Parameter** d. Unterprogramms
- W.m.d. *CALL*-Befehl aufgerufen
- W.m.d. *RETURN*-Befehl abgeschlossen

---

### (Laufzeit-)Bibliothek
**Sammlung** v. haeufig benoetigten Unterprogrammen

---

### CALL-Befehl
**Programmverzweigung i.d. Unterprogramm**
1. CALL-Befehl w. geholt 
2. **[Programmzaehler](befehlszaehler)** w. inkrementiert 
$$
  PC++
$$
3. **Verzweigungsadresse** (Startadresse d. Unterprogramms) w.i.e. zus. Adressregister $AR$ gerettet
$$
  AR\leftarrow Ziel
$$
4. **Ruecksprungadresse** w.a.d. Stapel gelegt 
$$
  SP\leftarrow SP-1\\
  M[SP] \leftarrow PC 
$$
5. **Startadresse** d. Unterprogramms w.a.d. Adressregister i.d. Programmzaehler geladen
$$
  PC\leftarrow AR
$$

---

### RETURN-Befehl
(Return from Subroutine, RTS)\
Umkehrung v. Schritt 4 d. CALL-Befehls
$$
  PC \leftarrow M[SP]\\
  SP \leftarrow SP+1
$$

---

### [Rekursion](rekursion)
M.s.v.e. *Rekursion*, w.s. Unterprogramme selbst o. gegenseitig aufrufen

---

### Zeitbedarf
- Dynamischer Aufbar e. Verbindung zwischen d. Haupt- u. Unterprogramm erhoeht d. Zeitbedarf
- Preis f.d. eingesparten Speicherplatz
- **Alternative b. zeitkritischen anwendungen:** [Makros](makros)



----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
