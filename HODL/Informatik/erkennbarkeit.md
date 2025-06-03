---
title: Erkennbarkeit
date: 2025-05-24 11:05
tags: 
---

----

### Definition
##### Erkennbarkeit

Wir nennen eine [Sprache](sprachen) $L$ *erkennbar*, falls es ein Python-Programm $P$
mit einem Eingabeparameter $w$ gibt, welches genau dann eine 1 ausgibt, wenn $w\in L$.

##### Standardnummerierung von $\Sigma$
Bijektion zwischen den natuerlichen Zahlen und den Woertern ueber einem [Alphabet](alphabet) $\Sigma$.\
Woerter werden der Laenge nach nummeriert und Woerter gleicher Laenge werden gemaess der 
Ordnung von $\Sigma$ geordnet.

##### Ueberzaehlbare Menge
Eine Menge $M$ ist Ueberzaehlbar wenn es keine Bijektion zu den natuerlichen Zahlen fuer sie 
gibt.

---

### Notation
**Ergebnis, das vom Python-Programm $P$ mit Eingabe $w$ berechnet wird**\
$P(w)$

**Von einem Python-Programm erkannte Sprache**\
$L(P)$

---

### Lemma 1
##### Die Menge $\{L \subseteq \Sigma ^{*} \}$ aller Sprachen ueber $\Sigma$ ist ueberzaehlbar.
**Verfahren:** Diagonalisierungsverfahren

**Beweis.** Sei $L_i$ die $i$-te Sprache in der abgeleiteten Nummerierung. Wir tragen alle 
Sprachen in eine unbeschraenkte Tabelle $T$ ein. Hierbei werden wir $L_i$ in die $i$-te Zeile
eintragen. Die Spalten von $T$ sind mit Woertern aus $\Sigma ^{*}$ beschriftet. Die beschriftung
der $i$-ten Spalte bezeichnen wir mit $w_i$. Wir markieren die Woerter, welche in $L_i$ enthalten
sind, indem wir in der korrespondierenden Zeile eine 1 eintragen. Wenn nicht 0. So 
koennen wir jede Sprache aus $L$ als eine unendliche Sequenz von 0en und 1en angeben. Diese 
Folge nennen wir die **Signatur der Sprache**. Wir konstruieren nun eine Sprache $L^{\prime}$, 
welche in der Nummerierung der $L_i$ fehlt. Dazu negieren wir die Diagonale der Tabelle und 
interpretieren die so erhaltene Folge als Signatur von $L^{\prime}$.
$$
  L^{\prime}\coloneqq \{w_i\mid w_i\notin L_i\}   
$$
Die Sprache $L^{\prime}$ fehlt in der Nummerierung der $L_i$, da sie sich von jeder dieser
Sprachen unterscheidet. 

---

### Korollar 1
##### Es gibt Sprachen die nicht erkennbar sind.

**Beweis.** Nach Lemma 1 gibt es keine Bijektion zwischen der Menge der Python-Programme und
der Menge aller Sprachen ueber $\Sigma ^{*}$. Somit gibt es auch keine Bijektion zwischen den
erkennbaren Sprachen ueber $\Sigma$ und allen Sprachen ueber $\Sigma$.


----

----
**Backlinks:**
- [📂Berechenbarkeitstheorie](/📁Berechenbarkeitstheorie)
