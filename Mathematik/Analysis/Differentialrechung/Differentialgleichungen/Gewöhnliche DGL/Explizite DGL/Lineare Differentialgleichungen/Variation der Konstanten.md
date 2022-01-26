## Beschreibung
Variation der Konstanten ist ein Verfahren, mit dem sich [[Lineares Differentialgleichungssystem erster Ordnung|lineare inhomogene DGLSs]] lösen lassen.

## Lösung von eindimensionalen DGLs
Eine [[Skalare Lineare Differentialgleichung erster Ordnung|skalare lineare inhomogene DGL]] $x' = f(t)x + g(t)$ zum [[Startwertproblem]] $x(\tau)=\xi$ wird durch 
$$\lambda_{(\tau, \xi)} = e^{\int\limits_\tau^t f(s) \, ds}\xi + e^{\int\limits^t_\tau f(s) \, ds}\int\limits^t_\tau e^{-\int\limits_\tau^s f(r) \, dr} f(s) \, ds$$ gelöst


## Lösung von mehrdimensionalen DGL
Ein [[Lineares Differentialgleichungssystem erster Ordnung]] $x'=A(t)x+g(t)$ zum [[Startwertproblem]] $x(\tau)=\xi$ hat die eindeutige maximale Lösung
$$\lambda_{(\tau, \xi)}(t) = \Phi(t)\Phi(\tau)^{-1}\xi + \Phi(t)\int\limits_\tau^t\Phi(s)^{-1}g(s)\,ds$$
wobei $\Phi(t)$ die [[Fundamentalmatrix]] des homogenen Teils von $(1)$ und $\Phi(t)^{-1}$ dessen Inverse zum Startzeitpunkt $\tau$ ist.[^1]

## Lösung von mehrdimensionalen DGL mit konstantem A(t)
Ist $A(t) = A \in M_d(\mathbb{R})$ also konstant, dann ist die [[Fundamentalmatrix]] $\Phi(t) = e^{tA}$.
Außerdem ist $\Phi(t)\Phi(\tau)^{-1} = e^{(t-\tau)A}$ die [[Übergangsmatrix]] für $x' = Ax$

Damit vereinfacht sich die Lösungsformel:
$$\lambda_{(\tau, \xi)}(t) = e^{(t-\tau)A}\xi + e^{tA}\int\limits_\tau^t e^{-sA}g(s)\,ds$$[^2]


#Mathe-IV 

[^1]: Zenk - Satz 19.1.13
[^2]: Zenk - Satz 19.2.4