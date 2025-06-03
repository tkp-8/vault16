---
title: Primzahlen
date: 2025-05-03 10:09
tags: 
---

----

### Definition
##### Primzahlen
$p \in \mathbb{N}$ ist eine **Primzahl**, wenn $p > 1$ und wenn $p$ **genau zwei
positive Teiler** hat

Primzahlen $\leftrightarrow$ [zusammengesetzte Zahlen](zusammengesetzte_zahlen)

##### [Mersenne'sche Primzahlen](mersennesche_primzahlen)
Primzahlen der Form $p=2^{n}-1$, $n\in \mathbb{N}$

---

### Terminologie

**Echte Teiler:** Alle positiven Teiler von n, die **ungleich 1** und **ungleich n** sind 

**Primteiler $p$ von $n$**: $p \in \mathbb{P}$ und $p\mid n$  

**Primzahlzwillinge:** $\{(p,p+2) \mid p,p+2 \in \mathbb{P}\}$

[Primzahldrillinge](primzahldrillinge): $\{(p,p+2,p+4) \mid p,p+2,p+4 \in \mathbb{P}\}$

**Primzahlfunktion $\pi (x)$:** $\pi: \mathbb{R}\to \mathbb{N}_0$, ordnet jeder reellen Zahl x die 
Anzahl der Primzahlen $\le x$ zu

---

### 🍁Maple
`isprime(n:int)`$\to true/false$ : Ueberpruefung ob Primzahl 

`nextprime(n:int)/prevprime(n:int)`$\to int$ : naechste/letzte Primzahl

`pi(x:R+)`$\to int$: $\pi (x)$

---

### Eigenschaften 

- [Primteilerexistenz](primteilerexistenz): $\forall n \in \mathbb{N}, n \ge 2 \ \exists p \in \mathbb{P}: p \mid n$  
- [Satz_des_Euklid](satz_des_euklid): Es gibt unendlich viele Primzahlen.
- [Primzahldrillinge](primzahldrillinge): Ausser $(3,5,7)$ gibt es keine weiteren Primzahldrillinge.
- [Primabstand](primabstand): Es gibt beliebig grosse Loecher zwischen Primzahlen

---

### Algorithmen

- [Das_Sieb_des_Eratosthenes](das_sieb_des_eratosthenes): Bestimmung aller Primzahllen kleiner oder gleich einer 
  vorgegebenen Zahl



----

----
**Backlinks:**
- [📂Elementare_Zahlentheorie](📁Elementare_Zahlentheorie)
