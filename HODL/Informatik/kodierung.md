---
title: Kodierung
date: 2025-05-05 07:27
tags: 
---

----

### Definition 
- **Umwandlung** eines mathematischen Modells in eine endliche Anzahl von **Zeichen**, welche von 
einem Rechner gelesen werden kann 
- **Injektive** Abbildung der Menge der Probleminstanzen $\mathcal{I}$ auf die Menge aller
- **alle Bestandteile** der Probleminstanz muessen aus der 
Kodierung unkompliziert **wiedergewinnbar** sein
[Woerter](woerter) eines [Alphabets](alphabet)
$\Sigma ^{*}$ 
$$
    enc:\mathcal{I}\to \Sigma ^{*} 
$$

---

### Notation 
**Probleminstanz** \
$\mathcal{I}$

**Eine beliebige Kodierung der Probleminstanz** $\mathcal{I}$ \
$\left< \mathcal{I} \right>$

---

### Kodierung von Zahlen
##### Unaere Darstellung
Seien $\texttt{a} \in \Sigma$ und $n\in \mathbb{N}$\
Kodirung von $n$: $n$ verkettete Zeichen $\texttt{a} \quad(\texttt{a}^{n})$

##### Binaerdarstellung 
$\Sigma = \{\texttt{0},\texttt{1}\}$, $\text{bin}: \mathbb{N}\to \Sigma ^{*}$\
$\text{bin}(5)=101$

---

### Methoden

Beispiel: Kodierung eines Graphens $G$\
Menge aller Zeichen: $\{0,1,2,3,4,5,6,7,8,9,\#\}$

##### Wort-Kantenkodierung
- Trennung der Woerter durch $\#\#$
- Kante $(a,b)$ mit Gewicht $w(a,b)$: $a\#b\#w(a,b)$
- das **Wort** das wir erhalten: Kodierung des Graphens $G$:
    - $1\#2\#2\#\#2\#3\#1\#\#3\#4\#1\#\#4\#2\#1$

##### Kodierung als Adjazenzliste
- Abspeichern der Nachbarn fuer jeden Knoten
- Inklusive des Gewichts der dazugehoerigen Kante
- Redundanz ist vorhanden
$$
    N_u = u\#v_{1}\#w(u,v_{1})\#v_{2}\#w(u,v_{2})\#\ldots 
$$
- Kodierung des Graphens $G$ ist das Wort
$$
    N_{1}\#\#N_{2}\#\#N_{3}\ldots 
$$

##### Kodierung als Adjazenzmatriz
- Matrix $A=(a_{ij})$, fuer die gilt:
$$
    a_{ij} = \begin{cases}
        w(i,j) \quad &\text{falls} \ (i,j) \ \text{Kante im Graph}\\
        0 &\text{sonst}
    \end{cases}
$$
- Gewicht 0 nicht erlaubt
- Trennung der Zeilen durch $\#\#$


----

----
**Backlinks:**
- [📁Formale_Sprachen&Automaten](📁Formale_Sprachen&Automaten)
