---
title: Zusammengesetzte_Zahlen
date: 2025-05-04 00:38
tags: 
---

----

### Definition 
$n$ ist eine zusammengesetzte Zahl, wenn $n\in \mathbb{N}\setminus\mathbb{P}$

---

### Eigenschaften
**Lemma 1:** Sei $n \in \mathbb{N}$ eine zusammengesetze Zahl. Dann hat n einen Teiler d, mit $1<d\le \sqrt{n}$\
**Beweis:** $n$ ist eine zusammengesetzte zahl $\Leftrightarrow n=d_{1}d_{2}$ mit $d_{1},d_{2}\in \mathbb{N}$ beide 
groesser als 1. Falls beide groesser als $\sqrt{n}$ sind, so folgt $n=d_{1}d_{1}>\sqrt{n}\sqrt{n}=n$, also
$n>n$ und dies ist ein Widerspuch.

**Lemma 2:** Sei $n\in \mathbb{N}$ eine zusammengesetzte Zahl. Dann hat $n$ einen Primteiler $p$
mit $1<p\le \sqrt{n}$\
**Beweis:** Mit Lemma 1 hat n einen Teiler d mit $1<d\le \sqrt{n}$. Nach der [Primteilerexistenz](primteilerexistenz) 
hat $d$ einen Primteiler $p$. Es gilt also $1<p\le d\le \sqrt{2}$. Da $p\mid d$ und $d\mid n$,
folgt $p\mid n$, und wir sind fertig.






----

----
**Backlinks:**
- [Primzahlen](primzahlen)
