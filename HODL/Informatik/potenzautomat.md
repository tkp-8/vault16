---
title: Potenzautomat
date: 2025-05-07 07:44
tags: 
---

----

### Definition 
Sei $N=(Q,\Sigma,\delta,q_{0},F)$ ein [NEA](nea), dann ist der Potenzautomat
zu $N$ ein [DEA](dea) $M=(Q_P,\Sigma_P,\delta_P,q_p,F_P)$ mit   

> - $Q_P\coloneqq \mathcal{P}(Q)$
> - $\delta_P$ gegeben durch $\delta_P(P,x)\coloneqq 
E(\bigcup\nolimits_{p \in  P}\delta(p,x))$
> - $q_P\coloneqq E(q_{0})$
> - $F_P = \{P\subseteq Q \mid \exists p \in P:p \in F\}$

---

### Bemerkung
- $|Q_P|=2^{|Q|}$ Zustaende
- Zustand $\empty$ moeglich, da $\empty \in \mathcal{P}(Q)$

---

### Lemma 1
##### Sei $N=(Q,\Sigma,\delta,q_{0},F)$ ein NEA mit Potenzautomat $M_P=(Q_P,\Sigma,\delta_P,q_P,F_P)$. Dann gilt, dass fuer alle $P\subseteq Q$ und alle $w\in \Sigma ^{*}$
$$
  \delta_P^{*}(E(P),w)=\delta ^{*}(P,w)   
$$
**Beweis.** Verfahren: Vollstaendige Induktion ueber $|w|$\
Induktionsanfang: $\delta_P^{0}(E(P),\varepsilon)=E(P)=\delta ^{0}(P,\varepsilon)$ \
Induktionsannahme: Wir nehmen an, dass $\delta_P^{*}(E(P),u)=\delta ^{*}(P,u)$ gilt 
(fuer alle Woerter der Laenge $k=|u|$)\
Induktionsschritt: Es folgt fuer alle $x\in \Sigma$:

$$
\begin{align*}
  \delta_P^{k+1}(E(P),ux) &\ = \delta_P(\delta_P^{k}(E(P),u),x ) \\
 &\stackrel{I.A.}= \delta_P(\delta ^{k}(P,u),x) \quad\\
 &\stackrel{def}= E(\bigcup\nolimits_{r \in  \delta ^{k}(P,u)}\delta(r,x))\\
 &\stackrel{def}=\delta ^{k+1}(P,ux) 
\end{align*}
$$
  
---

### Satz 1
##### Sei $N$ ein NEA und $M_P$ dessen Potenzautomat, dann gilt 
$$
  L(N) = L(M_P)
$$
**Beweis.** Sei $N=(Q,\Sigma,\delta,q_{0},F)$ und $M_P=(Q_P,\Sigma,\delta_P,q_P,F_P)$
$$
\begin{align*}
  N \text{ akzeptiert } w &\Leftrightarrow \delta ^{*}(\{q_{0}\},w) \cap F \neq \empty &def  \\
  &\Leftrightarrow \delta_P^{*}(E(\{q_{0}\}),w)\cap F \neq \empty  & Lemma \ 1\\
  &\Leftrightarrow\delta_P^{*}(q_P,w)\cap F \neq \empty & def \ q_P \\
  &\Leftrightarrow \delta_P^{*}(q_P,w)\in F_P & def \ F_P\\ 
  &\Leftrightarrow M_P \text{ akzeptiert } w & def 
\end{align*}
$$
 


----

----
**Backlinks:**
- [📂Formale Sprachen Potenzautomat Automaten](/📁Formale_Sprachen%linkAutomaten)
