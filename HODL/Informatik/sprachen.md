---
title: Sprachen
date: 2025-05-06 05:01
tags: 
---

----

### Definition 
##### Sprache
Eine Menge von [Woertern](woerter)

##### Komplement
Komplement der Sprache $L$: \
Die Sprache $\Sigma ^{*}\setminus L$

##### Abschlusseigenschaften
Eine Sprachklasse $\mathcal{L}$ ist **abgeschlossen unter der Operation** $\oplus$,
falls fuer alle $L_{1},L_{2}\in \mathcal{L}$ gilt, dass 
$$L_{1}\oplus L_{2} \in \mathcal{L}$$

---

### Notation
**Konkatenation** $\circ$\
Seien $L_{1},L_{2}$ Sprachen aus dem selben [Alphabet](alphabet)
$L_{1}\circ L_{2}\coloneqq \{uv\mid u\in L_{1} \ \text{und} \ v\in L_{2}\}$

$$
  L^{k}\coloneqq \{w_{1}\cdots w_k\mid \forall i\le k:w_i \in L\}   
$$

$$
  L^{1}\coloneqq L,\quad L^{0}\coloneqq \{\varepsilon\}, \quad L^{*}\coloneqq 
  \bigcup_{k =  0}^{\infty}L^{k}, \quad L^{+} \coloneqq \bigcup_{k=1}^{\infty}L^{k}       
$$
 
**Komplement**\
$\overline{L}$

**Spiegelung**\
$\overleftarrow{L}\coloneqq \{\overleftarrow{w}\mid w\in L\}$

---

### Klassifizierung
##### Chomsky-Hierarchie

- rekursiv aufzaehlbar (Typ 0, $\mathcal{L}_{RE}$)
- kontextsensitiv (Typ 1, $\mathcal{L}_{ECS}$)
- [kontextfrei](kontextfreie_sprachen) (Typ 2, $\mathcal{L}_{CF}$)
- [regulaer](regulaere_sprachen) (Typ 3, $\mathcal{R}$)
 
---

### Beispiel
**Entscheidungsproblem:** "Ist die Zahl $x$ eine Primzahl?"
$$
  L_{prim} = \{\text{bin}(x)\in \{\texttt{0},\texttt{1}\}^{*}\mid x \ \text{ist Primzahl}   \}  
$$
Das Problem reduziert sich darauf, zu entscheiden, ob ein Wort($\text{bin}(x)$) aus einer 
gegebenen Sprache($L_{prim})$
ist $\to$ **Wortproblem**  


----

----
**Backlinks:**
- [📁Formale_Sprachen&Automaten](📁Formale_Sprachen&Automaten)
