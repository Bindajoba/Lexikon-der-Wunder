# Beschreibung
Ein Teilring ist eine Untermenge eines [[Ring|Ringes]], welcher ebenfalls ein Ring ist und das gleiche 1-Element hat.

# Definition
Sei $R$ ein [[Ring]]. Eine Teilmenge $S \subset R$ wird **Teilring von R** genannt, wenn $1_R \in S$ gilt und mit $a, b\in S$ jeweils auch die Elemente $a-b$ und $ab$ in $S$ liegen.


*Durch das $a-b$ spart man sich das Prüfen der Inversen und Abgeschlossenheit.[^1]*

Man schreibt $R|S$

*Wahrscheinlich um auszudrücken, dass $R$ ein [[Erweiterungsring]] von $S$ ist.*
*Die Schreibweise ähnelt sehr der Schreibweise der [[Division mit Rest|Teilbarkeit]]. Ich sollte Herr Gerkmann fragen, ob es da einen Zusammenhang gibt.*

Das Gegenstück eines Teilrings wird [[Erweiterungsring]] genannt.


# Eigenschaften
### Vereinigung von Teilringen
Sei $(R, +, \cdot)$ ein Ring, und sei $(S_i)_{i \in I}$ eine [[Familie]] von [[Teilring|Teilringen]].
Dann ist auch $S = \bigcap_{i \in I}S_i$ ein Teilring von $R$


# Übungen
## Zahlentheorie Klausur 2019 Aufgabe 2
![[Zahlentheorie Klausur 2019 Aufgabe 2.png]]
### a)
- $R \subseteq \R$ 
- $1$ ist $1$-Element.
- $\frac{a}{5^n} + \frac{b}{5^m} = \frac{5^ma+5^nb}{5^{nm}} \in R$
- $\frac{a}{5^n} * \frac{b}{5^m} = \frac{ab}{5^{nm}} \in R$


### b)
Zeige erst $\subseteq$:
Sei $\frac{a}{5^n} \in R \implies a(\frac{1}{5})^n \in \mathbb{Z}[\frac{4}{5}]$, denn $\frac{1}{5} = 1- \frac{4}{5} \implies R \subseteq \Z[\frac{4}{5}]$.

Zeige $\supseteq$:
$\Z \subseteq R$ und $\frac{4}{5} \in R \implies \Z[\frac{4}{5}] \subseteq R$

## Zth Klausur 2018 Aufgabe 2
![[Zth Klausur 2018 Aufgabe 2.png]]
### a)
Offensichtlich gilt $R \subseteq \R$.
$R$ ist ein Ring, denn:
- $0, 1 \in R$ sind das Null/Einselement
- Es gilt $\frac{a}{6^n}-\frac{b}{6^m} = \frac{a6^m - b6^n}{6^{nm}} \in R$
- Es gilt $\frac{a}{6^n}\cdot\frac{b}{6^m} = \frac{ab}{6^{nm}} \in R$

$R$ und $\R$ haben das gleiche $1$-Element.

### b)
- $\supseteq:\frac{1}{6} = \frac{1}{2}\cdot\frac{1}{3} \in \Z[\frac{1}{2}, \frac{1}{3}] \implies \frac{a}{6^n} \in \Z[\frac{1}{2}, \frac{1}{3}] \implies R = \Z[\frac{1}{2}, \frac{1}{3}]$
- $\subseteq:\frac{1}{2} = \frac{3}{6} \in \Z[\frac{1}{2}, \frac{1}{3}]$ und $\frac{1}{3} = \frac{2}{6} \in \Z[\frac{1}{2}, \frac{1}{3}]$





$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$


#Zahlentheorie 

[^1]: Gerkmann Satz 3.2