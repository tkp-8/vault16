---
title: Das_Sieb_des_Eratosthenes
date: 2025-05-03 10:20
tags: algorithmus
---

----

### Algorithmus 
##### Sei $n\in \mathbb{N}$. Die Ausgabe ist die Liste aller Primzahlen $\le n$.
1. (Initialisierung) Sei $P=[2,3,\ldots,n]$ die Liste der Zahlen von 2 bis $n$.
   Sei $i=1$. (Wir benutzen $p_i$ zur Berechnung des $i$-ten Elements in $P$.)
2. (Sind wir fertig?) Wenn $p_i$ nicht existiert oder $p_i>\sqrt{n}$, gehe zu Schritt 4. 
3. (Streiche Vielfache von $p_i$) Streiche alle $kp_i$ von $P$, fuer die $k\in \mathbb{N}$
   und  $2\le k\le \frac{n}{p_i}$ gilt. Setze so lange $i$ auf $i+1$, bis $p_i$ die naechste
   nicht gestrichene Zahl in der Liste ist, und gehe zu Schritt 2.
4. (Ausgabe) Gib $P$ aus und beende den Algorithmus.





----

----
**Backlinks:**
- [📂Elementare_Zahlentheorie](/📁Elementare_Zahlentheorie)
