---
title: Teileranzahlfunktion
date: 2025-06-21 00:53
tags: 
---

----

### Definition

Die Funktion $\tau:\mathbb{N}\to \mathbb{N}$, definiert durch $\tau(n)=\sum_{d\mid n}{1}$ fuer alle $n\in \mathbb{N}$

---

### Maple

`Divisors(n):` Auflistung der positiven Teiler einer natuerlichen Zahl $n$\
`tau(n):` Ordnung von `Divisors(n)`\
`SumOfDivisors(n,k):` Summe der $k$-ten Potenz aller positiven Teiler von $n$

---

### Satz 1

Sei $n\in \mathbb{N}, n>1$, und sei $n=p_{1}^{e_{1}}\cdots p_r^{e_r }$ die kanonische Primfaktorzerlegung von $n$. 
Dann gilt 
$$
  \tau(n)= \prod_{i=1}^{r}{(e_i+1)} 
$$

**Beweis**: Induktion nach $n$

---

### Korollar 1

Sei $n\in \mathbb{N}, n>1$. Dann gilt 
$$
  n \text{ ist Quadratzahl }\Leftrightarrow \tau(n) \text{ ungerade }
$$

**Beweis:** \
$\Rightarrow$: Sei $n$ eine Quadratzahl. Dann ist $n=a^{2}$ fuer ein $a\in \mathbb{N}$. Sei $p_{1}^{e_{1}}\cdots p_{r}^{e_r}$ die 
kanonische Primfaktorzerlegung von $a$. Dann ist die kononische Primfaktorzerlegung von $n=p_{1}^{2e_{1}}\cdots p_r^{{2e_r}}$. Mit Satz 1
folgt
$\tau(n)=\prod_{i=1}^{r}{2e_i+1}$. 
Somit ist jeder Faktor von $\tau(n)$ ungerade und folglich ist $\tau(n)$ auch ungerade.

$\Leftarrow$: Sei $\tau(n)$ ungerade und sei $n=p_{1}^{e_{1}}\cdots p_r^{e_r}$ die kanonische Primfaktorzerlegung
von $n$. Dann gilt $2\nmid \prod_{i=1}^{r}(e_{1}+1)$. Somit sind alle $e_{i}+1$ ungerade, das heisst, alle $e_{i},1\le i\le r$, sind gerade. Somit gilt $e_i=2f_i$, mit $f_i\in \mathbb{N}$.

---

### Korollar 2
Sei $n\in \mathbb{N},n>1$. Sei $p(n)$ das Produkt aller positiven Teiler von $n$. Dann gilt
$$
  p(n)=n^{\frac{\tau(n)}{2}} 
$$

**Beweis:** Seien $1=d_{1}<d_{2}<\cdots<d_{\tau(n)}=n$ die Teiler von $n$.
Dann gilt $d_{1}d_{\tau(n)}=n,d_{2}d_{\tau(n)-1}=n, \ldots$ Wir unterscheiden jetzt zwei faelle

i ) $\tau(n)$ ist gerade, also $\tau(n)=2t$ fuer ein $t\in \mathbb{N}$. Dann gilt
$$
  p(n)=d_{1}\cdot d_{2}\cdots d_{2t}=(d_{1}d_{2t})\cdots(d_t d_{t+1})=n^{t}=n^{\frac{\tau(n)}{2}}  
$$

ii ) $\tau(n)$ ist ungerade, also $\tau(n)=2t+1$ fuer ein $t\in \mathbb{N}$. Dann gilt 
$$
  p(n)=d_{1}\cdot d_{2}\cdots d_{2t+1} = (d_{1}d_{2t+1})\cdots (d_t d_{t_{t+2}}) d_{t+1}
$$
Mit Korollar 1 ist $n$ eine Quadratzahl, und $d_{t+1}=\sqrt{n}\in \mathbb{N}$. Es folgt $n^{t}\cdot \sqrt{n}=n^{t+\frac{1}{2}}=n^{\frac{\tau(n)}{2}}$







----

----
**Backlinks:**
- [📂Elementare_Zahlentheorie](/📁Elementare_Zahlentheorie)
