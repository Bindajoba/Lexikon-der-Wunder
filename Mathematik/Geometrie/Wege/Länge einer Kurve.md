TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Hier soll die Länge einer [[Kurve]] gemessen werden.

# Motivation
Länge versucht einer Kurve $\gamma$ eine Zahl $l(\gamma)$ zuzuordnen, sodass
1) Die Länge eines [[Segment|Geradensegments]] ist gleich dem Abstand von Start- und Endpunkt.
2) Bei der [[Verkettung (Kurve)]] summiert sich die Länger der beiden Kurven.

*Mit Hilfe der Differenzierung kann man eine noch einfachere Methode entwickeltn, Kurvenlängen zu messen. Vorausgesetzt, die Kurve ist dafür geeignet.*

# Definition
Die Länge einer Kurve $\gamma: [a, b] \to \R^n$ berechnet sich durch:
$$l(\gamma):= \sup\ges{\sum_{i = 1}^{n-1}d(\gamma(t_i), \gamma(t_{i+1})):a = t_1 < t_2 < ... t_{n-1} < t_n = b}$$
wobei die $t_i$ eine Zerlegung von $[a,b]$ sind.

# Eigenschaften



$\newcommand{\ges}[1]{\left\{ #1 \right\}}$
$\newcommand{\wink}[1]{\left\langle #1 \right\rangle}$
$\newcommand{\klam}[1]{\left( #1 \right)}$
$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$



#Geometrie



