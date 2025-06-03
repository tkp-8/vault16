---
title: Konvergenz_Folge
date: 2025-06-03 00:11
tags: 
---

----

### Definition 
Eine reelle [Folge](folgen) *konvergiert* gegen $a\in \mathbb{R}$, wenn es zu jeder positiven
Zahl $\varepsilon$ einen Index $n_{0}$ so gibt, dass fuer alle Indizes $n>n_{0}$ stets 
$|a_n-a|<\varepsilon$ ist

**Bemerkung:** Eine Folge ist *konvergent*, wenn sie nicht [divergent](divergenz_folge) ist

---

### Notation

Dass eine Folge $(a_n)$ gegen $a$ konvergiert drueckt man wie fogt aus:
$$
  \lim_{n\to \infty}a_n = a \text{ oder } \lim{a_n} =a
$$

---

### Terminologie

**Teilfolge**\
Ist $(n_{1},n_{2},\ldots )$ eine streng wachsende Folge von natuerlichen Zahlen (also $n_i<n_{i+1}$ fuer alle $i\in \mathbb{N}$), 
so nennen wir $(a_{n_{1}},a_{n_{2}}, \ldots )$ eine *Teilfolge* von $(a_n)$

**Beschraenkte Folgen**\
Eine Folge $(a_n)$ heisst *beschraenkt*, wenn die Menge $\{a_{1},a_{2},\ldots \}$ beschraenkt ist

**Monotonie**\
Eine Folge $(a_n)$ heisst *monoton* falls gilt:

1. $\forall n\in \mathbb{N}: a_n\le a_{n+1}$, oder 
2. $\forall n\in \mathbb{N}: a_n\ge a_{n+1}$

Im ersten fall nennt man $(a_n)$ *monoton wachsend*, im zweiten Fall *monoton fallend*


---

### Eigenschaften konvergenter Folgen

##### Proposition 1 
Eine konvergente Folge besitzt genau einen Grenzwert

##### Proposition 2
Jede Teilfolge einer konvergenten Folge $(a_n)$ konvergiert gegen $\lim{a_n}$

##### Proposition 3
Jede konvergente Folge $(a_n)$ ist beschraenkt

##### Proposition 4
Jede [reelle Zahl](reelle_zahlen) $a$ ist Grenzwert einer Folge rationaler Zahlen

---

### Beispiele konvergenter Folgen

**Konstante Folge**\
$(a,a,a\ldots )$ konvergiert gegen $a$

**Kehrwert einer Wurzel**\
Sei $p \in \mathbb{N}$. Die Folge $\left(\frac{1}{\sqrt[p]{n}}\right)$ konvergiert gegen $0$

**Wurzel mit selbem Radikand und Wurzelexponenten**\
$(\sqrt[n]{n})$ konvergiert gegen 1

**Potenzfolge mit |Basis| $<1$**\
Fuer feste $q$ mit $|q|<1$ konvergiert die Folge $(q^{n})$ gegen 0

---

### Rechnen mit konvergenten Folgen

- [Vergleichssatz](vergleichssatz)
- [Einschnuerungssatz](einschnuerungssatz)
- [Betragssatz](betragssatz)

##### Rechenregeln
Sei $(a_n)$ konvergent gegen $a$, und sei $(b_n)$ konvergent gegen $b$. 

1. $(a_n+b_n)$ konvergiert gegen $a+b$
2. $(a_nb_n)$ konvergiert gegen $ab$
3. Ist $\alpha \in \mathbb{R}$, so konvergiert $(\alpha a_n)$ gegen $\alpha a$
4. $(a_n-b_n)$ konvergiert gegen $a-b$
5. Ist $b\neq 0$, und sind fast alle $b_n\neq 0$, so konvergiert $(\frac{a_n}{b_n})$ gegen $\frac{a}{b}$

---

### Vier Prinzipien der Konvergenztheorie

1. [Monotonieprinzip](monotonieprinzip)
2. [Bolzano_Weierstrass](bolzano_weierstrass)
3. [Cauchyfolgen](cauchyfolgen)
4. [Intervallverschaltelung](intervallverschaltelung)


----

----
**Backlinks:**
- [Konvergenz](/konvergenz)
