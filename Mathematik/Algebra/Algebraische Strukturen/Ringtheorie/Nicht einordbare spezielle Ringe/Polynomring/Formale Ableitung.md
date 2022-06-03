TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Die Formale Ableitung ist eine Operation. Sie erlaubt es, ein [[Polynom (Ring, Körper)|Polynom]] in ein anderes Polynom umzuwandeln, als hätte man eine [[Ableitung]] verwendet.
Formale Ableitung wird oft im Zusammenhang mit nicht-[[Stetigkeit|stetigen]] [[Ring|Ringen]] oder [[Körper|Körpern]] verwendet. Eine Ableitung im herkmmlichen Sinne ist daher nicht definierbar. Daher nennt man diese formal.

# Definition
Die Formale Ableitung entspricht der [[Ableitung]]. Im Gegensatz zu ihr ist diese aber nur durch eine formale Anwendung der Ableitungsregeln definiert.

Sei $K$ ein [[Körper]] und $f = \sum_{k=0}^n a_k x^k \in K[x]$, mit $n \in \mathbb{N}_0$ und $a_i \in K$.
Dann nent man 
$$f' = \sum_{k=1}^n k a_{k}x^{k-1}$$
die **formale Ableitung** von $f$[^1]


# Übungen
## McEliece Übung 6-1
Zeige dass einige Regeln der gewöhnlichen Regeln hier ebenfalls gelten

### a)
Die Additionsregel gilt offensichtlich: $(P+Q)' = P' + Q'$

### b)
Zeige, dass die Produktregel $(PQ)' = PQ'+P'Q$ gilt.
$$\begin{align}(PQ)' &= (\sum_{i=0}^n p_ix^i\sum_{j=0}^m q_ix^i)'\\
&= (\sum_{k = 0}^{n+m}(\sum_{i+j=k}p_iq_j)x^k)\\
&= (\sum_{k = 1}^{n+m}(\sum_{i+j=k}p_iq_j)kx^{k-1})\end{align}$$
Von der anderen Seite:
$$\begin{align}PQ'+P'Q &= (\sum_{i=0}^n p_ix^i)(\sum_{j=0}^m q_ix^i)'+(\sum_{i=0}^n p_ix^i)'(\sum_{j=0}^m q_ix^i)\\
&= (\sum_{i=0}^n p_ix^i)(\sum_{j=1}^m jq_jx^{j-1})+(\sum_{i=1}^n ip_ix^{i-1})(\sum_{j=0}^m q_jx^j)\\
&= (\sum_{k = 1}^{n+m}(\sum_{i+j=k}jp_iq_j)x^{k-1})+(\sum_{k = 1}^{n+m}(\sum_{i+j=k}jp_iq_j)x^{k-1})\\
&= \sum_{k = 1}^{n+m}(\sum_{i+j=k}(i+j)p_iq_j)x^{k-1}\\
&= \sum_{k = 1}^{n+m}(\sum_{i+j=k}p_iq_j)kx^{k-1}\\
&= (PQ)'\end{align}$$
### c)
Zeige $(P^m)' = mP^{m-1}P'$
Beweise das durch vollständige Induktion:
Induktionsanfang $(n = 1)$
$(P^1)' = P' = 1P^0P'$

Induktion $(n+1)$
$$(P^{m+1})' = (P\cdot P^m)' = P(P^m)'+P'(P^m) = PmP^{m-1}P'+P'P^m = P'P^m(m+1)$$

### d)
Sei $P = P_1^{e_1} ... P_m^{Pe_m}$ eine Faktorisierung eines Polynoms in irreduzible Polynompotenzen.
Zeige:
$$\frac{P}{ggT(P, P')} = P_1 ...  P_m$$
Zeige durch vollständige Induktion über $m$.
Induktionsanfang $m = 1$:
$$P = P_1^{e_1} \implies \frac{P_1^{e_1}}{ggT(P_1^{e_1}, P_1^{e_1-1}P_1')}=\frac{P_1^{e_1}}{P_1^{e_1-1}} = P_1$$
Denn $ggT(P_1^{e_1}, P_1^{e_1-1}P_1') = P_1^{e_1-1}$. $P_1$ und $P_1'$ müssen nämlich teilerfremd. Wären sie es nicht. Dann wäre $ggT(P_1, P_1') \neq 1$ und es gäbe somit ein Polynom welches das irreduzible Polynom $P_1$ teilt.

Induktion $(m+1)$:
$$\begin{align}\frac{P}{ggT(P, P')} &=\frac{\bar P P_{m+1}^{e_{m+1}}}{ggT(\bar PP_{m+1}^{e_{m+1}}, (\bar PP_{m+1}^{e_{m+1}})')}\\
&= \frac{\bar P P_{m+1}^{e_{m+1}}}{ggT(\bar PP_{m+1}^{e_{m+1}}, \bar P'P_{m+1}^{e_{m+1}} + \bar P (P_{m+1}^{e_{m+1}})' )} \\
&= \frac{\bar P P_{m+1}^{e_{m+1}}}{ggT(\bar PP_{m+1}^{e_{m+1}}, \bar P'P_{m+1}^{e_{m+1}} + \bar P (P_{m+1}^{e_{m+1}-1}P_{m+1}') )} \\
&= \frac{\bar P P_{m+1}^{e_{m+1}}}{ggT(\bar PP_{m+1}^{e_{m+1}}, P_{m+1}^{e_{m+1}-1}(\bar P'P_{m+1} + \bar P P_{m+1}'))} \\
&= \frac{\bar P P_{m+1}^{e_{m+1}}}{ggT(\bar PP_{m+1}^{e_{m+1}}, P_{m+1}^{e_{m+1}-1}(\bar PP_{m+1})')} \\
&= \frac{\bar P P_{m+1}^{e_{m+1}}}{P_{m+1}^{e_{m+1}-1}ggT(P, P')} \\
&= \frac{\bar P }{ggT(P, P')}P_{m+1} \\
&= P_1...P_mP_{m+1} \\
\end{align}
$$

Zeige des Weiteren, dass $P$ genau dann in einfache irreduzible Polynome zerfällt, wenn es mit seiner Ableitung teilerfremd ist.
Aus oberer Gleichung folgt:
$$P = ggT(P, P')P_1 ...  P_m$$
Man erkennt, das der $ggT=1$, damit $P = P_1...P_m$.

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Algebra 


