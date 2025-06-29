---
title: Loesung_Linearer_Kongruenzen
date: 2025-06-27 22:53
tags: 
---

----

### Definition
Sei $aX\equiv b \pmod{m}$ eine [lineare Kongruenz](lineare_kongruenzen). Eine *Loesung* von $aX\equiv b \pmod{m}$ ist ein 
$x_{0}\in \mathbb{Z}_{m}$ mit $ax_{0}\equiv b \pmod{m}$.

---

### Eigenschaften
**Beobachtung 1:** Wenn $x_{0}$ eine Loesung von $aX\equiv b \pmod{m}$ ist, dann ist $\text{ggT}(a,m)$ ein Teiler von $b$.\
**Beweis:** Sei $d=\text{ggT}(a,m)$ und sei $x_{0}\in \mathbb{Z}_m$ mit $ax_{0}\equiv b \pmod{m}$. Dann gilt $m\mid ax_{0}-b$, es gibt also 
ein $k\in \mathbb{Z}$ mit $km=ax_{0}-b$. Da $d$ ein Teiler von $m$ ist, folgt $d\mid ax_{0}-b$. Da $d$ ein Teiler von $ax_{0}-b$ und $a$ ist, ist $d$ 
ein Teiler von $ax_{0}-b-ax_{0}=-b$. Es folgt, dass $d$ ein Teiler von $b$ ist.

**Lemma 1 (Genau eine Loesung):** Sei $aX\equiv b \pmod{m}$ eine lineare Kongruenz. Sei $\text{ggT}(a,m)=1$, und seien 
$s,t\in \mathbb{Z}$, sodass $1=as+tm$ gilt. Sei $x_{0}=sb\text{ mod }m$. \
Dann ist $x_{0}$ die einzige Loesung von $aX\equiv b \pmod{m}$.\
**Beweis:** $\text{ggT}(a,m)=1$$\implies$ Mit dem [erweiterten Euklidischen Algorithmus](euklidischer_algorithmus) gibt es $s,t\in \mathbb{Z}$ mit $1=as+tm$.\
$\Leftrightarrow b=asn+tmb$ \
$\Leftrightarrow m\mid asb-b\Leftrightarrow a(sb)\equiv b \pmod{m}$\
Mit [Proposition 1](lineare_kongruenzen) ist $x_{0}=sb\text{ mod } m$ eine Loesung von $aX\equiv b\pmod{m}$ \
*Eindeutigkeit der Loesung:* Annahme: Es gibt eine weitere Loesung $x_{1}\in \mathbb{Z}_m$. \
$\Leftrightarrow$ $ax_{1}\equiv b \pmod{m}$, $b\equiv ax_{0}\pmod{m}$\
$\Leftrightarrow ax_{1}\equiv ax_{0} \pmod{m}$\
$\Leftrightarrow x_{1}\equiv x_{0}\pmod{m}$, da $\text{ggT}(a,m)=1$\
Da $x_{0},x_{1}\in \mathbb{Z}_m$, folgt $x_{0}=x_{1}$

**Lemma 2 (Mehrere Loesungen):** Sei $aX\equiv b \pmod{m}$. Sei $d=\text{ggT}(a,m)$, und sei $d$ ein Teiler von
$b$. Dann gibt es genau $d$ Loesungen von $aX\equiv b\pmod{m}$.\
Sei $x_{0}$ die eindeutig bestimmte Loesung von $\frac{a}{d} X \equiv \frac{b}{d} \pmod{\frac{m}{d}}$. Dann sind
$$
  x_{0},x_{0}+\frac{m}{d},x_{0}+2\frac{m}{d},\ldots ,x_{0}+(d-1)\frac{m}{d}
$$
alle Loesungen von $aX\equiv b \pmod{m}$.\
**Beweis:** Da $x_{0} \in \{0,\ldots ,\frac{m}{d}-1\}$, gilt $x_{0}<\frac{m}{d}$, also ist
$$
  0\le x_{0}<x_{0}+\frac{m}{d}<\cdots <x_{0}+(d-1)\frac{m}{d}<d\frac{m}{d}=m
$$
Das sind genau $d$ verschiedene Elemente in $\mathbb{Z}_m$. Wir zeigen, dass sie Loesungen von $aX\equiv b\pmod{m}$ sind.\
Mit [Proposition 1.2](lineare_kongruenzen) gilt $\frac{a}{d}(x_{0}+k\frac{m}{d})=\frac{b}{d}\pmod{\frac{m}{d}}$ fuer alle $k\in \mathbb{Z}$. \
$\Leftrightarrow \frac{a}{d}(x_{0}+k{\frac{m}{d}})-\frac{b}{d}=n_k{\frac{m}{d}}$ fuer ein $n_k\in \mathbb{Z}$\
$\Leftrightarrow$ $a(x_{0}+k{\frac{m}{d}})-b=n_km$\
$\Leftrightarrow a(x_{0}+k{\frac{m}{d}})\equiv b \pmod{m}$ fuer alle $0\le k\le d-1$\
Es gibt keine weiteren Loesungen:\
Sei $x_{1}\in \mathbb{Z_m}$ eine Loesung von $aX\equiv b\pmod{m}$.\
$\Leftrightarrow ax_{1}\equiv b \pmod{m}$ und $ax_{0}\equiv b \pmod{m}$\
$\Leftrightarrow ax_1\equiv ax_{0} \pmod{m}$\
$\Leftrightarrow x_{1}\equiv x_{0} \pmod{\frac{m}{d}}$, mit [Rechenregel 7](kongruenzen)\
$\Leftrightarrow \exists k\in \mathbb{Z}: x_{1}-x_{0}=k{\frac{m}{d}}$\
$\Leftrightarrow x_{1}=x_{0}+k{\frac{m}{d}}$ mit $k\in \{0,\ldots ,d-1\}$, da $x_{1}\in \mathbb{Z}$ \
Somit gilt $x_{1}\in \{x_{0},x_{0}+\frac{m}{d},\ldots ,x_{0}+(d-1)\frac{m}{d}\}$, genau die Loesungen die wir im ersten Schritt gefunden haben.

---

### Algorithmus
##### Bestimmung aller Loesungen einer lineaeren Kongruenz

1. Die Eingabe ist eine lineare Kongruenz $aX\equiv b \pmod{m}$ mit $\text{ggT}(a,m)=d$ und $d\mid b$. 
   Die Ausgabe sind alle $d$ Loesungen
2. Bestimme mit Hilfe des erweiterten Euklidischen Algorithmus ganze Zahlen $s$ und $t$, sodass $1=\frac{a}{d}s+\frac{m}{d}t$ ist
3. Setze $x_{0}=s\frac{b}{d}\text{ mod } \frac{m}{d}$
4. Fuer alle $1\le i\le d-1$ setze $x_i=x_{0}+i{\frac{m}{d}}$
5. Die Loesungen sind $x_{0},\ldots ,x_{d-1}$

----

----
**Backlinks:**
- [Lineare Kongruenzen](/lineare_kongruenzen)
