---
title: Kontextfreie Grammatiken
date: 2025-05-09 06:35
tags: 
---

----

### Definition 
##### kontextfreie Grammatik
[Grammatik](grammatiken) $G=(V,\Sigma,P,S)$ mit einer eingeschraenkten Menge von Produktionsregeln
$$
  P \subseteq \{(L,R)\mid L\in V, R\in (V\cup \Sigma)^{*}\}  
$$

##### Sprache einer kontextfreien Grammatik
Die [Sprache](sprachen) einer kontextfreien Grammatik $G=(V,\Sigma,P,S)$ ist definiert als
$$
  L(G)\coloneqq \{w\mid S\Rightarrow ^{*} w \}  
$$

---

### Beispiel
$G_{1}=(\{S\},\{\texttt{a},\texttt{b}\},\{(S,\texttt{a}S\texttt{b}),(S,\varepsilon)\},S)$   
Kurz: $S\to \texttt{a}S\texttt{b}\mid \varepsilon$\
[Woerter](woerter), die wir aus $G_{1}$ ableiten koennen:
 
- $S\Rightarrow \varepsilon$
- $S\Rightarrow \texttt{a}S\texttt{b}\Rightarrow \texttt{ab}$

Also ist die Sprache von $G_{1}$
$$
  L(G_{1})=\{\texttt{a}^{n}\texttt{b}^{n}\mid n\ge 0  \}  
$$

---

### Ableitungsbaum
Folgende Bedingungen muss ein Ableitungsbaum einer kontextfreien Grammatik $G$ erfuellen

- Alle **inneren Knoten** sind mit Variablen beschriftet und in der **Wurzel** steht das Startsymbol
- Alle **Blaetter** sind mit Terminalsymbolen oder $\varepsilon$ beschriftet
- Wenn ein innerer Knoten die Beschriftung $X$ aufweist, und seine Kinder (von links nach rechts)
mit $x_{1},x_{2},\ldots x_k$ beschriftet sind, dann muss es in $G$ die Regel $X\to x_{1},x_{2},\ldots ,x_k$ 
geben

----

### Chomsky Normalform
[CNF](cnf)

----
**Backlinks:**
- [📂Formale Sprachen kontextfreie_grammatiken Automaten](/📁Formale_Sprachen%linkAutomaten)
