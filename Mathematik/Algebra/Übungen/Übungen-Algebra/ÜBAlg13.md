TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


![[blatt13.pdf]]
# Aufgabe 1
## a)
Zu zeigen:
Für Zwischenkörper $M_1, M_2$ von endlicher Erweiterung $L|K$
$M_1 \subseteq M_2$ oder umgekehrt gdw. $[L:K]$ Primzahlpotenz.

$'\implies':$ Sei $M_1 \subseteq M_2$ oder umgekehrt für zwei beliebige Zwischenkörper, dann ist $[L:K]$ eine Primzahllpotenz.
Angenommen $[L:K] = n$ wäre keine Primzahlpotenz. Dann gibt es $a, b \in \N, a, b > 1$ mit $ab = m, ggT(a, b) = 1$. 
Die Galoisgruppe hätte dann als Zyklische Gruppe von Ordnung $n$ zwei zyklische Untergruppen von Grad $a$ und $b$. Nenne die Gruppen $C_a$ und $C_b$. Dann gilt weder $C_a \subseteq C_b$ noch $C_b \subseteq C_a$ da $C_a$ als zyklische Gruppe einen Erzeuger hat, welcher nicht in $C_b$ liegt, da dazu $a\mid b$ erfüllt sein müsste. Analog ist der Erzeuger von $C_b$ nicht in $C_a$.
Zu diesen Untergruppen müsste es entsprechende Zwischenkörper $M_a = L^{C_q}$ und $M_b = L^{C_b}$ mit  $M_a \nsubseteq M_b$ und $M_b \nsubseteq M_a$ geben. Das Widerspricht aber der Voraussetzung der Aufgabenstellung. Also ist $[L:K]$ eine Primzahlpotenz.

$'\impliedby':$ Sei $[L:K] = p^n$, dann gilt für alle Zwischenkörper $M_1 \subseteq M_2$ oder umgekehrt.
Gilt $[L:K] = p^n$, dann hat die zu $L|K$ zugehörige Galoisgruppe die Ordnung $p^n$.
Die Galoisgruppe ist nach Angabe zyklisch. In einer Zyklischen Gruppe gibt es für jeden Teiler der Ordnung genau eine Untergruppe. In unserem Fall gibt es also jeweils eine Untergruppe $C_1, C_p, C_{p^2}, ..., C_{p^n}$ der Ordnung $1, p,p^2, ..., p^n$.
Für alle diese Untergruppen gilt $C_1 \subseteq C_p \subseteq ... \subseteq C_{p^n}$ und damit das was zu zeigen war.

## b)
$\alpha \in L \backslash M \implies K(\alpha) \nsubseteq M \implies M \subset (\alpha)$
Gradformel: $[K(\alpha): M ][M :K] = [K(\alpha):K]$
$K(\alpha) \supset M \implies [K(\alpha):M]>1 \implies [K(\alpha): K]>[M:K] = p^{n-1}$
Andererseits ist $[K(\alpha):K]$ wegen $p^n=[L:K(\alpha)][K(\alpha):K]$ Teiler von $p^n \implies [K(\alpha):K] = p^n \implies [L:K(\alpha)]=1 \implies L = K(\alpha)$ 



# Aufgabe 2
Sei $\alpha \in \R$ und $\beta \in \C \backslash \R$
### 1. Variante
Direktes Überprüfen der Nicht-Kommutativität.
Sei $L \subseteq \C$ der Zerf.-körper von $f$ über $\Q$ in $\C$.
Dann ist $G = Gal(f|\Q)$ gleich $Gal(L | \Q)$
$f$ irred., $\alpha \beta \in \C$ Nullstellen von $f$, Fort.-Satz $\implies$ Es gibt einen $\Q$-Homomorphismus $\sigma$ mit $\sigma(\alpha) = \beta$
Da $L|\Q$ [[Galois-Erweiterung|galoissch]] ist $\sigma$ auch ein Autmomorphismus.
Sei außerdem $\tau \in Hom_\Q(L,  \C)$ mit $\tau(\alpha) = \bar \beta$.
Beh: $\sigma \circ \tau \neq \tau \circ \sigma$
$(\tau\sigma)(\alpha) \neq \beta = (\tau\circ \tau)(\alpha)$

*Ich denke, ich habe hier einen wesentlichen Schritt falsch.*

# 2.Variante
Durch Anwendung des Hauptsatzes des Galoistheorie.
Sei $L \subseteq \C$ wie oben definiert. Die Erweiterung $\Q(\a)|\Q$ ist nicht normal, dann das über $\Q$ irred. Polynom hat die reelle Nullstelle $\alpha$, durch dess Adjunktion erhält man aber nicht $\beta$. $f$ zerfällt dann nich in Linearfaktoren.
Da $\Q(\alpha)$ nicht normal ist, ist $Gal(L|\Q(\alpha))$ kein Normalteiler von $G$. Somit kann sie nicht abelsch sein. (In einer Abelschen Gruppe ist jede Utergruppe ein Normalteiler)

![[blatt13.pdf]]


# Aufgabe 3
## a)
Die Zwischenkörper der Galoisgruppe $Gal(L|K)$ entsprechen den Untergruppen von $A_4$. $A_4$ hat $12$ Elemente. Die Untergruppenordnung teilt $12$, können also sein: $1, 2, 3, 4, 6, 12$.
$A_4 = (12)(34), (13)(24), (14)(23), (123), (124), (132), (134), (142), (143), (234), (243)$
- Ordnung $1$: Nur das Neutralelement $id$.
- Ordnung $2$: Die Untergruppen von Ordnung $2$ sind zyklisch und werden aus einem einzigen Element erzeugt. Diese müssen Ordnung $2$ haben. Es kommen somit nur die Doppeltransmutationen $(12)(34)$, $(13)(24)$ und $(14)(23)$ infrage. Diese erzeugen Unterschiedliche Untergruppen, damit gibt es $3$ Untergruppen der Ordnung $2$
- Ordnung $3$: Die Untergruppen sind zyklisch. Infrage kommen nur die 3-Zykel $(123), (124), (132), (134), (142), (143), (234), (243)$ als Erzeuger infrage. Davon sind jeweils zwei zueinander invers, sodass $4$ Untergruppen der Ordnung $3$ entstehen.
- Ordnung 4: 
Eine Gruppe der Ordnung $4$ ist isomorph zu $C_4$ oder $C_2 \times C_2$. 
$C_4$ ist zyklisch. $A_4$ hat keine solche Untergruppe, da es kein Element der Ordnung $4$ gibt.
Die Elemente $id, (12)(34), (13)(24), (14)(23)$ bilden eine Gruppe die isomorph ist zu $C_2 \times C_2$ 
$C_2 \times C_2$ hat immer $3$ Elemente der Ordnung $2$ (und das Neutralelement). Gäbe es also mehr als eine Gruppe, die Isomorph zu $C_2 \times C_2$ wäre, dann müsste es mehr als $3$ 2-Zykel geben, sonst wären diese ja gleich. Somit gibt es maximal eine Untergruppe isomorph zu $C_2 \times C_2$
Da es nur $3$ $2$-Zykel gibt, gibt es genau eine Untergruppe, die Isomorph zu $C_2 \times C_2$ ist.
- Ordnung $6$:
Nach der Angabe in c) hat $A_4$ keine Untergruppe der Ordnung $6$.
- Ordnung $12$: Nur $A_4$

Insgesamt hat also $A_4$ $1+3+4+1+1 = 10$ Untergruppen.


## b)
Sei $M$ ein Zwischenkörper von $L|K$.
$M|K$ ist eine [[Galois-Erweiterung]], wenn es separabel und normal ist.

Sei $\alpha \in M$. Das Minimalpolynom $\mu_{\alpha, K}$ ist separabel, da auch $\alpha \in L$ und die Erweiterung $L|K$ sparabel ist.
Damit ist $M|K$ separabel.

Eine Erweiterung $M|K$ ist normal, wenn die zugehörige Untergruppe $U = Gal(L|M)$ ein Normalteiler von $A_4 = Gal(L|K)$ ist. 

Suche alle Normalteiler von $A_4$. 
Nach den [[Sylowsätze]], ist eine Untergruppe genau dann ein Normalteiler, wenn es nur eine Sylowgruppe gibt. $V_4$ ist die einzige Untergruppe von Grad $4$.
Vom Grad $3$ gibt es mehrere Untergruppen. Vom Grad $2$ muss man zu Fuß zeigen, ob die [[Normalteiler]] sind.



## c)

Der oben gesuchte Zwischenkörper hat eine Zugehörige Gruppe von Ordnung $12:4 = 3$
Er soll $K(\alpha) = M$ für alle $\alpha \in M \backslash K$ erfüllen. Das gilt, wenn $M$ die kleinste echte Erweiterung von $K$ ist, bzw. wenn es keinen echten Zwischenkörper der Erweiterung $M|K$ gibt.

Das ist erfüllt, wenn es keinen Gruppe echt zwischen einer Untergruppe der Ordnung 3 von $A_4$ und $A_4$ gibt.
Die Ordnung einer solchen Gruppe muss ein echtes Vielfaches von $3$ aber ein echtes Teiler von $12$ sein. Das lässt nur $6$ zu aber da $A_4$ keine Untergruppen der Ordnung $6$ hat, kann es keine Gruppe zwischen oberen beiden Untergruppen und damit auch keinen echten Zwischenkörper von $M|K$ geben.

# Aufgabe 4
![[blatt13.pdf]]
## a)
Betrachte das Polynom ist $\Z/3\Z$. Dann verschwindet die $n$-Abhängigkeit:
$\implies f' := x^3 + 2x + 1$
Angenommen, es wäre reduzibel, dann müsste es in einen Term ersten und zweiten Grades zerfallen, d.h. eine Nullstelle in $\Z/3\Z$ haben. Es gilt aber $f'(0) = 1, f'(1) = 1, f'(2) = 2$
Damit ist $f$ nach dem Irreduzibilitätskriterium irreduzibel.

## b)
Behauptung: $f = x^2+4$ hat die angeg. Eigenschaften
$f$ ist irred. über $\Q$, denn ansonsten lägen die Nullstellen $\pm 2i$ wegen $grad(f) = 2$ in $\Q$ das tun sie aber nicht.
Da $f$ nromiert, somit insb. primitiv ist, ist $f$ auch irred. über $\mathbb{Z}$. Ang. es gibt ein $d \in \Z$, so dass auf $f(x+d)$ das Eisensteinkriterium mit einer Primzahl angewendet werden kann.
Es ist $f = (x+d)^2+4 = x^2 + 2dx + (d^2 + 4)$
- Fall $p \neq 2$:
$p \mid (2d) \implies p \mid d$
$p \mid d, p \mid (d^4+4) \implies p \mid 4 \implies p = 2$
- Fall $p = 2:$
$p \mid (d^2)+4 \implies p \mid d^2 \implies p \mid d$ Rest ist Übung für wann anders.

#Algebra 


