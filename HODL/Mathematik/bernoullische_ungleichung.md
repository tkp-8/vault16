---
title: Bernoulli'sche Ungleichung
date: 2025-06-02 11:28
tags: 
---

----

### Satz 
Fuer alle $x\in \mathbb{R}$ mit $x\ge -1$ und alle $n\in \mathbb{N}$ gilt  
$$
  (1+x)^{n}\ge 1+nx 
$$

---

### Beweis
**Verfahren:** Vollstaendige Induktion nach $n$\
Induktionsanfang: Fuer $n=1$ gilt $(1+x)\ge 1+x$ fuer alle $x\in \mathbb{R}$\
Induktionsannahme: Wir nehmen an, dass die Behauptung schon fuer ein $n\ge 1$ bewiesen ist\
Induktionsschritt: Da $1+x\ge 0$, folgt aus dem [Monotoniegesetz](ordnungsaxiome) $(1+x)^{n}(1+x)\ge (1+nx)(1+x)$ also
$$
  (1+x)^{n+1}\ge 1+(n+1)x+nx^2  
$$
Da $x^2\ge 0$ und da n>0, folxt $nx^2\ge 0$. Es ist $1+(n+1)x+nx^2\ge 1+(n+1)x$, also $(1+x)^{n+1}\ge 1+(n+1)x$.







----

----
**Backlinks:**
- [Ordnungsaxiome](/ordnungsaxiome)
