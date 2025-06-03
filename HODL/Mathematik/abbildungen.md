---
title: Abbildungen
date: 2025-06-02 08:16
tags: 
---

----

### Definition

Seien $M$ und $N$ Mengen. Eine *Abbildung* von $M$ nach $N$ ist eine Teilmenge $f \subseteq M\times N$,
so dass folgende Eigenschaften gelten:

1. Fuer alle $m\in M$ gibt es ein $n\in N$, so dass $(m,n)\in f$
2. Wenn $(m,n)\in f$ und $(m,n^{\prime})\in f$, so folgt $n=n^{\prime}$

$M$ heisst **Definitionsbereich**, $N$ heisst **Wertebereich** von $f$

---

### Notation
Seien $f\subseteq M\times N$ und $g\subseteq L\times M$ Abbildungen

**$f$ ist eine Abbildung von $M$ nach $N$**\
$f:M\to N$

**Zu $m\in M$ eindeutig bestimmte $n\in N$**\
$n=f(m)$

**$m$ wird auf $f(m)$ abgebildet**
$m\mapsto f(m)$

**Komposition von $f$ und $g$**\
$g\circ f:L\to N$, definiert durch $(g\circ f)(l)=g(f(l))$

**Identische Abbildung**\
$\text{id}_M:M\to M$, $\text{id}_M(m)=m$ fuer alle $m\in M$

---

### Terminologie
##### Bild 
Man nennt $f(m)$ das *Bild* von $m$ unter $f$

##### Bildbereich (alt: Bild)
$\text{Bild}(f)=\{n\in N\mid \text{es gibt ein }m\in M \text{ mit } f(m)=n\}$

##### Urbild 
Ist $n\in \text{Bild}(f)$, so wird ein $m\in M$ mit $f(m)=n$ ein *Urbild* von $n$ unter $f$ genannt

##### Invertierbarkeit
$f$ heisst *invertierbar*, wenn es eine Abbildung $f^{-1}:N \to M$ gibt, so dass $f^{-1}\circ f = \text{id}_M$ 
und $f\circ f^{-1}  = \text{id}_M$ ist

---

### Klassifizierung
##### Surjektivitaet
$f$ heisst *surjektiv*, wenn jedes Element $n\in N$ in $\text{Bild}(f)$ liegt

##### Injektivitaet
$f$ heisst *injektiv*, wenn jedes Element im $\text{Bild}(f)$ genau ein Urbild besitzt

##### Bijektivitaet
$f$ heisst *bijektiv*, wenn $f$ sowohl *surjektiv* als auch *injektiv* ist

---

### Invertierbare Abbildungen
Sei $f:M\to N$ eine Abbildung. Die folgenden Aussagen sind aequivalent:\

1. $f$ ist bijektiv
2. $f$ ist invertierbar





----

----
**Backlinks:**
- [🗃️Analysis](/🗃️Analysis)
