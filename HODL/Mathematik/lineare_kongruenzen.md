---
title: Lineare Kongruenzen
date: 2025-05-26 11:01
tags: 
---

----

### Definition
**Lineare Kongruenz** \
Eine *lineare Kongruenz* ist ein Ausdruck $aX\equiv b \pmod{m}$, wobei $a,b\in \mathbb{Z}$
und $m\in \mathbb{N},m>1$, sind.

**[Loesung_Linearer_Kongruenzen](loesung_linearer_kongruenzen)**\
Sei $aX\equiv b \pmod{m}$ eine lineare Kongruenz. Eine *Loesung* von $aX\equiv b \pmod{m}$ ist ein 
$x_{0}\in \mathbb{Z}_{m}$ mit $ax_{0}\equiv b \pmod{m}$.

---

### Proposition 1
##### Sei $aX\equiv b \pmod{m}$ eine lineare Kongruenz. Dann gilt:
1. Wenn $ax\equiv b \pmod{m}$ fuer ein $x\in \mathbb{Z}$ ist, so folgt $a(x\text{ mod {m}})\equiv b \pmod{m}$
2. Ist $ax\equiv b \pmod{m}$ fuer ein $x\in \mathbb{Z}$, so folgt $a(x+km)\equiv b \pmod{m}$
   fuer alle $k\in \mathbb{Z}$

**Beweis:**

1. Sei $ax\equiv b \pmod{m}$. Sei $x_{0}=x \text{ mod }m$ \
   Mit [Korollar1](restklassen) gilt $x\equiv x_{0}\pmod{m}$. Mit [Rechenregel](lineare_kongruenzen) 5 folgt 
   $$
    ax\equiv ax_{0}\pmod{m}
   $$
   Mit Rechenregel 2 folgt 
   $$
    ax_{0}\equiv ax \pmod{m}
   $$
   Wir haben damit 
   $$
    ax_{0}\equiv ax\pmod{m} \text{ und } ax\equiv b \pmod{m}
   $$
   Mit Rechenregel 3 folgt $ax_{0}\equiv b \pmod{m}$
 
3. Sei $ax\equiv b \pmod{m}$. Dann gilt $m\mid ax-b$. Sei $k\in \mathbb{Z}$. Dann gilt
   $$
    a(x+km)-b=ax+akm-b=(ax-b)+akm
   $$
   Da $m$ ein Teiler von $ax-b$ und $akm$ ist, ist $m$ ein Teiler von $a(x+km)-b$. Somit gilt die Behauptung fuer alle $k\in \mathbb{Z}$
   





----

----
**Backlinks:**
- [Kongruenzen](/kongruenzen)
