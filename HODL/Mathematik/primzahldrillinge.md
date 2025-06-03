---
title: Primzahldrillinge
date: 2025-05-04 05:58
tags: 
---

----

### Definition
$\{(p,p+2,p+4) \mid p,p+2,p+4 \in \mathbb{P}\}$

### Eigenschaften
**Proposition 1:** Ausser $(3,5,9)$ gibt es keine weiteren Primzahldrillinge.\
**Beweis:** Sei $p>3$ eine Primzahl. Betrachte die Tripel $(p,p+2,p+4)$. Wir
wollen zeigen, dass $(p,p+2,p+4)$ kein Primzahldrilling ist. Wir werden zeigen,
dass eine der Zahlen $p+2$ oder $p+4$ durch 3 teilbar ist.\
Wir dividieren $p$ mit Rest durch 3, und da $p>3$ eine Primzahl ist, kann der Rest
nicht 0 sein, er ist also 1 oder 2.\
i.) $p=1 \mod 3$: 
$$
 \begin{align*}
    p&=3q+1\\
    \implies p+2&=3q+3=3(q+1)
 \end{align*}
$$
Es folgt, dass $p+2$ durch 3 teilbar ist

ii.) $p=2 \mod 3$:
$$
  \begin{align*}
    p&=3q+2\\
    \implies p+4&=3q+6\\
    \implies p+4&=3(q+2)
  \end{align*}
$$
Es folgt, dass $p+4$ durch 3 teilbar ist.

----

----
**Backlinks:**
- [Primzahlen](/primzahlen)
