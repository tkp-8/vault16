---
title: Regulaere Sprachen
date: 2025-05-07 05:42
tags: 
---

----

### Definition

Jede der folgenden Bedingungen ist aequivalent zur Regularitaed einer [Sprache](sprachen) 
$L$
 
- es gibt einen sie definierenden [regulaeren Ausdruck](regulaerer_ausdruck) 
- Es gibt einen [endlichen Automaten](endliche_automaten), der die Sprache akzeptiert 
- $L$ wird von einer regulaeren Grammatik erzeugt
$$
  REG \coloneqq \{L\mid L\text{ ist regulaer}\}  
$$

---

### Satz 1
##### Jede endliche Sprache ist regulaer
**Beweis.** Sei $L\subseteq \Sigma ^{*}$ eine endliche Sprache. $l$: laengstes
Wort, $\Sigma=\{\texttt{a},\texttt{b}\}$ \
Wir muessen zeigen, dass es einen [DEA](dea) $M$ fuer $L$ existiert.\

- Grundstruktur des Zustandsdiagramms entspricht einem [binearen Baum](binaerer_baum)
    - Tiefe $l$ 
    - von einem inneren Knoten gibt es zweit Kanten: $\texttt{a}$ und $\texttt{b}$
    - Wurzel: Startzustand 
- fuer jeden Knoten existiert genau einen Pfad von der Wurzel
- Zustand $q_w$, wenn $w$ das [Wort](woerter), das man lesen muss, um ihn zu erreichen
- $F=\{q_w\mid w\in L\}$
- **Muellzustand** $q_-$ fuer $|w|>l$
- **Allgemein:** $k$-aerer Baum mit $k=|\Sigma|$

---

### Satz 2 
##### Sei $L$ eine regulaere Sprache, dann existiert ein regulaerer Ausdruck $R$ mit $L(R)=L$
**Beweis.** [Satz von Kleene](satz_von_kleene)

---

### Abschlusseigenschaften
##### Die regulaeren Sprachen $REG$ sind unter folgenden Operationen abgeschlossen

- **Vereinigung**\
**Beweis.** Verfahren: Produktautomat.\
Seien $L_{1},L_{2}$ regulaere Sprachen mit den zugehoerigen DEAs $M_{1}, M_{2}$. 
Wir konstruieren einen DEA $M_{3}=(Q_{3},\Sigma,\delta_{3},q_{3},F_{3})$, der 
die Sprache $L(M_{3})=L_{1}\cup L_{2}$ akzeptiert. Wir lassen $M_{1}$ und $M_{2}$ gleichzeitig
durch $M_{3}$ ausfuehren lassen, indem wir $M_{3}$ in einem Zustandsraum von $Q_{3}\coloneqq Q_{1}\times Q_{2}$ laufen
lassen. Der Startzustand von $M_{3}$ ist $q_{3}=(q_{1},q_{2})$.\
Wir definieren die Uebergangsfunktion als 
$$
  \forall (p,q)\in Q_{3} \ \forall a\in \Sigma: \quad \delta_{3}((p,q),a)\coloneqq (\delta_{1}(p,a),\delta_{2}(q,a)).
$$
Als Letztes legen wir die Menge $F_{3}$ fest.
$$
  F_{3}\coloneqq \{(p,q)\in Q_{3}\mid p \in F_{1} \text{ oder } q \in F_{2}\}  
$$
**Alternativer Beweis:** NEA Konstruktion.
![](img/reg_1.png)

- **Konkatenation** \
**Beweis.** Verfahren: NEA Konstruktion. \
Seien $L_{1},L_{2}$ regulaere Sprachen mit den zugehoerigen DEAs $M_{1}, M_{2}$. 
Wir konstruieren einen NEA $N$, 
welcher die Sprache $L(M_{3})=L_{1}\circ L_{2}$ akzeptiert. Fuer jeden akzeptierten 
Zustand von $M_{1}$ fuegen wir einen $\varepsilon$-Uebergang zum Startzustand von $M_{2}$ 
hinzu. \
Als akzeptierende Zustaende von $N$ waehlen wir nur die akzeptierenden Zustaende von $M_{2}$\

- **Kleene Stern** \
**Beweis.** Verfahren: NEA Konstruktion. \
Sei $L\in REG$ und $M$ ein DEA, welcher $L$ akzeptiert. Wir fuegen 
einen neuen Startzustand ein, der gleichzeitig ein akzeptierender Zustand ist, da 
$\varepsilon \in L^{*}$. Wir verbinden den neuen Startzustand mit einem 
$\varepsilon$-Uebergang zum alten Startzustand und zusaetzlich fuehren wir $\varepsilon$-Uebergaenge
von den akzeptierenden Zustaenden zum neuen Startzustand ein.









----

----
**Backlinks:**
- [Endliche Automaten](endliche_automaten)
