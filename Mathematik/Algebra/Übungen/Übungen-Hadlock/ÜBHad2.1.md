TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
# Aufgabe 1 
Zeige Division mit Rest für ganze Zahlen.
Seien $m, n \in \mathbb{Z}$
Es gibt ein $q, r \in \Z$ mit $r < |n|$, sodass $m = qn+r$

Führe eine Fallunterscheidung durch:
- $m < n$: In dem Fall wähle $q = 0$ und $r = m$ und die Aufgabe ist erfüllt
- $m \geq n$: Zeige durch Induktion über $m$:
Induktionsanfang: $m = n$: Wähle $q=1$ und $r = 0$
Induktion: Sei ein $m$. Reduziere $m$ um $n < m$. Dann gibt es nach Induktionsvoraussetzung ein $q'$ und $r'$ mit $m-n = q'n + r'$.
Das lässt sich in die Form $m = (q'+1)n + r'$ bringen, was die Aufgabe löst.

# Aufgabe 2
Beweise den [[Euklidischer Algorithmus|euklidischen Algorithmus]]:
Seien $n, m \in \Z$. Zeige: der euklidische Algorithmus ergibt den $ggT(n, m)$ und es gbt zwei Zahlen $s, t \in \Z$ mit $ggT(n, m)=sn + tm$

Der euklidische Algorithmus:
$n = q_0m+ r_0$
$m = q_1r_0 + r_1$
$r_0 = q_2r_1 + r_2$
$...$
$r_{k-3} = q_{k-1}r_{k-2} + r_{k-1}$
$r_{k-2} = q_kr_{k-1} + 0$

Was solls, siehe für den Beweis [[Euklidischer Algorithmus]].

# Aufgabe 3
538

$714:264 = 2R186$
$264 : 186 = 1R78$
$186:78 = 2R30$
$78:30 = 2R18$
$30:18 = 1R12$
$18:12 = 1R6$

186
Also ist $ggT(714, 264) = 6$.
$6 = 18 - 12 = 18-(30-18) = -30 +2*18 =-30 + 2(78-2*30) =$
$=2*78-5*30 = 2*78 - 5*(186-2*78) = -5*186 +12*78 =$
$= -5*186 + 12(264-186) = 12*264-17*186 = 12*264 - 17(714-2*264) =$$=-17*714+46*264$.

Andersherum geht natürlich auch.

# Aufgabe 4
Euklidischer Algorithmus auf 
$f(x) = 2x^6-10x^5+2x^4-7x^3-15x^2+3x-15$
$g(x) = x^5-4x^4-3x^3-9x^2-4x-5$

$f:g = (2x-2)R(5x^3-18x^2+5x-25)$
$g:(5x^3-25x^2+5x-25) = \frac{1}{5}(x^2+x+1)$

# Aufgabe 6
Sei $f, g$ [[Irreduzibles Polynom]] aus $K[x]$ Zeige: Wenn sich die Polynome eine Nullstelle in einer Erweiterung teilen, dann teilt $f|g$.

Behauptung $ggT(f, g) =$ gleicher Grad wie $f$.
Angenommen dass ist nicht so, dann gibt es ein nichtkonstantes $h \in K[x]$, sodass $h*ggT(f, g) = f$. Dann ist aber $f$ nicht zerlegbar.

Wenn der ggT aber gleichen Grad wie $f$ und $g$ hat müssen diese miteinander teilbar sein.





#Hadlock 


