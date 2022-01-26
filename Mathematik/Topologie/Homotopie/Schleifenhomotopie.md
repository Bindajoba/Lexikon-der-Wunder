## Beschreibung
Eine **Schleifenhomotopie** ist eine [[Homotopie]] (aber keine Kurvenhomotopie!) die eine [[Stetigkeit|stetige]] Deformation einer [[Schleife]] in eine andere [[Schleife]] ist.

## Definition
Sei U [[Wegzusammenhängende Menge|wegzusammenhängend]]
Zwei [[Schleife|Schleifen]] $\gamma_0: [a, b] \to U$ und $\gamma_1: [a, b] \to U$ heißen **schleifenhomotop**, wenn es eine **Schleifenhomotopie** von $\gamma_0$ zu $\gamma_1$ gibt.

Eine **Schleifenhomotopie** $H$ von $\gamma_0$ zu $\gamma_1$ ist eine stetige Abbildung $H:[a, b]\times [0, 1] \to U$ mit den Eigenschaften:
1. *Zum Zeitpunkt 0 ist H die Schleife $\gamma_0$*
$H(t, 1)=\gamma_0(t)$ für alle $t \in [a, b]$
2. *Zum Zeitpunkt 1 ist H die Schleife $\gamma_1$*
$H(t, 0)=\gamma_0(t)$ für alle $t \in [a, b]$
3. *Während der Deformation bleibt $H$ eine Schleife*
$H(a, s)=H(b, s)$ für alle $s \in ]0, 1[$

#Mathe-IV 