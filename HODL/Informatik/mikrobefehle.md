---
title: Mikrobefehle
date: 2025-07-10 07:16
tags: 
---

----

### Definition
(Auch: Steuerwoerter)\
Interne Steueranweisung **innerhalb** d. [Prozessors](prozessor), d.e. Teil e. [Maschinenbefehls](maschinenbefehl)
realisiert\
Steuert **direkt** einzelne funktionale Einheiten, wie Registertransfer, [ALU](alu)-Operationen o. Buszugriffe

---

### Eigenschaften
 
- **Nicht sichtbar** fuer Programmierer
- Organisiert i. [Mikroprogramme](mikroprogrammierung)
- Realisierung durch [Leitwerk](leitwerk)
  - entweder fest verdraht
  - oder mikroprogrammiert

---

### Befehlsformat
Mikrobefehle enthalten nicht nur Steuerbits, sondern auch Information zur **Adresserzeugung**
f.d. Mikrobefehlszaehler \
Zwei Teile e. Mikrobefehls:

1. Steuerwort zur Auswahl d. Operationen i. Rechenwerk
2. Adressauswahlwort, um d. Adresse d. naechsten Mikrobefehls festzulegen

- Mikrobefehle sind codiert, da e. geringer Prozentsatz d. moeglichen Steuerwoerter sinnvoll
- Steuerwort w.i. mehrere voneinander unabhaengige Felder unterteilt
- Jedes Feld codiert e. Mikrooperation 

**Klassifikation**\
Horizontale Mikrobefehle: 
 
- Viele Steuer-Bits 
- Hohe Zahl paralleler Mikrrooperationen

Vertikale Mikrobefehle:

- Nur ein Steuerfeld
- Hoher Dekodierungsaufwand
- Eine einzige Mikrooperaition pro Taktzyklus






----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
