TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$


![[blatt12.pdf]]

# Aufgabe 0
## a)
Elemente sind Nullstellen von $x^{p^n}-x$

## b)
Minimalpolynom $\mu_{K,\alpha}$ ist Teiler von $f$ ein $K[x]$

## c)
$L|K$ normal, wenn sie algebraisch ist und jedes über $K$ irred. Polyno $f \in K[x]$, welches in $L$ eine Nullstelle besitzt, zerfällt über $L$ in Linearfaktoren.

$grad=2 \implies L|K$ normal
endliche Körpererw. $L|K$ gdw. $L$ Zerfällungskörper eines Polynoms $f \in K[x]$ über $K$ ist.
endliche Erweiterung $L|K$ normal gdw. $Hom_K(L, \tilde K) = Aut_K(L)$, wobei $\tilde K$ ein bel. alg. abg Erweiterungskörper von $L$ ist.

## d)
![[Separables Polynom]]


$f = x^p - 2$, $f' = px = 0$ in $\F_p$.
$f$ ist nicht seperabel, da $ggT(f, f') = f \neq 1$

# Aufgabe 1
![[blatt12.pdf]]

## a)
$f = x^q-x = x^{p^n}-x$
$\iff:$ zz. $grad(g) = d, g|f \implies d|n$

$grad(g) = d$ und $g$ irreduzibel und o.E normiert. Dann ist $g$ ein Minimalpolynom zu einer Nullstelle $\alpha$. 
$g$ teilt $f$. Damit ist jede Nullstelle von $g$ eine Nullstelle von $f$.
Den Zerfällungskörper von $§$ 

$\F_p^{alg}$ alg. Abschluss von $\F_p, \alpha \in \F_p^{alg}$ Nst. von $g$.
Dann ist $g$ ein Minimalpolynom von $\alpha$, d.h $[\F_p(\alpha): \F_p] = grad(g) = g \implies \F_p(\alpha) = \F_{p^d}$ (aufgrund der Vektorraumstruktur).

$\alpha$ ist auch eine Nullstelle von $f$. $\F_{p^n}$ ist der Zerfällungskörper von $f$, damit gilt $\F_{p^d} \subseteq \F_{p^n}$ gdw. $d|n$.

## b)
Sei $f = g_1, ..., g_r$ eine Zerlegung von $f$ über $\F_p$ irred., normierte Faktoren $g_k = \F_P[x], 1 \leq k \leq r$. Die Nullstellen von $f$ sind genau die $p^n$ verschiedenen Elemente von $\F_p \implies$ Faktoren $g_i$ verschieden.

Der Grad dieser Polynome ist nach (a) ein Teiler von $n$
Sei $g \in \F_p[x]$ ein beliebiges irr. Polynom dessen Grad ein Teiler von $d$ ist, dann ist $g$ nach (a) ein Teiler von $f \implies g$ muss mit einem $g_k$ übereinstimmen.

## c)
Nach b) ist $x^9 -x = x^{3^2}-x$ ein Produkt aller normierten, irred. Polynomen, deren Grad 2 teilt.
Diese Polynome können sein:
- $x$ (!)
- $x+1$ (!)
- $x+2$ (!)
- $x^2$
- $x^2+1$ (!)
- $x^2+2 = x^2-1 = (x+1)(x-1)$
- $x^2+x$
- $x^2+x+1$, durch 1 teilbar
- $x^2+x+2$ (!)
- $x^2+2x$ 
- $x^2+2x+1$
- $x^2+2x+2$ (1)

D.h.
$f = x(x+1)(x+2)(x^2+1)(x^2x+2)(x^2+2x+2)$

## d)


#Algebra 


