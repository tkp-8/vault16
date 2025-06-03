---
title: CYK-Algorithmus
date: 2025-05-10 02:28
tags: algorithmus 
---

----

### Zweck

- Wortproblem fuer [kontextfreie Sprachen](kontextfreie_sprachen) loesen
- Entscheidet ob [Wort](woerter) $w\in L(G)$
- Nur fuer [kontextfreie Grammatiken](kontextfreie_grammatiken) in [CNF](cnf)

---

### Eingabe

- Wort $w=w_{1},w_{2},\ldots ,w_n$
- Grammatik $G=(V,\Sigma,P,S)$

---

### Ausgabe

- $true/false$, ob $w\in L(G)$

---

### Initialisierung

- Sei $w[j,j]$ das Teilwort von $w$, welches mit dem $i$-ten Zeichen beginnt und 
  mit dem $j$-ten Zeichen endet.
$$
  W_{i,j}\coloneqq \{X\in V\mid X\Rightarrow ^{*} w[i,j]\}  
$$
- Das Wortproblem reduziert sich darauf, zu testen, ob $S \in W_{1,n}$

---

### Iteration

**Rekursiver Ansatz**

**$j=i$:**\
 
- Da CNF, kann es nur die Regel der Form $A\to w[i,i]$ geben
$$
  W_{i,i}=\{A\in V\mid \text{ es gibt die Regel } A\to w[i,i]\}  
$$

**$j>i$:**\

- Regel der Form $A\to XY$ wurde als erstes angewendet
$$
  A\Rightarrow XY\Rightarrow \cdots \Rightarrow w[i,j]
$$

- Da es fuer $A\neq S$ keine Regeln $A\to \varepsilon$ gibt, muss $X\Rightarrow ^{*}u$ 
  und $Y\Rightarrow ^{*} v$ folgen, mit $w[i,j]=uv$
- **Aufteilung** von $w[i,j]$ in zwei nichtleere Teilwoerter
$$
  W_{i,j}=\bigcup_{t = i}^{j-1}\{A\in V\mid \text{es gibt die Regel }A\to XY \text{ und } 
X\Rightarrow ^{*}w[i,t] \text{ und } Y\Rightarrow ^{*}w[t+1,j]\}    
$$
- Wir koennen davon ausgehen, dass $W_{i,t}$ und $W_{t+1,j}$ schon bestimmt wurden
$$
  W_{i,j}=\bigcup_{t = i}^{j-1}\{A\in V\mid \text{es gibt die Regel }A\to XY \text{ und } 
X\in W_{i,t} \text{ und } Y\in W_{t+1,j}\}
$$

---

### Algorithmus


`Algorithmus 1: CYK-Algorithmus`

// Initialisierung \
**01** **for** $i=1$ to $n$ **do** $W[i,i]=\{A\in V \mid A \to w[i,i]\}$\
  // Iteration\
**02** **for** $d=1$ **to** $n-1$ **do**\
**03** $\cdot \ \cdot$ **for** $i=1$ **to** $n-d$ **do**\
**04** $\cdot \cdot \cdot \ \cdot$ $j=i+d$ \
**05** $\cdot \cdot \cdot \ \cdot$ **for** $t=i$ **to** $j-1$ **do**\
**06** $\cdot \cdot \cdot \cdot \cdot \ \cdot$ **for all** $A\to XY\in P$ **do**\
**07** $\cdot \cdot \cdot \cdot \cdot \cdot \cdot \ \cdot$ **if** $X\in W[i,t]$ **and**
$Y\in W[t+1,j]$ **then** $W[i,j]=W[i,j]\cup \{A\}$ \
**08** $\cdot \cdot \cdot \cdot \cdot \ \cdot$ **end**\
**09** $\cdot \cdot \cdot \ \cdot$ **end**\
**10** $\cdot \ \cdot$ **end**\
**11** **end**\
**12** **if** $S\in W[1,n]$ **then return** $true$ **else return** $false$




----

----
**Backlinks:**
- [Kontextfreie Sprachen](/kontextfreie_sprachen)
