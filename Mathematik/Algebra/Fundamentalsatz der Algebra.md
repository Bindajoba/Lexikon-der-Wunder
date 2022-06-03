# Beschreibung
Jedes Polynom zerfällt in Linearfaktoren mit Nullstellen in $\C$


 # Definition
 Jedes nichtkonstante [[Komplexe Zahlen|komplexe]] [[Polynom (Komplexe Analysis)]] $$p: \begin{array}{rcl} \mathbb{C} & \to & \mathbb{C}\\ z & \mapsto & a_nz^n+...+a_1z+a_0 \end{array}$$ also mit $n \geq 1, c_n, ..., c_1, c_0 \in \mathbb{C}$ und $c_n \neq 0$ hat mindestens hat mindestens eine [[Nullstelle]] in $\mathbb{C}$

In dem Fall zerfällt es in eine Nullstelle und ein Restpolynom und das Polynom zerfällt induktiv in Linearfaktoren.

 # Beweis
 ## Satz von Rouche
 Der Fundamentalsatz kann mit dem [[Satz von Rouché]] ziemlich leicht bewiesen werden.
 
 Sei ein Polynom $P(z) = z^n + Az^{n-1}+Bz^{n-2}+\dots+E$
 Teile nun das Polynom auf in $P(z) = f(z)+g(z) = (z^n) + (Az^{n-1}+Bz^{n-2}+\dots+E)$.
 
 Betrachte den Kreis mit Radius $|z| = 1 + |A| + |B|+\dots+|E|$:
 Nach etwas Rechnung erhält man $f(z)>g(z)$ auf dem Rand des Kreises.
 
 Nach dem Satz von Rouché müssen $f(z) = z^n$ und $f(z)+g(z) = P(z)$ die gleiche Zahl an Nullstellen haben.

## Satz von Liouville
Der Fundamentalsatz kann auch mit dem [[Satz von Liouville]] bewiesen werden.

## Algebraischer Beweis
**Lemma 1:** Besitzt jedes nichtkonstante Pol. $f \in \R[x]$ in $\C$ eine Nullstelle dann auch jedes nicht-konstante Polynom $g \in C$.
Sei $g \in \C$, dann gilt $g\overline{g} \in \R[x]$ und nicht konstant, besitzt also Nullstellen in $\C$.

**Lemma 2**: Jedes $\R$-Polynom ungeraden grades hat mindestens eine Nullstelle in $\R$.

**Lemma 3**: Jedes $f \in \C[x]$ von Grad $2$ hat in $\C$ eine Nullstelle.
Einfach Mitternachtsformel anwenden.

**Beweis 1:**



