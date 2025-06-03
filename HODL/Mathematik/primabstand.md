---
title: Primabstand
date: 2025-05-04 06:41
tags: 
---

----

### Proposition
##### Sei $k$ eine beliebige, fest vorgegebene natuerliche Zahl. Dann gibt es eine natuerliche Zahl $n$, sodass $n+1,n+2,\ldots,n+k$ [zusammengesetzte Zahlen](zusammengesetzte_zahlen) sind.

---

### Beweis

Setze $n=2\cdot 3\cdots (k-1)\cdot k\cdot (k+1)+1$. Dann gilt
$$
  \begin{align*}
    n&+1 = 2\cdot 3\cdots (k-1)\cdot k\cdot (k+1)+2 \implies 2\mid n+1\\
    &\; \; \vdots \\
    n&+k = 2\cdot 3\cdots (k-1)\cdot k\cdot (k+1)+(k+1) \implies (k+1)\mid n+k\\
  \end{align*}
$$
Es folgt, dass $n+1,n+2,\ldots n+k$ zusammengesetzte Zahlen sind.







----

----
**Backlinks:**
- [Primzahlen](/primzahlen)
