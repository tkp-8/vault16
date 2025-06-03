---
title: Satz von Kleene
date: 2025-05-08 13:03
tags: 
---

----

### Satz von Kleene 
Die Menge der [regulaeren Sprachen](regulaere_sprachen) und die Menge der Sprachen, die durch einen 
[regulaeren Ausdruck](regulaere_ausdruecke) beschrieben werden koennen, sind identisch

### Beweis
Verfahren: Gleichheit zweier Mengen\
Sei $R$ ein regulaerer Ausdruck und 
sei $REG$ die Menge der regulaeren Sprachen

##### 1.) $L(R)\subseteq REG$
Verfahren: Vollstaendige Induktion ueber die Anzahl der benutzten Ableitungsregeln fuer $R$\
Induktionsanfang: Wenn $R$ nur eine Ableitungsregel nutzt, gibt es nur drei Faelle:\
$R=\empty$, $R=\varepsilon$, $R=a, \ a\in \Sigma$. Die dazugehoerigen Sprachen sind  alle regulaer, 
sie endlich sind. \
Induktionsannahme: Wir nehmen an, dass die Aussage fuer RAs, die maximal $k$ Ableitungsregeln
nutzen, gilt. \
Induktionsschritt: 
Sei $R$ ein RA, der $k+1$ Ableitungsregeln benutzt. Dann koennen wir $R$ schreiben
als \
$R=(S+T), \ R=(S\cdot T)$ oder $R=(S)^{*}$. $S, \ K$: RAs, die hoechstens $k$ Ableitungsregeln
benutzen. Nach Induktionsvorraussetzung gilt $L(S)\in REG$ und $L(T)\in REG$. Da nach den 
[Abschlusseigenschaften](regulaere_sprachen) die regulaeren Sprachen unter Vereinigung, Konkatenation 
und Kleene Stern abgeschlossen sind, ist dann auch $L(R)\in REG$.


##### 2.) $REG\subseteq L(R)$
Sei $M$ ein DEA, welcher $L$ akzeptiert. Wir gehen davon aus, dass die Zustaende von 
$M=(Q,\Sigma,\delta.q_{0},F)$ mit den Zahlen von $1$ bin $n$ durchnummeriert sind, also 
$Q=\{1,\ldots , n\}$. Wir nehmen an, dass der Startzustand die Nummer $1$ hat.
Den RA $R$ werden wir aus $M$ ableiten. \
Fuer einen Lauf von Zustand $i$ zum Zustand $j$ nennen wir alle Zustaende ausser des ersten 
und des letzten Zustands einen *inneren Zustand*. \
$R_{ij}^{(k)}$: RA, der beschreibt, wie man vom Zustand $i$ zum Zustand $j$ kommt, ohne 
dabei ueber einen inneren Zustand $>k$ zu laufen.\
Ziel: Bestimmung der Ausdruecke $R_{1j}^{n}$ mit $j\in F$, denn es gilt fuer $F=\{f_{1},f_{2},\ldots, f_m\}$
$$
  R=R_{1f_{1}}^{(n)}+R_{1f_{2}}^{(n)}+\cdots+R_{1f_m}^{(n)}.   
$$
Um die $R_{ij}^{(k)}$ Ausdruecke zu bestimmen, benutzen wir einen rekursiven Ansatz. Der Basisfall
ist $k=0$:
$$
  R_{ij}^{(0)}\coloneqq \begin{cases}
    \empty, &\text{falls } i\neq j \text{ und } \{a\mid \delta(i,a)=j\}=\empty  \\
    a_{1}+a_{2}+\ldots &\text{falls } i\neq j \text{ und } a_l \in \{a\mid \delta(i,a)=j\}\\
    \varepsilon + a_{1}+a_{2}+\ldots  &\text{falls } i=j \text{ und } a_l \in \{a\mid \delta(i,a)=i\}  
  \end{cases} 
$$
Nun werden wir eine rekursive Beschreibung fuer $R_{ij}^{(k)}$ finden. Die erste Moeglichkeit 
ist, vom Zustand $i$ zu Zustand $j$ zu kommen, ohne ueber den Zustand $k$ zu laufen, also 
$R_{ij}^{(k-1)}$. Die zweite Moeglichkeit ist, vom Zustand $i$ zum Zustand $j$ zu laufen, 
und dabei den Zustand $k$ zu durchlaufen. Ein solcher Lauf kann man wie folgt aufspalten:

- der erste Teil laeuft vom Zustand $i$ zum Zustand $k$, ohne (dazwischen) einen Zustand 
$\ge k$ zu besuchen (durch $R_{ik}^{(k-1)}$ erfasst)
- ein oder mehrere Teile vom Zustand $k$ zum Zustand $k$, ohne (dazwischen) einen Zustand
$\ge k$ zu besuchen (durch $R_{kk}^{(k-1)}$ erfasst)
- der letzte Teil laeuft vom Zustand $k$ zum Zustand $j$, ohne (dazwischen) einen Zustand 
$\ge k$ zu besuchen (durch $R_{kj}^{(k-1)}$ erfasst)

$$
  R_{ij}^{(k)}=R_{ij}^{(k-1)}+R_{ik}^{(k-1)}(R_{kk}^{(k-1)})^{*}R_{kj}^{(k-1)}     
$$




----

----
**Backlinks:**
- [Regulaere Sprachen](/regulaere_sprachen)
