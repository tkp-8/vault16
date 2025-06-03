---
title: CNF
date: 2025-05-10 01:04
tags: normalform 
---

----

### Definition 
##### Chomsky Normalform
Eine [kontextfreie Grammatik](kontextfreie_grammatiken) $G=(V,\Sigma,P,S)$ ist in 
Chomsky Normalform (CNF), falls sie ausschliesslich aus den Regeln
der folgenden Form besteht:

1. $A\to XY$ wobei $A,X$ und $Y$ Variablen sind, $X$ und $Y$ sind jedoch 
nicht $S$
2. $A\to x$, wobei $A$ Variable und $x$ Terminalsymbol
3. $S\to \varepsilon$

---

### Beispiel

$$
  \begin{align*}
    S&\to AA\mid AB\mid b\mid \varepsilon \\
    A&\to BB\mid a\\
    B&\to b
  \end{align*}
$$

---

### Satz
##### Zu jeder [kontextfreien Sprache](kontextfreie_sprachen) $L$ gibt es eine kontextfreie Grammatik $G$ in CNF, sodass $L(G)=L$
**Beweis.** Jede kontextfreie Grammatik laesst sich wie folgt in CNF umwandeln.

---

### Umwandlung
1. **Eliminiere Regeln mit $S$ auf rechter Seite** 
 
- Ersetze $S$ mit $S^\prime$
- Neue Regel: $S\to S^{\prime}$

2. **Eliminiere jede Regel der Form $A\to \varepsilon$ mit $A\neq S$**

- Streiche $A\to \varepsilon$
- Aendere jede Regel mit $A$ auf der rechten Seite $X\to uAw, \ u,w\in (\Sigma \cup V)^{*}$ 
zu $X\to uAw\mid uw$ 

3. **Eliminiere jede Regel der Form $A\to B$** 

- Streiche $A\to B$
- Fuege fuer jede Regel der Form $B\to w$ eine Regel $A\to w$ ein 
  
4. **Eliminiere jede Regel mit langer rechter Seite**

- Sei $A\to x_{1}x_{2}\ldots x_n, \quad x_i\in V\cup \Sigma$ eine Regel mit mehr als 2 Zeichen auf der rechten Seite
- Seien $X_{1},X_{2},\ldots X_{n-2}$ neue Variablen
- Fuege folgene Regeln hinzu
$$
  \begin{align*}
    A&\to x_{1}X_{1}\\
    X_{1}&\to x_{2}X_{1}\\ 
    & \vdots \\
    X_{n-2}&\to x_{n-1}x_n
  \end{align*}
$$

5. **Eliminiere jede Regel mit Terminalsymbolen auf der rechten Seite, ausser
sie hat die Form $X\to a$**

- Neue Variable $V_x$ fuer jedes Terminalsymbol $x$
- Neue Regel $V_x\to x$






----

----
**Backlinks:**
- [Kontextfreie Grammatiken](/kontextfreie_grammatiken)
