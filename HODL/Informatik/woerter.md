---
title: Woerter
date: 2025-05-06 02:17
tags: 
---

----

### Definition
##### Wort
Eine **Sequenz**(Tupel) von **Zeichen**

##### Teilwort
Wort $u$ heisst Teilwort von $w\in \Sigma ^{*}$, falls $x,y\in \Sigma ^{*}$ mit 
$w=xuy$ existieren

##### Praefix
Teilwort als Anfangsteil des Wortes

##### Suffix 
Teilwort als Endteil des Wortes

---

### Notation
**Haeufig Benutzte Variablen fuer Woerter**\
$u,v,w,x,y,z$

**Seine Zeichen in der entsprechende Reihenfolge** \
(z.B. $\texttt{aba}$)

**Laenge eines Wortes $u$** \
$|u|$ 

**Menge Woerter der Laenge $k$ ueber dem [Alphabet](alphabet)** $\Sigma$\
$\Sigma^{k}$ 

**Das leere Wort**\
$\varepsilon$ 

**Menge aller Woerter** $\Sigma ^{*}$\
$\Sigma^{*}\coloneqq \bigcup ^{\infty}_{k=0}\Sigma ^{k}$

**Menge aller Woerter ausschliesslich** $\varepsilon$\
$\Sigma ^{+} \coloneqq \bigcup_{k=1}^{\infty}\Sigma ^{k}=\Sigma ^{*} \setminus \{\varepsilon\}$

**Kodierung von Objekten $\cdot$ als Woerter**\
$\langle \cdot \rangle$

**Konkatenation** $\cdot$ \
Hintereinanderreihung von Woertern $u,v$\
$uv$ oder $u\cdot v$\
$u^{k}=u^{k-1}u \quad$ ($u^{0}=\varepsilon$)

**Spiegelung** \
Umkehrung der Reihenfolge der Zeichen eines Wortes $u=\texttt{abb}$\
$\overleftarrow{u}=\texttt{bba}$

---
 
### Beispiel
##### [Kodierung](kodierung) eines Graphens $G$
- Menge aller Zeichen $\{0,1,2,3,4,5,6,7,8,9,\#\}$
- Trennung der Woerter durch $\#\#$
- Kante $(a,b)$ mit Gewicht $w(a,b)$: $a\#b\#w(a,b)$
- das **Wort** das wir erhalten: Kodierung des Graphens $G$
    - $1\#2\#2\#\#2\#3\#1\#\#3\#4\#1\#\#4\#2\#1$






----

----
**Backlinks:**
- [📁Formale_Sprachen&Automaten](📁Formale_Sprachen&Automaten)
- [Kodierung](kodierung)
