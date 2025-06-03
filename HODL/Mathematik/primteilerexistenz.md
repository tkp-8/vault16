---
title: Primteilerexistenz
date: 2025-05-03 12:05
tags: 
---

----

### Lemma
##### $\forall n \in \mathbb{N}, n \ge 2 \ \exists p \in \mathbb{P}: p \mid n$  

---

### Beweis
**Verfahren:** Vollstaendige Induktion 

Induktionsanfang:\
Die Aussage gilt fuer $n_{0}=2$, da $2 \in \mathbb{P}$ und $2 \mid 2$.

Induktionsannahme:\
Wir nehmen an, dass $n \ge 2$ ist, und dass jede Zahl $r$ mit $2\le r\le n$ durch
eine Primzahl teilbar ist .

Induktionsschritt:\
Wir zeigen, dass $p\mid n+1$. Wenn $n+1$ selbst eine Primzahl ist, sind wir fertig. 
Also koennen wir annehmen, dass $n+1$ eine zusammengesetzte Zahl ist und somit 
mindestens einen echten Teiler $2\le d \le  n$ besitzt. Nach der Annahme ist solch eine 
Zahl durch eine Primzahl teilbar. Es folgt $p\mid d$ und $d\mid n+1$, also $p\mid n+1$.

Mit dem Prinzip der vollstaendigen Induktion folgt die Behauptung.


----
**Backlinks:**
- [Primzahlen](primzahlen)
