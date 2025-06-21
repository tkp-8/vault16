---
title: Funktionen
date: 2025-06-03 00:02
tags: 
---

----

### Definition 
##### Funktion
Sei $D$ eine nicht leere Teilmenge von $\mathbb{R}$. Eine *Funktion* $f$ auf $D$ ist eine [Abbildung](abbildungen)
$f:D\to \mathbb{R}$. 

##### Bild
Die Menge 
$$
\{y\in \mathbb{R}\mid \text{es gibt ein }x\in D\text{ mit }f(x)=y\}  
$$
wird das *Bild* von $D$ unter $f$ genannt und mit $f(D)$ oder $\text{Bild}(f)$ bezeichnet

##### Graph
Der *Graph* einer Funktion $f:D\to \mathbb{R}$ ist die Menge
$$
  \{(x,f(x))\mid x\in D\}\subseteq D\times \mathbb{R}  
$$

##### Umkehrfunktion
Sei $f:D\to \mathbb{R}$ eine injektive Funktion. Die Funktion
$$
  f^{-1}:f(D)\to \mathbb{R} \text{ mit } f^{-1}\circ f=\text{id}_D \text{ und } f\circ f^{-1}=\text{id}_{f(D)}   
$$
wird *Umkehrfunktion* von $f$ genannt

##### Restriktion
Sei $f:D\to \mathbb{R}$ eine Funktion, und sei $D^{\prime}\subseteq D$, wobei $D^{\prime}\neq \empty$ ist. Dann
heisst die Funktion $f|_{D^{\prime} }:D^{\prime}\to \mathbb{R}$, definiert durch $f|_{D^{\prime} }(x)=f(x)$ fuer alle $x\in D^{\prime}$, die *Restriktion* von $f$ auf $D^{\prime}$

---

### Beispiele
##### Dirichletfunktion
$f:\mathbb{R}\to \mathbb{R}$, definiert durch
$$
  f(x)\begin{cases}
    1, &\text{ falls }x\in Q\\
    0, &\text{ falls }x\in \mathbb{R}\backslash \mathbb{Q}
    
  \end{cases}
$$

##### [Polynomfunktionen](polynomfunktionen)

---

### Eigenschaften

##### 1. Jede streng monotone Funktion $f:D\to \mathbb{R}$ ist injektiv\
**Beweis:** Sei $f:D\to \mathbb{R}$ streng monoton wachsend. Seien $x,y\in D$ mit $x\neq y$. Dann
gilt $x<y$, also $f(x)<f(y)$, oder $y<x$ und damit $f(y)<f(x)$. In Beiden Faellen folgt $f(x)\neq f(y)$, das 
heisst, $f$ ist injektiv

##### 2. Ist $f$ strend monoton wachsend / fallend, so ist $f^{-1}:f(D)\to \mathbb{R}$ streng monoton wachsend / fallend
**Beweis:** Sei $f:D\to \mathbb{R}$ streng monoton wachsend. Da $f$ injektiv ist, existiert $f^{-1}$.
Seien $x,y\in D$ mit $x\neq y$. Wir nehmen an, dass $x<y$. Dann gilt $f(x)<f(y)$ und $f^{-1}(f(x))=x<y=f^{-1}(f(y))$.


---





----

----
**Backlinks:**
- [Konvergenz](/konvergenz)
