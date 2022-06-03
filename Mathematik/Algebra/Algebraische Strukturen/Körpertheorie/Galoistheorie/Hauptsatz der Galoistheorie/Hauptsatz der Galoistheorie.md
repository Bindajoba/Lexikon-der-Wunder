TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Der Hauptsatz der Galoistheorie beschreibt, wie Zwischenkörper einer [[Galois-Erweiterung]] Untergruppen der [[Galoisgruppe]] zugeordnet werden können.

Es ist ja bereits bekannt, dass eine [[Galois-Erweiterung]] $L|K$ die Galoisgruppe $Gal(L|K)$ hat. Diese gibt die Menge aller [[Körperautomorphismus|Körperautomorphismen]] auf $L$ an, die $K$ gleich lassen.

Genau so kann man für eine [[Körpererweiterung]] $L|M$ eines [[Zwischenkörper]] $M$ eine entsprechende Gruppe finden:
Die Gruppe ist einfach die Menge aller Körperautomorphismen auf $L$, die $M$ gleich lassen. (Was offensichtlich eine Untergruppe von $Gal(L|K)$).

Umgekehrt betrachte eine Menge von Körperautomorphismen. Die zugehörige Erweiterung ist die Erweiterung des Körpers, der von den Automorphismen gleich gelassen wird. 



# Definition
Sei $L|K$ eine endliche [[Galois-Erweiterung]] mit [[Galoisgruppe]] $G = Gal(L|K), \mathscr{U}$ die Menge der [[Untergruppe]] von $G$ und $\mathscr{Z}$ die Menge der [[Zwischenkörper]] von $L|K$. Dann sind die Zuordnungen 
$$\phi: \mathscr{U} \to \mathscr Z, U \mapsto L^U \text{ und } \psi: \mathscr Z \to \mathscr U, ; \mapsto Gal(L|K)$$
zueinander inverse [[Bijektive Abbildung|Bijektionen]] zwischne $\mathscr U$ und $\mathscr Z$ gegeben.

# Ergänzende Aussagen
Zum Hauptsatz kommen einige Ergänzungen.

## Ergänzung 1
Sind $U_1, U_2 \in \mathscr U$ mit $U_1 \subset U_2$, dann folgt $L^{U_1} \supseteq L^{U_2}$
Sind umgekehrt $M_1, M_2 \in \mathscr Z$ mit $M_1 \subseteq M_2$, dann ist $Gal(L|M_1) \supseteq Gal(L|M_2)$

## Ergänzung 2
Es gilt $L^{\{id_l\}} = L, L^G = K$ und $Gal(L|L) = \{id_L\}, Gal(L|K) = G$

## Ergänzung 3
Ist $M$ ein Zwischenkörper und $U = Gal(L|M)$ die zugehörige Untergruppe, dann gilt $[L:M] = |U|$ und $[M:K] = (G:U)$

## Ergänzung 4
Sei $M$ ein Zwischenkörper von $L|K$ und $U = Gal(L|M)$ die zugehörige Untergruppe vn $G = Gal(L|K)$. Dann sind folgende Aussagen äquivelent
1. Die Erweiterung $M|K$ ist [[Normale Erweiterung|normal]]
2. Die Untergruppe $U$ ist [[Normalteiler]] von $G$

In diesem Fall erhalten wir durch $\sigma \mapsto \sigma|_M$ eine Abbildung $G \to Gal(M|K)$, und diese induziert einen natürlichen [[Gruppenisomorphismus|Isomorphismus]]


$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$



#Algebra 


