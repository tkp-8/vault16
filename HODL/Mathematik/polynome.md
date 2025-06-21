---
title: Polynome
date: 2025-06-21 10:48
tags: 
---

----

### Definition 

##### Polynom 
Sei $\mathbb{K}$ ein Koerper. Ein *Polynom* ueber $\mathbb{K}$ in der Unbestimmten $T$ hat die Form
$$
    a_{0}T^{0}+a_{1}T^{1}+\cdots+a_nT^{n}=\sum_{i=0}^{n}a_iT^{i}     
$$
Die Menge aller Polynome ueber $\mathbb{K}$ wird mit $\mathbb{K}[T]$ bezeichnet

##### Koeffizient
$a_{0},\ldots ,a_n\in \mathbb{K}$

##### Nullpolynom
Wenn alle Koeffizienten eines Polynoms $0$ sind

##### Grad
Sei $p=\sum_{i=0}^{n}{a_iT^{i}}$ ein Polynom in $\mathbb{K}[T]$, und sei $p$ nicht das Nullpolynom. 
Dann gibt es einen Koeffizienten $a_i$, der nicht $0$ ist. Sei $m$ der groesste Index, so dass der Koeffizient 
$a_m\neq 0$ ist. Wir nennen $m$ den *Grad* von $p$ und schreiben $\text{Grad}(p)=m$.
Nullpolynom: $\text{Grad(0)}=-\infty$

---

### Produkt
##### Definition
Seien $p=\sum_{i=0}^{n}{a_iT^{i} }$ und $q=\sum_{i=0}^{m}{b_iT^{i} }$ Polynome in $\mathbb{K}[T]$. Wir 
definieren das *Produkt* $pq$ durch 
$$
  pq=\sum_{k}c_kT^{k} \text{ mit } c_k=\sum_{i+j=k}{a_ib_j} 
$$

##### Gradformel 
Seien $p=\sum_{i=0}^{n}{a_iT^{i} }$ und $q=\sum_{i=0}^{m}{b_iT^{i} }$ Polynome in $\mathbb{K}[T]$ mit $\text{Grad}(p)=n\ge 0$ und 
$\text{Grad}(q)=m\ge 0$. Dann gilt $\text{Grad}(pq)=n+m$

---

### Nullstellen

---

### [Polynomfunktionen](polynomfunktionen)




----

----
**Backlinks:**
- [Polynomfunktionen](/polynomfunktionen)
