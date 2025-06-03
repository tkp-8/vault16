---
title: Kongruenzen
date: 2025-05-17 12:22
tags: 
---

----

### Definition 
Seien $a$ und $b$ ganze Zahlen, und sei $m\in N$.
Wir sagen, dass $a$ **kongruent** zu $b$ **modulo** $m$ ist, wenn $m$ ein Teiler von 
$a-b$ ist. 


---

### Notation
**$a$ kongruent zu $b$ modulo $m$** \
$a\equiv b \pmod{m}$

**Wenn nicht**\
$a\not\equiv b \pmod{m}$

---

### Bemerkung
Seien $a,b\in \mathbb{Z}$, und sei $m\in \mathbb{N}, \ m>1$.
$$
  a\equiv b\pmod{m}\Leftrightarrow \exists k\in Z: a=b+km
$$
**Beweis**\
$\Rightarrow$: Es gilt $m\mid (a-b)$, also gibt es ein $k\in \mathbb{Z}$ mit $a-b=km$.
Somit gilt $a=b+km$ fuer ein $k\in \mathbb{Z}$\
$\Leftarrow$: Es folgt $a-b=km$, also $m\mid (a-b)$. Somi gilt $a\equiv b \pmod{m}$.

---

### Eigenschaften
**Proposition 1:** Seien $a,b\in Z$ und sei $m\in N, \ m>1$. 
$$
  a\equiv b \pmod{m} \Leftrightarrow a \text{ und } b \text{ haben bei der Division durch } m
  \text{ mit Rest denselben Rest}
$$
**Beweis:** Sei $a\equiv b \pmod{m}$. Wir teilen $a$ und $b$ durch $m$ mit Rest und erhalten
$$
  a=q_{1}m+r_{1} \text{ und } b=q_{2}m+r_{2} \text{ mit } 0\le r_{1},r_{2}<m.
$$
$\Rightarrow$: Es gilt $a-b=(q_{1}-q_{2})m +r_{1}-r_{2}$. Da $m$ ein Teiler von $a-b$ und $(q_{1}-q_{2})m$
ist, muss $m$ auch $r_{1}-r_{2}$ teilen. Da $0\le r_{1},r_{2}<m$ gilt, folgt $|r_{1}-r_{2}|<m$.
Daher ist $m\mid (r_{1}-r_{2})$ nur dann moeglich, wenn $r_{1}-r_{2}=0$ gilt. Es folgt $r_{1}=r_{2}.$\
$\Leftarrow$: Seien umgekehrt $a=q_{1}m+r$ und $b=q_{2}m+r$ mit $0\le r\le m$. Dann gilt 
$a-b=(q_{1}-q_{2})m$, also $m\mid (a-b)$, und es gilt $a\equiv b \pmod{m}$.

**Korollar zu Proposition 1**:
$$
  a\equiv b \pmod{m} \Leftrightarrow a\text{ mod }{m}=b\text{ mod }{m}
$$

---

### Rechenregeln 
Fuer alle $a,b,c\in \mathbb{Z}$ und alle $m\in \mathbb{N}, m>1$, gilt:
1. $a\equiv a \pmod{m}$
2. Ist $a\equiv b \pmod{m}$, so ist $b \equiv a \pmod{m}$
3. Sind $a\equiv b \pmod{m}$ und $b\equiv c\pmod{m}$, so gilt $a\equiv c \pmod{m}$
4. Ist $a\equiv b \pmod{m}$, so gilt $a+c\equiv b+c \pmod{m}$
5. Ist $a\equiv b \pmod{m}$, so gilt $ac\equiv bc \pmod{m}$
6. Ist $ac\equiv bc \pmod{m}$, und gilt $\text{ggT}(c,m)=1$, so folgt $a\equiv b \pmod{m}$
7. Ist $ac \equiv bc \pmod{m}$, und gilt $\text{ggT}(c,m)=d$, so folgt $a\equiv b \pmod{\frac{m}{d}}$
8. Ist $a\equiv b \pmod{m}$, so gilt $a^{n}\equiv b^{n}\pmod{m}$ fuer alle $n\in \mathbb{N}$

**Beweis:**
1. Es gilt $m\mid (a-a)$
2. Es gilt $m\mid (a-b)$, also $m\mid -(a-b)$, und somit $m\mid (b-a)$
3. Es gelten $m\mid (a-b)$ und $m\mid (b-c). Dann gibt es $x,y \in \mathbb{Z}$ mit 
   $mx=a-b$ und $my=b-c$. Es folgt $m(x+y)=a-c$, also $m\mid (a-c)$
4. Wenn $m\mid (a-b)$, so folgt $m\mid (a+c-b-c)$
5. Wenn $m\mid (a-b)$, so folgt $m\mid c(a-b)$, also $m\mid ac-bc$
6. Es gilt $m\mid c(a-b)$ und wegen $\text{ggT}(c,m)=1$ folgt $m\mid (a-b)$
7. Es gilt $m\mid c(a-b)$, also $\frac{m}{d}\mid \frac{c}{d}(a-b)$. Da $\text{ggT}(\frac{m}{d},\frac{c}{d})=1$
   , folgt $\frac{m}{d}\mid (a-b)$
8. Es gilt $m\mid (a-b)$. Ausserdem gilt $(a-b)\mid a^{n}-b^{n}$, da
$$
\begin{align*}
  &\quad \; (a-b)(a^{n-1}+a^{n-2}b+\cdots+ab^{n-2}+b^{n-1}    )\\
  &= a^{n} -a^{n-1}b+a^{n-1}b -\cdots-ab^{n-1}+ab^{n-1}-b^{n}      \\
  &= a^{n}-b^{n}  
\end{align*}
$$

---

### Verwandt
[Restklassen](restklassen)
[Lineare Kongruenzen](lineare_kongruenzen)

----

----
**Backlinks:**
- [📂Elementare_Zahlentheorie](/📁Elementare_Zahlentheorie)
