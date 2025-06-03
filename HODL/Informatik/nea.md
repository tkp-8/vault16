---
title: NEA
date: 2025-05-07 06:16
tags: 
---

----

### Definition 
##### Nichtdeterministischer Endlicher Automat $N$
$N\coloneqq (Q,\Sigma, \delta, q_{0}, F)$\
$\mathcal{P}(X)\coloneqq \{Y\mid Y\subseteq X\}$

> - $Q$ eine endliche nich-leere Menge, genannt **Zusatsmenge**
> - $\Sigma$ ein (endliches) [Alphabet](alphabet)
> - $\delta$ eine Funktion $\delta:Q\times (\Sigma \cup \{\varepsilon\}) \to \mathcal{P}(Q)$, genannt **Uebergangsfunktion**
> - $q_{0}$ ein Element aus $Q$, genannt **Startzustand**
> - $F$ eine Teilmenge von $Q$, genannt Menge der **akzeptierten Zustaende**

##### $\varepsilon$-Uebergaenge
Zustandsuebergang, **ohne** ein Zeichen der Eingabe zu lesen

Sei $E(p)$ die Menge aller Zustaende, die wir von $p$ aus erreichen koennen, ohne
ein Zeichen zu lesen
$$
  E(p)\coloneqq \{q\mid q \text{ ist von } p \text{ durch eine Sequenz von }\ge 0 \ \varepsilon\text{-
Uebergaengen erreichbar}\}  
$$
Fuer Mengen $P\subseteq Q$ definieren wir
$$
  E(P)\coloneqq \bigcup_{p \in  P}E(p) 
$$

##### Sprache eines NEAs 
Sei $N$ ein NEA, dann ist die von $N$ akzeptierte [Sprachen](sprachen) definiert als
$$
  L(N)\coloneqq \{w\in \Sigma ^{*}\mid \delta ^{*}(\{q_{0}\},w)\cap F \neq \empty\}  
$$
D.h. es muss mindestens einen **akzeptierenden $w$-Lauf** geben, damit $w \in L(N)$


---

### Iterierte Uebergangsfunktion 
Sei $\delta$ die Uebergangsfunktion eines NEAs, dann definieren wir fuer 
alle $P\subseteq Q$
$$
  \delta ^{0}(P,\varepsilon) = E(P) 
$$
und fuer alle $i>0$ und alle Woerter $w=ua\in \Sigma ^{i}$ mit $u\in \Sigma ^{i-1}$
und $a\in \Sigma$
$$
  \delta ^{i}(P,w) = E\left( \bigcup\nolimits_{r \in \delta ^{i-1}(P,u)}\delta(r,a) \right) 
$$
**Iterale Uebergangsfunktion** $\delta ^{*}:\mathcal{P}(Q)\times \Sigma ^{*}\to \mathcal{P}(Q)$
$$
  \delta ^{*}(P,w) \coloneqq \delta ^{|w|}(P,w)  
$$


----

----
**Backlinks:**
- [Endliche Automaten](/endliche_automaten)
