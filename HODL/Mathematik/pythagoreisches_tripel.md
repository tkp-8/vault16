---
title: Pythagoreisches Tripel
date: 2025-06-14 01:35
tags: 
---

----

### Definition
**Pythagoreisches Tripel**\
Loesung $(a,b,c)$ mit $a,b,c\in \mathbb{N}$ von $X^2+Y^2=Z^2$

**Primitiv**\
Wenn Pythagoreisches Tripel $(a,b,c)$ mit $\text{ggT}(a,b)=1$

---

### Eigenschaften 

**Lemma 1:** Sei $(a,b,c)$ eine Pythagoreisches Tripel. Sei $d=\text{ggT}(a,b)$. Dann ist $(\frac{a}{d},\frac{b}{d},\frac{c}{d})$ 
ebenfalls ein Pythagoreisches Tripel\
**Beweis:** Da $a^2+b^2=c^2$, folgt $d^2\mid c^2$, also $d\mid c$. Somit gilt $\frac{a}{d},\frac{b}{d},\frac{c}{d}\in \mathbb{N}$. 
Da auch $(\frac{a}{d})^2+(\frac{b}{d})^2 =(\frac{c}{d})^2$, ist $(\frac{a}{d},\frac{b}{d},\frac{c}{d})$ ein Pythagoreisches Tripel

**Lemma 2:** Wenn $(a,b,c)$ ein *primitives* Pythagoreisches Tripel ist, dann sind $a,b,c$ paarweise teilerfremd\
**Beweis:** $\text{ggT}(a,b)=1$, nach Def. Sei $d=\text{ggT}(a,c)$. Angenommen $d>1$. Sei $p$ eine Primzahl, die $d$ teilt.
Dann gilt $p\mid a^2$ und $p\mid c^2$, also $p\mid b^2$. Da $p$ eine Primzahl ist, folgt $p\mid b$. 
Somit gilt $p\mid a$ und $p\mid b$, ein Widerspruch zu $\text{ggT}(a,b)=1$. Analog wird gezeigt, dass
$\text{ggT}(b,c)=1$ ist 

**Lemma 3:** Ist $(a,b,c)$ ein *primitives* Pythagoreisches Tripel, so ist genau eine der Zahlen
$a$ oder $b$ gerade.

**Lemma 4:** Wenn $(a,b,c)$ ein *primitives* Pythagoreisches Tripel ist, dann ist $c$ ungerade\
**Beweis:** Nach Lemma 3 ist die Summe von $a^2$ und $b^2$ eine ungerade Zahl. Also ist $c^2$ ungerade und somit ist 
$c$ ebenfalls ungerade








----

----
**Backlinks:**
- [📂Elementare_Zahlentheorie](/📁Elementare_Zahlentheorie)
