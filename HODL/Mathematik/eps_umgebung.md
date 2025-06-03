---
title: Eps_Umgebung
date: 2025-06-02 22:57
tags: 
---

----

### Definition 

Sei $(a,b)$ beziehungsweise $[a,b]$ ein Intervall mit Mittelpunkt $x_{0}$ und Radius $\varepsilon$.
Dann wird $(a,b)$ mit $U_\varepsilon(x_{0})$ und $[a,b]$ mit $U_\varepsilon[x_{0}]$ bezeichnet
und **offene $\varepsilon$-Umgebung** beziehungsweise **abgeschlossene $\varepsilon$-Umgebung** um
$x_{0}$ genannt

---

### Eigenschaften

##### Proposition 1
Sei $x_{0}\in \mathbb{R}$, und sei $\varepsilon>0$. Dann gilt 
$$
  U_\varepsilon(x_{0})=\{x\in \mathbb{R}\mid |x-x_{0}|<\varepsilon\}\text{ und }    U_\varepsilon[x_{0}]=\{x\in \mathbb{R}\mid |x-x_{0}|\le \varepsilon\}
$$
**Beweis:** Die Randpunkte sind $a=x_{0}-\varepsilon$ und $b=x_{0}+\varepsilon$. \
Sei $x\in U_\varepsilon(x_{0})$. Dann gilt $x_{0}-\varepsilon<x<x_{0}+\varepsilon$. Aus dem [Monotoniegesetz](ordnungsaxiome) 
folgt $-\varepsilon<x-x_{0}<\varepsilon$. Ist $x-x_{0}\ge 0$, so folgt $|x-x_{0}|=x-x_{0}<\varepsilon$, also 
$x\in \{x\in \mathbb{R}\mid |x-x_{0}|<\varepsilon\}$. Ist $x-x_{0}<0$, so folgt aus $-\varepsilon<x-x_{0}$ die 
Ungleichung $-(-\varepsilon)>-(x-x_{0})$. Es sind aber $-(-\varepsilon)$ und $-(x-x_{0})=|x-x_{0}|$. Somit gilt auch 
in diesem Fall $|x-x_{0}|<\varepsilon$ und $x\in \{x\in \mathbb{R}\mid |x-x_{0}|<\varepsilon\}$. Also haben wir gezeigt, 
dass $U_\varepsilon(x_{0}) \subseteq \{x\in \mathbb{R}\mid |x-x_{0}|<\varepsilon\}$ gilt.

Sei umgekehrt $x\in \mathbb{R}$ mit $|x-x_{0}|<\varepsilon$. Ist $x-x_{0}\ge 0$, so gilt $|x-x_{0}|=x-x_{0}<\varepsilon$ 
und wir bekommen $-\varepsilon<x-x_{0}<\varepsilon$. Mit dem Monotoniegesetz folgt $x_{0}-\varepsilon<x<x_{0}+\varepsilon$.
Ist $x-x_{0}<0$, so gilt $-(x-x_{0})=|x-x_{0}|$, also $-\varepsilon<-(x-x_{0})<\varepsilon$. Es folgt $\varepsilon>x-x_{0}>-\varepsilon$, 
und mit dem Monotoniegesetz erhalten wir $x_{0}-\varepsilon<x<x_{0}+\varepsilon$. Es folgt $\{x\in \mathbb{R}\mid |x-x_{0}|<\varepsilon\} \subseteq U_\varepsilon(x_{0})$, also
$U(x_{0})=\{x\in \mathbb{R}\mid |x-x_{0}|<\varepsilon\}$




----

----
**Backlinks:**
- [📂Analysis Grundlagen](/📁Analysis_Grundlagen)
