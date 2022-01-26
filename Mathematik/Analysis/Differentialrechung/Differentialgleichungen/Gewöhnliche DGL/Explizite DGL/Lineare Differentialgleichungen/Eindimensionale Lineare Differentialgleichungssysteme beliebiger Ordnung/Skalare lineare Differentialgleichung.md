## Beschreibung
Eine **Skalare Lineare Differentialgleichung** ist der eindimensionale Spezialfall eines [[Reelles Lineares Differentialgleichungssystem|Reellen Linearen Differentialgleichungssystems]]
Durch eine Skalare lineare DGL wird eine beliebige höhere Ableitung als affine Linearkombination vom aktuellen Zeitpunkt und Zustand beschrieben.

## Definition
Eine Skalare lineare DGL hat die Form
$$x^{(k)}(t) = c_1(t)x + c_2(t)x'+...+c_k(t)x^{(k-1)}+g(t)$$

## Lösung
Eine **Skalare Lineare Differentialgleichung** kann in ein [[Lineares Differentialgleichungssystem erster Ordnung]] umgewandelt werden:

Behandle die Ableitungen von x wie seperate Variablen:
$$\begin{align} y_1(t) 	&= x(t) \\
				y_2(t)	&= x'(t) \\
				\vdots\\
				y_k(t)	&= x^{(k-1)}(t)	\end{align}$$
Dann muss natürlich gelten: $y_1'(t) = x'(t) = y_2(t)$

Damit ergibt sich ein [[Lineares Differentialgleichungssystem erster Ordnung]]:
$$\begin{align} y_1'(t) &= y_2(t) \\
				y_2'(t)	&= y_3(t) \\
				\vdots\\
				y_k'(t)	&= c_1(t)y_1 + c_2(t)y_2+...+c_k(t)y_k+g(t)	\end{align}$$
Nach Anwendung der [[Variation der Konstanten]] ergibt sich folgende Lösung zum [[Startwertproblem]] $x(\tau) = \xi$:
$$\lambda = \begin{pmatrix}\overline{\mu_1(t)}\\\vdots\\\overline{\mu_k(t)}\end{pmatrix} \cdot \left(\Phi(\tau)^{-1}\begin{pmatrix}\xi_1\\\vdots\\\xi_k\end{pmatrix} + \int\limits_\tau^t{\Phi(s)^{-1}\begin{pmatrix}0\\\vdots\\0\\\xi_k\end{pmatrix}} \,ds \right)$$

## Spezialfall ($c_i(t)$ ist reell und konstant, g ist 0)
Hat die DGL die Form:
$$x^{(k)}(t) + a_kx^{(k-1)} ... a_2x' + a_1x = 0$$

Dann ergeben sich linear unabhängigen Lösungen aus dem [[Charakteristisches Polynom| charakteristischem Polynom]].

#Mathe-IV 