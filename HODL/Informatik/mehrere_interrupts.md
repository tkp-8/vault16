---
title: Mehrere_Interrupts
date: 2025-07-09 00:41
tags: 
---

----

### Grundfunktion
[Einzelner_Interrupt](einzelner_interrupt)

---

### Probleme
1. Jedem [Interrupt](interrupts) muss e. eig. Startadresse f.d. Service-Routine zugeordnet w.
2. Wenn mehrere Interrupts gleichzeitig *haengend* s., muss e. Entscheidung getroffen w., welcher 
   Interrupt vorrangig bearbeitet w.

---

### Maskierbarkeit
1. Maskierbare Interrupts
    - Koennen v. Programmierer **freigegeben** o. **gesperrt** w. 
    - Sperren, w. Anwendung zeitkritisch
2. Nicht-maskierbare Interrupts (Non Maskable Interrupts, **NMI**)
    - Koennen **nicht gesperrt** w.  
    - Fehlerbehandlung u. muessen unverzueglich bearbeitet w. 
    - Bsp: Abfall d. Betriebsspannung, Traps
  
---

### Methoden zur Bestimmung Startadresse
Um d. Startadresse d. Service-Routine zu bestimmen, gibt es drei Moeglichkeiten:

##### Abfragemethode (Polling)
Vorteil: 

- Geringster Hardwareaufwand 
- Am [Prozessor](prozessor) nur e. Interrupt-Eingang noetig
 
Nachteil: 

- Hoher **Zeitbedarf** z. Abfrage d. einzelden I/O-Bausteinen

Ablauf:

1. IRQ d. einzelnen I/O-Bausteine w. durch e. **OR-Funktion** verknuepft, d. diesen einzelnen Eingang IRQ steuert
2. Eingang IRQ, d. alle Interrupts verwaltet: **Interrupt Handler** 
3. Wenn e. haengende IRQ erkannt w., w.d. laufende Programm unterbrochen, indem d. CPU d. Service-Routine (Interrupt Handler) aufruft
4. Ermittlung d. Interrupt-Quelle
    - Lesen d. [Statusregister](statusregister) d. einzelnen I/O-Bausteine u. Pruefen, ob **Interrupt-Flag** gesetzt
    - Interrupt Handler **kennt** d. Startadressen d. Service-Routinen f. jeden einzelnen Baustein
    - Flag positiv -> **unbedingter Sprung** zu d. zugeordneten Service-Routine
    - **Prioritaet** bestimmt Reihenfolge d. Abfrage
5. Abschliessen d. *Device Handler-Programm* m.d. **RETI**-Befehl

##### Vektormethode (vectored Interrupts)
Vorteil: 

- **Schnelle** Beantwortung v. Interrunpt-Anforderungen
- **Startadresse** d. Device Handlers spaetestens n.e. Befehlszyklus bekannt
 
Nachteil: 

- Groesster Hardwareaufwand
- F. jede moegliche Interrupt-Anforderung e. eigener Eingaenge an CPU noetig
- Nur ein Device Handler pro Anforderungsleitung
 
Ablauf:

1. Interrupt-Anforderungen w.i.e. besonderen Register **ISRQ** (Interrupt Service REQuest) aufgefangen
2. Sie w.m.e. **Interrupt-Maske** *IM*, d. Bestandteil d. Statusregisters ist, bitweise **AND**-verknuepft
3. Freigegebener Interrupt w. erkannt -> Ablaufsteuerung der betreffenden Anforderungsleitung k.e. Maschinenbefehl zuordnen 
4. Maschinenbefehl legt implizit d. Startadresse f.e. Service-Routine fest

##### Codemethode
Vorteil:

- Hohes Mass an **Flexibilitaet**

Ablauf:

1. Jeder Anforderungsleitung $IRQ_i$ w.e. Quittungssignal $INTA_i$ zugeordnet
2. I/O-Baustein enthael auf e. Interrupt-Anforderung hin e. Quittungssignal -> antwortet m.e. **Codewort** aud d. [Datenbus](busse)
3. Aus d. Codewort w.d. Startadresse d. gewuenschten Device Handlers bestimmt

---

### Interrupt-Controller (Festlegung Prioritaeten)
A.d. Chip integriete Hardware-Loesung, um **Prioritaeten** festzulegen

##### Interrupt-Tabelle
Tabelle, i.d.d Startadressen abgelegt sind
![](img/interrupt_2)

##### Aufbau
![](img/interrupt_3)

##### Ablauf
1. Wenn alle Interrupts freigegeben (IM=1111) -> haengende Anforderungen i. ISQR gelangen z.e. *Prioritaetsencoder*
2. Nummer d. Anforderung **hoechster Prioritaetw.v. Prioritaetsencoder als Dualzahl ausgegebe 
3. Code w.m.d. **Interrupt-Status-bits** *IS* d. Statusregisters verglichen (IS gibt d. **Prioritaetsebene** an, i.d.s.d. Prozessor gerade befindet)
4. Falls Prioritaetscode $A > IS$ -> Anforderung m.d. hoechsten Prioritaet w. akzeptiert u. bearbeitet:
    1. M. Hilfe d. Prioritaets-Codes w.d. Startadresse d. Service-Routine n.e.d. o.g. **Methoden** bestimmt u.d. passende $INTA_i$-Signal w. ausgegeben
    2. **Ruecksprungadresse** w. zsm. m.d. alten IS-Code (Statusregister) a.d. **Stapel** gelegt
    3. Startadresse d. Service-Routine w.i.d. [Befehlszaehler](befehlszaehler) geladen -> IS-Teil d. Statusregisters w.m.d. **akt. Prioritaetscode** ueberschrieben
    4. Abarbeitung d. **Service-Routine** -> Abschliessen m.e. RETI-Befehl (stellt d. alte Statusregister wiederher, bewikt e. Rueckkehr i.d. unterbrochene Prioritaetsebene)



----

----
**Backlinks:**
- [Interrupts](/interrupts)
