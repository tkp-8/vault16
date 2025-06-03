---
title: Grammatiken
date: 2025-05-09 07:23
tags: 
---

----

### Definition
##### Grammatik
Eine Grammatik $G$ ist ein 4er-Tupel $G = (V,\Sigma,P,S)$ wobai gilt:

> - $V$ ist eine endliche Menge von Variablen
> - $\Sigma$ ist eine endliche Menge von Terminalsymbolen. Dabei gilt $V\cap \Sigma\neq \empty$
> - $P\subseteq \{(L,R)\mid L,R\in (V\cup \Sigma)^{*}\}$ ist eine endliche Menge von Produktionsregeln 
> - $S\in V$ ist das Startsymbol

##### Mehrdeutige Grammatik
Eine Grammatik, zu der es mehrere Ableitungsbaeume gibt

---

### Notation
**Produktionsregel**\
$\alpha \to \beta$: $\alpha$ kann ersetzt werden durch $\beta$\
$\alpha\to \beta\mid \gamma\mid \delta$: Bei mehreren Regeln

**Ableitungsschritt**\
$w\Rightarrow v$: tatsaechliche Anwendung einer Produktionsregel auf ein Wort,
wenn es eine Regel $a\to \beta \in P$ gibt \
$w\Rightarrow ^{*}v$: Sequenz von Ableitungen 

---

### Konzept
- Beschreibung des Aufbaus von [Sprachen](sprachen) durch Produktionsregeln
- Menge von Regeln, die beschreiben, wie man aus einem Symbol durch das wiederholte Ersetzen
von Teilwoertern ein [Wort](woerter) konstruieren kann
- Auch fuer komplexe Strukturen
- Gaengig fuer die Beschreibung von Programmiersprachen

---

### Klassifizierung
##### Chomsky-Hierarchie
 
- allgemein (Typ 0)
- kontextsensitiv (Typ 1)
- [kontextfrei](kontextfreie_grammatiken) (Typ 2)
- regulaer (Typ 3)




----

----
**Backlinks:**
- [📂Formale Sprachen Grammatiken Automaten](/📁Formale_Sprachen%linkAutomaten)
