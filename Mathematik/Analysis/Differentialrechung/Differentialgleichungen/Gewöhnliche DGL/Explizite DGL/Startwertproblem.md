## Beschreibung

In Aufgaben zu Differentialgleichungen wird häufig ein Startwertproblem $x(t_0) = x_0$ mitgegeben.

Der Graph der Lösung des DGL, die auch das Startwertproblem löst, muss durch den Punkt $(t_0, x_0)$ verlaufen.

Obacht: Eine Funktion, die die DGL und das Startwertproblem erfüllt, muss nicht immer eindeutig sein. (Siehe Arnold)

## Definition
Seien
- $k, n \in N$ 
*$k$ ist die höchste Ableitung der Gleichung*
*$n$ ist die Dimension von der Lösung*
- $U\subseteq \mathbb{R} \times \mathbb{K}^{kn}$ ein [[Gebiet]]
*$U$ ist der Defintionsbereich der Gleichung $f$*
- $f: U \to \mathbb{K^n}$ eine [[Explizite Differentialgleichung]]

Eine [[Explizite Differentialgleichung| Lösung einer Expliziten Differentialgleichung]]$\lambda$ heißt Lösung des **Anfangswertproblems**
$$\begin{array}{c}\lambda^{(k)}=f(t, \lambda(t), \lambda'(t), ..., \lambda^{(k-1)}(t)) \\ x(t_0) = x_0, x'(t_0) = x_1, ..., x^{(k-1)}(t_0) = x_{k-1} \end{array}$$ wenn $t_0 \in I$ und 
$$\lambda(t_0) = x_0, \lambda'(t_0) = x_1, ..., \lambda^{(k-1)}(t_0) = x_{k-1}$$[^1]

#Mathe-IV 

[^1]: Zenk - Definition 17.1.6