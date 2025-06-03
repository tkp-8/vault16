---
title: DEA
date: 2025-05-07 01:13
tags: 
---

----

### Definition  
##### Deterministischer Endlicher Automat $M$
$M\coloneqq (Q,\Sigma, \delta, q_{0}, F)$

> - $Q$ eine endliche nich-leere Menge, genannt **Zusatsmenge**
> - $\Sigma$ ein (endliches) [Alphabet](alphabet)
> - $\delta$ eine Funktion $\delta:Q\times \Sigma \to Q$, genannt **Uebergangsfunktion**
> - $q_{0}$ ein Element aus $Q$, genannt **Startzustand**
> - $F$ eine Teilmenge von $Q$, genannt Menge der **akzeptierten Zustaende**

##### Sprache eines DEAs
$$
  L(M)\coloneqq \{w\in \Sigma ^{*}\mid \delta ^{*}(q_{0},w)\in F  \}  
$$

---

### Iterierte Uebergangsfunktion
Sei $\delta$ die Uebergangsfunktion eines DEAs, dann definieren wir fuer alle $q\in Q$
$$
    \delta ^0(q,\varepsilon) = q
$$
und fuer alle $i>0$ und alle Woerter $w=ua\in \Sigma ^{i}$ mit $u\in \Sigma ^{i-1}$
und $a \in \Sigma$
$$
    \delta ^{i}(q,w) = \delta(\delta ^{i-1}(q,u),a) 
$$
**Iterierte Uebergangsfunktion** $\delta ^{*}:Q\times \Sigma ^{*}\to Q$
$$
    \delta ^{*}(q,w) \coloneqq \delta ^{|w|}(q,w) 
$$

---

### Beispiel 
$M_{1}=(Q,\Sigma,\delta,q_{0},F)$ mit $Q=\{q_{0},q_{1}\}, \Sigma=\{\texttt{a},\texttt{b}\}, F=\{q_{0}\}$

|$q\in Q$|$x\in \Sigma$|$\delta(q,x)$|
|----- |--- |--- |
|$q_{0}$|$\texttt{a}$|$q_{1}$|
| $q_{0}$ |  $\texttt{b}$ | $q_{0}$  |
|  $q_{1}$ |$\texttt{a}$   |  $q_{0}$ |
| $q_{1}$  | $\texttt{b}$  |  $q_{1}$ |
![](img/dea_1.png)

$$
  L(M_{1}) = \{w\in \{\texttt{a},\texttt{b}\}^{*}\mid w \text{ enthaelt gerade Anzahl von } \texttt{a}\text{s}\}  
$$








----

----
**Backlinks:**
- [Endliche Automaten](/endliche_automaten)
