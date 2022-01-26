## Beschreibung
Eine **Kurvenhomotopie** ist eine stetige Deformation einer [[Weg|Kurve]] in eine andere Kurve mit gleichem Anfangs- und Endpunkt.

Den Begriff Kurvenhomotopie habe ich mir zur besseren Differenzierung selbst ausgedacht. Normalerweise benutzt man den Begriff Homotopie.

## Definition
Sei U [[Wegzusammenhängende Menge|wegzusammenhängend]]
Zwei [[Weg|Wege]] $\gamma_0: [a, b] \to U$ und $\gamma_1: [a, b] \to U$ heißen **homotop**, wenn es eine **Homotopie** von $\gamma_0$ zu $\gamma_1$ gibt.

Eine **Homotopie** $H$ von $\gamma_0$ zu $\gamma_1$ ist eine stetige Abbildung $H:[a, b]\times [0, 1] \to U$ mit den Eigenschaften:
1. *Zum Zeitpunkt 0 ist H der Weg $\gamma_0$*
$H(t, 1)=\gamma_0(t)$ für alle $t \in [a, b]$
2. *Zum Zeitpunkt 1 ist H der Weg $\gamma_1$*
$H(t, 0)=\gamma_0(t)$ für alle $t \in [a, b]$
3. *Der Anfangspunkt ändert sich während der Deformation nicht*
$H(a, s)=\gamma_0(a) = \gamma_1(a)$ für alle $s \in [0, 1]$
4. *Der Endpunkt ändert sich während der Deformation nicht*
$H(b, s)=\gamma_0(b) = \gamma_1(b)$ für alle $s \in [0, 1]$

#Mathe-IV 