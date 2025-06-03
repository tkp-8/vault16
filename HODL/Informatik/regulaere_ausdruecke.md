---
title: Regulaere Ausdruecke
date: 2025-05-07 05:47
tags: 
---

----

### Definition 
##### Regulaerer Ausdruck (RA)
Fuer ein [Alphabet](alphabet) $\Sigma$ bezeichnen wir [Woerter](woerter) ueber 
$\Sigma \cup \{(,),*,+,\cdot,\empty,\varepsilon\}$, die nach folgenden Regeln 
gebildet wurden, als regulaere Ausdruecke:

- $\empty,\varepsilon$ sind regulaere Ausdruecke
- fuer jedes $a \in \Sigma$ ist $a$ ein regulaerer Ausdruck
- wenn $S$ und $T$ regulaere Ausdruecke sind, dann auch $(S+T),(S\cdot T)$ und $(S)^{*}$

##### Sprache eines RA
Sei $R$ ein RA, dann bezeichnen wir dessen Sprache mit $L(R)$. Die Sprache $L(R)$ definiert sich
induktiv wie folg ($S$ und $T$ sind andere RAs)

- $R=\empty\implies L(R)=\empty$
- $R=a, \ a\in \Sigma \cup \{\varepsilon\} \implies L(R)=\{a\}$
- $R=(S+T)\implies L(R)=L(S)\cup L(T)$
- $R=(S\cdot T)\implies L(R)=L(S)\circ L(T)$
- $R=(S)^{*} \implies L(R) = L(S)^{*}$

--- 

### Konzept
- Beschreibung der Struktur der Woerter
 
---

### Beispiele
1.) $R_{1} = (\texttt{0}+\texttt{1})^{*}\texttt{0101}(\texttt{0}+\texttt{1})^{*}$
 
- $\Sigma=\{\texttt{0},\texttt{1}\}$
- **Praefix:** $(\texttt{0}+\texttt{1})^{*}$, also ein wort aus $\Sigma ^{*}$ 
- **Teilwort:** $\texttt{0101}$
- **Suffix:** $(\texttt{0}+\texttt{1})^{*}$, also ein wort aus $\Sigma ^{*}$ 
$$
  L(R_{1})=\{w\in \Sigma ^{*}\mid w \text{ enthaelt} \texttt{ 0101 } \text{als Teilwort}\}  
$$

2.) $R_2=\empty+(\texttt{b}^{*}\texttt{ab}^{*}\texttt{ab}^{*})^{*}$ 

- $\Sigma = \{\texttt{a},\texttt{b}\}$
- $(\texttt{b}^{*}\texttt{ab}^{*}\texttt{ab}^{*})^{*}$: genau zwei $\texttt{a}$s und 
  beliebig viele $\texttt{b}$s davor und dahinter
$$
\begin{align*}
   L(R_{3}) &= L(\empty) \cup \{w\in \Sigma ^{*} \mid w \text{ enthaelt gerade Anzahl an } \texttt{a}s\}\\ 
  &= \{w\in \Sigma ^{*} \mid w \text{ enthaelt gerade Anzahl an } \texttt{a}s\}  
\end{align*}
$$

---

### Satz 1
##### Sei $R$ ein regulaerer Ausdruck, dann ist $L(R)$ regulaer
**Beweis.** [Satz von Kleene](satz_von_kleene)




----

----
**Backlinks:**
- [Regulaere Sprachen](regulaere_sprachen)
