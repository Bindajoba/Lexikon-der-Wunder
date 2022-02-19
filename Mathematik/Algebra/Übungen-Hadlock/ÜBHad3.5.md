TARGET DECK: Universität::Mathematik::Algebra

# Aufgabe 1
Wenn $L|K$ eine [[Galois-Erweiterung]] ist und $K_1, K_2$ Zwischenkörper sind, beschreibe $Gal(L|K_1 \cap K_2)$.

$Gal(L|K_1 \cap K_2)$ besteht aus allen Automorphismen, die den Schnitt von $K_1$ und $K_2$ gleich lassen.
Es enthält demnach alle Automorphismen, die $K_1$ oder $K_2$ gleich lassen.
Somit gilt $Gal(L|K_{1/2}) \subset Gal(L|K_1 \cap K_2)$ desweiteren erhält jeder Automorphismus von $Gal(L|K_1)$ und $Gal(L|K_2)$ $K_1 \cap K_2$. Eine Verkettung dieser Automorphismen ergibt damit wieder einen Automorphismus aus $Gal(L|K_1 \cap K_2)$.

Oder spezifischer: Es ist die kleinste Gruppe, die $Gal(L|K_1)$ und $Gal(L|K_2)$ enthält.

# Aufgabe 3
Sei $L|K$ eine Galoiserweiterung. Seien $M_1, M_2$ Zwischenkörper. Sei $M$ der kleinste Körper, der $M_1$ und $M_2$ enthält.
Was ist $Gal(L|M)$?

$Gal(L|M) = Gal(L|M_1) \cap Gal(L|M_2)$
$'\subseteq':$ Sei $\phi$ ein Automorphismus, der Elemente von $M$ fix lässt. Dann lässt er auch Elemente aus $M_1$ und $M_2$ fix.
$'\supseteq':$ Sei $\phi$ ein Automorphismus, der Elemente von $M_1$ und $M_2$ fix lässt. Dann lässt er wegen der Homormorphismuseigenschaft auch Addition/Multiplikation/Division von diesen Elementen fest. Diese Elemente bilden einen Körper, der $M_1$ und $M_2$ enthält. $M$ ist definiert, als der kleinste Oberkörper von $M_1$ und $M_2$. $\phi$ hält irgendeinen Oberkörper von $M_1$ und $M_2$ fest und damit auch $M$.

# Aufgabe 4
Sei $\zeta$ eine $5$-te Einheitswurzel. Zum Beispiel die mit Argument $72°$
Finde einen Körper $K$, sodass $[K(\zeta):K] = 2$.

Ich muss nur ein MInimalpolynom von Grad 2 finden, dass $\zeta$ als Nullstelle hat. Probieren wir:
$$(x-\zeta)(x-\bar\zeta) = x^2 - (\zeta+\bar\zeta)x+|\zeta|^2 = x^2 - 2\cos(72°)x+1$$
Was ein Polynom in $\R[x]$ ist. Anscheinend ist $\R$ schon ein solcher Körper. ($\Q(\sqrt 5)$ würde aber auch gehen)

# Aufgabe 5
Sei $\zeta$ eine $31$-te Einheitswurzel. Zum Beispiel die mit Argument $72°$
Finde einen Körper $K$, sodass $[K(\zeta):K] = 6.

$31$ ist eine Primzahl, damit ist die Galoisgruppe $Gal(\Q(\zeta)|\Q)$ zyklisch mit Ordnung $30$. Es gibt einen Automorphismus $\phi$, der $Gal(\Q(\zeta)|\Q)$ erzeugt. $\phi^5$ erzeugt eine Untergruppe der Ordnung $6$. Für diese Untergruppe gilt damit $(Gal(\Q(\zeta)|K):Gal(\Q(\zeta)|\Q(\zeta))) = 6$ Damit gibt es auch einen Zwischenkörper $K$ mit $[\Q(\zeta):K] = 6$

# Aufgabe 6
Beschreibe die Galoisgruppe von $f =x^4-2$. 
Sei $L$ der Zerfällungskörper von $f$
$f$ hat die Nullstellen $\sqrt[4]2, -\sqrt[4]2, i\sqrt[4]2, -i\sqrt[4]2$

Man erkennt, dass der Zerfällungskörper von $f$ damit $\Q(\sqrt[4]2, i)$ ist.
$\Q(\sqrt[4]2, i)$ hat den Erweiterungsgrad $8$, also muss es $8$ Automorphismen geben.
Diese sind durch die Bilder der Erzeuger $\sqrt[4]2$ und $i$ eindeutig festgelegt.

Ein Automorphismus muss Nullstellen von $x^2+1$ und $x^4-2$ auf andere Nullstellen des gleichen Polynoms abbilden.

Das Verhalten der möglichen Automorphismen kann man in einer Tabelle darstellen:

| Bilder           | $\phi_1$     | $\phi_2$      | $\phi_3$      | $\phi_4$       | $\phi_5$     | $\phi_6$      | $\phi_7$      | $\phi_8$       |
| ------------ | ------------ | ------------- | ------------- | -------------- | ------------ | ------------- | ------------- | -------------- |
| $\sqrt[4] 2$ | $\sqrt[4] 2$ | $i\sqrt[4] 2$ | $-\sqrt[4] 2$ | $-i\sqrt[4] 2$ | $\sqrt[4] 2$ | $i\sqrt[4] 2$ | $-\sqrt[4] 2$ | $-i\sqrt[4] 2$ |
| i            | i            | i             | i             | i              | -i           | -i            | -i            | -i             |


# Aufgabe 7
Bestimme aller Untergruppen der Galoisgruppe $G$ von $f = x^4-2$ und bestimme, welche Normal sind.
Wir beobachten: Die oberen Automorphismen lassen sich durch nur zwei Automorphismen $\phi := \phi_2$ und $\psi := \phi_5$ erzeugen.
- $\phi_1 = id$
- $\phi_2 = \phi$
- $\phi_3 = \phi^2$ denn $\phi^2(\sqrt[4] 2) = -\sqrt[4] 2$ und $\phi^2(-i)=-i$
- $\phi_4 = \phi^3$
- $\phi_5 = \psi$
- $\phi_6 = \phi\psi$
- $\phi_7 = \phi^2\psi$
- $\phi_8 = \phi^3\psi$

$\phi$ hat Ordnung $4$. Damit kann es sich nur noch um $C_2 \times C_4, D_4$ oder die Quaternionengruppe $Q_4$ handeln. Die Art, wie $\phi$ die Nullstellen von $x^4-2$ dreht und $\psi$ diese an der reellen-Achse spiegelt sieht mir sieht es aber sehr nach [[Diedergruppe]] aus.
Durch nachrechnen oder Zeichnen von [[Cayley-Diagramm]] bekommt man als Normalteiler: $\{id, \phi^2\}, \{id, \phi, \phi^2, \phi^3\}, \{id, \phi^2, \phi\psi, \phi^3\psi\}, \{id, \phi^2, \psi, \phi^2\psi\}$.
Untergruppen, die keine Normalteiler sind, sind:
$\{id, \psi\}, \{\phi\psi\}, \{\phi^2\psi\}, \{\phi^3, \psi\}$

# Aufgabe 8
Wenn $L|M$ und $M|K$ [[Normale Erweiterung|normal]], ist dann $L|K$ normal?

Sei $f$ ein Irreduzibles Polynom in $K[x]$ mit Nullstelle in $L$.
Dann ist $f$ auch ein Polynom in $M[x]$ und zerfällt in $M$ in irreduzible Polynome. Diese müssen aber keine Nullstelle in $L$ haben, deshalb geht der Beweis nicht!

Die Aussage ist falsch! Betrachte die obere Diedergruppe:
$\{id, \psi\}$ ist ein Normalteiler von $\{id, \phi^2, \psi, \phi^2\psi\}$
$\{id, \phi^2, \psi, \phi^2\psi\}$ ist ein Normalteiler von $D_4$

Aber $\{id, \psi\}$ ist kein Normalteiler von $D_4$.
Damit gilt das auch für Körper nicht!

# Aufgabe


















$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


#Hadlock 