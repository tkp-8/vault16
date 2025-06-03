---
title: Ordnungsaxiome
date: 2025-06-02 09:30
tags: axiome
---

----

### Axiome 
(A1) **Trichotomiegesetx:** Fuer je zwei Zahlen $a,b$ gilt genau eine der drei Beziehungen:
$$
  a<b \text{ oder } a=b \text{ oder } a>b
$$
(A2) **Transitivitaetsgesetz:** Ist $a<b$ und $b<c$, so folgt $a<c$\
(A3) **Monotoniegesetz:** Ist $a<b$, so gilt $a+c<b+c$ fuer alle $c$, und es gilt $ac<bc$ fuer alle $c>0$

---

### Folgerungen
##### Proposition 1
Fuer alle reellen Zahlen $a$ und $b$ gilt:

1. $a<b\Leftrightarrow b-a>0$
2. $a<0\Leftrightarrow -a>0$
3. $a>0\Leftrightarrow -a<0$
4. $a<b \Leftrightarrow -b<-a$

**Beweis:** 
1. Aus $a<b$ folgt mit (A3) $0=a+(-a)<b+(-a)=b-a$, also $b-a>0$. Gilt umgekehrt $b-a>0$, 
   so folgt $b-a+a>0+a$, also $b>a$
2. Die Aussage folgt aus 1. mit $b=0$
3. Die Aussage folgt aus 2., wenn wir $a$ durch $-a$ ersetzen und beachten, dass $-(-a)=a$ ist
4. Es gilt 
   $$
   \begin{align*}
    
    a<b&\Leftrightarrow b-a>0 &\text{mit }1 \\
    &\Leftrightarrow -a-(-b)>0 & \text{da } -(-b)=b \\
    &\Leftrightarrow -b<-a & \text{mit } 1
   \end{align*}
   $$

##### Proposition 2
Sei $b\neq 0$. Dann gilt:

1. $\frac{1}{b}>0\Leftrightarrow b>0$
2. $\frac{a}{b}>0\Leftrightarrow \text{ Zaehler und Nenner sind beide positiv oder beide negativ}$

**Beweis:**

1. Es ist $b\cdot \frac{1}{b}=1>0$. Da $1$ positiv ist, ist das Produkt genau dann positiv, 
   wenn beide Faktoren positiv sind (da $b >0$)
2. Genau dann ist $\frac{a}{b}=a\cdot \frac{1}{b}$ positiv, wenn $a$ und $\frac{1}{b}$ positiv sind 
   oder $a$ und $\frac{1}{b}$ negativ sind

##### Proposition 3 (Abschaetzung von Bruechen)

1. Ist $p_{1}<p_{2}$ und $q>0$, so gilt $\frac{p_{1}}{q}<\frac{p_{2}}{q}$
2. Ist $0<q_{1}<q_{2}$ und ist $p>0$, so gilt $\frac{p}{q_{2}}<\frac{p}{q_{1}}$

**Beweis:**

1. Mit Proposition 2 ist $\frac{1}{q}>0$. Die Behauptung ergibt sich aus (A3)
2. Es ist $\frac{p}{q_{1}q_{2}}>0$. Wir multiplizieren die Ungleichung $q_{1}<q_{2}$ mit $\frac{p}{q_{1}q_{2}}$, und 
   mit (A3) folgt die Behauptung

##### Satz 1 (Bernoulli'sche Ungleichung)
[Bernoulli'sche Ungleichung](bernoullische_ungleichung)






----

----
**Backlinks:**
- [📂Analysis Grundlagen](/📁Analysis_Grundlagen)
