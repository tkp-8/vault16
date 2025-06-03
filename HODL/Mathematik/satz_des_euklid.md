---
title: Satz_des_Euklid
date: 2025-05-03 12:40
tags: 
---

----

### Satz 
##### Es gibt unendlich viele Primzahlen.

---

### Beweis
**Verfahren:** Indirekter Beweis 

Annahme: Es gaebe nur endlich viele Primzahlen. Nennen wir diese $p_{1},\ldots,p_r$.

Wir bilden 
$$
  n = p_{1}\cdot p_{2}\cdots p_{r-1}\cdot p_r +1
$$
Nach der [Primteilerexistenz](primteilerexistenz) ist jede natuerliche Zahl $n$ durch
eine Primzahl teilbar. Da es nur endlich viele Primzahlen gibt, muss p 
eine der $p_{1},\ldots, p_r$ sein. Dann gilt 
$$
  p\mid n \text{ und } p\mid (p_{1}\cdot p_{2}\cdots p_r), \text{ also } p\mid (n-p_{1}\cdot p_{2}\cdots p_r)
$$
Es gilt also $p\mid 1$. Dies ist ein Wiederspruch, denn $p>1$. Die Annahme ist falsch gewesen und 
daraus folgt die Behauptung.





----

----
**Backlinks:**
- [Primzahlen](/primzahlen)
