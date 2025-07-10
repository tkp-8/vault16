---
title: Mikroprogrammierung
date: 2025-07-07 11:26
tags: 
---

----

### Definition
Eine Architekturmoeglichkeit des [Leitwerks](leitwerk)\
Technik zur **Steuerrung der [CPU](prozessor)** ueber **vordefinierte [Mikrobefehl](mikrobefehle)-Sequenzen**\
Jeder [Maschinenbefehl](maschinenbefehl) w. durch e. zugehoeriges *Mikroprogramm* realisiert

---

### Eigenschaften
- Mikroprogramme bestehen aus Mikrobefehlen
- Gespeichert i.e. speziellen [Speicher](speicher):
  - **Mikroprogrammspeicher** (oft ROM o. PLA)
- **Ersetzt** fest verdrahtete Steuerlogik (Alternative zu hardwired control)
- Wesentlich langsamer als Hardware-Loesung

---

### Aufbau Mikroprogramm-[Steuerwerk](leitwerk)

![](img/mikroprogrammierung_1.png)
D. Befehlssatz e. Prozessors u.d. Faehigkeiten d. Rechenwerks w. durch Mikroprogramme miteinander verknuepft
- Zu jedem [Makrobefehl](maschinenbefehl) gibt es e. Bereich im Steuerwort-Speicher, d.d. zugehoerigen 
  Mikrobefehle enthaelt <- **Mikroprogramm**
- **Befehlssatz**: Menge saemtlicher Mikroprogramme
- Meistens fester Befehlssatz
- **Mikroprogramm-Steuerwerk**: Hardware-Interpreter fuer d. Maschinenbefehlssatz
- **Mikroassembler**: Symbolische **Sprache**, um Mikroprogramme zu entwickeln
- [Opcode](opcode) w.i. Befehlsregister abgelegt u. durch e. Schaltnetz i.d. **Startadresse** d. zugehoerigen Mikroprogramms umgeformt
- Steuerwort-Speicher w. ueber d. **Control Memory Address Register** (CMAR) adressiert (wie e. [Programmzaehler](befehlszaehler) fuer Makroprogramme)





----

----
**Backlinks:**
- [📂Rechnerarchitektur](/📁Rechnerarchitektur)
