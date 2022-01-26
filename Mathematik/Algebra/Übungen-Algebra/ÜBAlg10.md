$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
![[AlgÜB10.pdf]]


# Aufgabe 1
a)

$K' := \mathbb{Q}(\sqrt{2}, i) = \mathbb{Q}(\sqrt{2})(i)$
Damit ist $\mathbb{Q}(\sqrt 2)$ ein Zwischenkörper von $K'$ und $\mathbb{Q}$ und es gitl die Gradformel:
$$[K':\mathbb{Q}] = [K' : \mathbb{Q}(\sqrt 2)] \cdot [\mathbb{Q}(\sqrt 2):\mathbb{Q}]$$
Beh.: $f(x)=x^2-2$ ist das Minimalpolynom von $\sqrt{2}$ in $\mathbb{Q}$, da $f$ normiert und $f(\sqrt 2) = 0$
Angenommen, $f$ ist reduzibel über $\Q$. Wegen $grad(f) = 2$ liegen dann die Nullstellen $\pm \sqrt{2}$ in $\Q$ (Widerspruch)
$\implies [\mathbb{Q}(\sqrt 2):\mathbb{Q}] = 2$
$x^2+1 = (x+i)(x-i)$ ist normiert, in $\mathbb{Q}(\sqrt 2) \subset \mathbb{R}$ irreduzibel, da $\pm i \notin \mathbb{R}$ und hat Grad $2$. $\implies [K' : \mathbb{Q}(\sqrt 2)] = [\Q(i)(\sqrt 2):\Q(\sqrt 2)] = 2$. 

Damit ist: $[K' : \mathbb{Q}] = 2\cdot 2 = 4$

Sei $h = x^3-2 \in \Q[x]$. $h$ normiert. $h(\sqrt[3]2) = 0$, $h$lt. Angabe irreduzibel 
$\implies h = \mu_{\sqrt[3]2, \Q} \implies [\Q(\sqrt[3]2 : \Q)] = grad(h) = 3$

$h \in \Q(\sqrt 2, i)[x], h(\sqrt[3]2) = 0 \implies \mu_{\sqrt[3]2, \Q(\sqrt, i)}$ teilt $h \implies grad(\mu_{\sqrt[3]2, \Q(\sqrt, i)}) \leq grad(h) = 3$.
$\implies [K:\Q] = [K:K'] \cdot [K':\Q] \leq 3\cdot 4 = 12$

Andererseits: $\Q(\sqrt[3]2)$ ist Zwischenkörper von $K|\Q$
$grad(f) \implies [K:\Q] = [K:\Q(\sqrt[3]2)]\cdot [\Q(\sqrt[3]2, \Q)] = [K:\Q(\sqrt[3]2)]\cdot 3 \implies$ 3 teilt $[K:\Q]$
$K'$ ist Zwischenkörper von $K |\Q \implies [K_\Q ]= [K: K'] \cdot [K': \Q] = [K:K']\cdot 4 \implies 4$ teilt $[K:\Q]$.

$[K:\Q]$ wird durch $3$ und $4$, also auch $kgV(3, 4) = 12$ geteilt. D.h. $[K:\Q]\geq 12$

$\implies [K:\Q] = 12$


b)

Bestimme die Anzahl der $\mathbb{Q}$-Homomorphismen $\phi: \Q (\sqrt[3]2) \to \mathbb{C}$ mit $\phi(\sqrt[3] 2) = \zeta\sqrt[3]2$.
Ein $\Q$-Homomorphismus bildet die Nullstelle $\sqrt[3]2$ der Funktion $x^3-2$ nach dem Prinzip Nullstelle auf Nullstelle ab.
Für jedes mögliche Bild ist der Homomorphismus nach Vorlesung eindeutig festgelegt. $\zeta \sqrt[3]2$ ist eine Nullstelle von $x^3-2$. Somit existiert genau eine Funktion $\phi$ mit den oberen Voraussetzungen.

Wie viele Fortsetzungen von $\phi$ auf $\Q(\sqrt[3]2, i)$ gibt es?
$x^2+1 = (x+i)(x-1)$ ist in $\Q(\sqrt[3]2)$ wegen $i \notin \mathbb{R}\supseteq\Q(\sqrt[3]2)$ irreduzibel, normiert und ist damit Minimalpolynom von $i$ in $\Q(\sqrt[3]2)$.
Nach dem Fortsetzungssatz gibt es genau eine Fortsetzung $\psi$ von $\phi$, die die Nullstelle $i$ von $x^2+1$ auf die andere Nullstelle $-i$ abbildet.

Nach Vorlesung ist ein $\Q$-Homomorphismus eindeutig definiert, wenn die Bilder wir die Bilder seiner Erzeuger kennen. $\sqrt[3]2, i$ erzeugen $\Q(\sqrt[3]2, i)$, daher ist $\psi$ der einzige Homomorphismus auf $\Q(\sqrt[3]2, i)$ mit $\psi(\sqrt[3]2) = \zeta \sqrt[3]2$ und $\psi(i) = -i$ 

Wie viele Fortsetzungen von $\psi$ auf $K_0 = \Q(\sqrt[3]2, i, \sqrt 2)$ gibt es?
Jeder $\Q$-Hom $\sigma: K \to \C$ mit $sigma(\sqrt[3]2 = \zeta\sqrt[3]2)$ und $\sigma(i) = -i$ ist eine Fortsetzung von  von $\psi$, da $\sigma|_{K_0}(\sqrt[3]2) = \psi(\sqrt[3]2), \sigma|_{K_0}(i) = \psi(i)$ und $\psi$ wie eben beschrieben der einzige Homomorphismus mit der Eigenschaft ist.

Gesucht ist die Anzahl der Fortsetzungen von $\psi$ auf $K= K_0(\sqrt 2)$
Beh.: $\mu_{\sqrt 2, K_0} = x^2-2 = f$
$f$ ist normiert, und hat Nullstelle $\sqrt 2$.
Angenommen $f$ ist reduzibel über $K_0$. Da $grad(f) = 2$ gilt $\pm \sqrt 2 \in K_0$
$\implies [K:K_0] = [K_0(\sqrt 2: K_0] = 1$
$[K_0: \Q(\sqrt[3]2)] = [\Q(\sqrt[3]2, i): \Q(\sqrt[3]2)] = 2$
$grad f \implies [K_0 : \Q] = [K_: \Q(\sqrt[3]2)]\cdot [\Q(\sqrt[3]2:\Q)] = 2 \cdot 3 = 6$
$grad f \implies [K: \Q] = [K:K_0] \cdot [K_0 : \Q] = 1\cdot 6 = 6$
widerspruch zu a)

...

Es gibt zwei Fortsetungen von $\psi$ auf $K$.

## c)
Das Element $\sqrt[3]2$ sit Nullst. von $h = x^3 -1$.
Angenommen es gibt ein $\Q$-Hom. $\tau$ wie in Aufgebenstellung. Dann müsste das Bild $\tau(\sqrt[3]2) = 1+i$ wieder Nullstelle von $h$ sein.
Aber: $(1+i)^3-2 = 2(1-i)-1 \neq 0$

# Aufgabe 2

# Aufgabe 3
## a)
Zu Zeigen: $\zeta, \zeta^2, \zeta^4, \zeta^5$ sind Nullstellen von $g = x^4+x^2+1$. Das sieht man durch Einsetzen.


## b)
$g$ teilt $f$, damit hat $f$ die Nullstellen von $g$.

## c)
Nach Definition des Zerfällungskörper gilt:
$L = \Q(N)$, wobei $N$ die Menge der Nullstellen von $f$ in $\C$ ist.
Die Zahlen $\{\zeta, \zeta^2, \zeta^4, \zeta^5, \sqrt 3, -\sqrt 3\}$ sind Nullstellen von $f$. Da es $6 = grad(f)$ verschiedene Elemente sind, sind das alle Nullstellen von $f$. 

Beh.: $\Q(\sqrt{-3} = \Q(N)$
$\subseteq:$ klar
$\supseteq:$ Die Potenzen von $\zeta$, sind mit $\zeta$ erzeugbar. $\zeta = 1/2 + \frac{1}{2}\sqrt{-3}$ und $\pm\sqrt{-3}$ ist durch $\sqrt{-3}$ und Elementen aus $\Q$ erzeugbar. $\implies N \subset \Q(\sqrt{-3})$

$[L:\Q] = [\Q(\sqrt{-3}):\Q] =2$
Da $x^2-3$ das Minimalpolynom von $\sqrt{-3}$ ist.


# Aufgabe 4
## a) 
Zu Zeigen: $x$ ist in $\Z[x]$ ein [[Primelement]].

$x$ ist im Hauptidealring genau dann ein Primelement, wenn $(x)$ ein Primideal ist.
$(x)$ ist genau dann ein Primideal, wenn $\Z[x]/(x)$ ein Integritätsbereich ist.

Verwende den Auswertungshomomorphismus $\phi$, der $x$ auf $0$ abbildet. Zeige
- $\phi$ ist surjektiv
Sei $a\in \Z$ vorgegeben. Dann gilt $\phi(a) = a$
- $ker(\phi) = (x)$
Für ein Polynom $f$ gilt $\phi(f) = 0$, genau dann wenn der letzte konstante Koeffizient $0$ ist. Genau diese Polynome sind durch $x$ teilbar und bilden damit $(x)$

%%
Definiere die Abbildung $\phi: \Z[x] \to \Z, f=a_nx^n + ... a_1x + a_0 \mapsto a_0$.
$\phi$ ist ein Ringhomomorphismus, da
- $\phi(1) = 1$
- $\phi(f + g) = \phi((f' + f_0)+(g'+g_0)) = \phi((f'+g')+(f_0+g_0)) = f_0 + g_0 = \phi(f) + \phi(g)$
Wobei $f_0, g_0$ der konstante Koeffizient der Polynome $f, g$ ist und $f', g'$ der Rest.
- $\phi(fg) = \phi((f'+f_0)(g'+g_0)) = \phi(f'g' + f'g_0 + g'f_0 + f_0g_0) = \phi(f_0g_0) = \phi(f)\phi(g)$
%%
$im(f) = \Z$ und $\Z[x]/(x)$ sind isomorph.
$\implies \Z[x]$ ist ein Integritätsbereich.


Zu Zeigen: $(2, x)$ ist ein maximales Ideal in $\Z[x]$

Wende den Homomorphismus für Ringe auf $\bar \phi = \pi \circ \phi$, wobei $\pi : \Z \to \Z/2\Z = \F_2$ den kan- Epimorphismus $a\mapsto a+2\Z$ bezeichnet.
$\bar \phi$ ist als Komposition zweier surj. Ringhomomorphismen ist auch $\bar \phi$ ein surjektiver Ringhomomorphismus

*Meine Lösung ist dazu gannz ähnlich. Siehe unten.*

Behauptung: $(2, x) = \{a\cdot 2 + b \cdot  x: a, b \in \Z[x]\} = \{a_nx^n + ... + a_1x + a_0: a_k \in \Z, a_0 \text{ gerade}\}$
$\subseteq:$ Sei $f \in \{a\cdot 2 + b \cdot  x: a, b \in \Z[x]\}$. Offensichtlich ist der letzte Koeffizient von $f$ gerade.
$\supseteq:$ Sei $f \in \{a_nx^n + ... + a_1x + a_0: a_k \in \Z, a_0 \text{ gerade}\}$. Dann gilt $f = (a_nx^{n-1}+a_1)x + a_0$, wobei $a_0$ es ein $b \in \Z$ gibt, sodass $a_0 = 2b$


$(2, x)$ ist genau dann ein Maximales Ideal, wenn $\Z[x]/(2, x)$ ein [[Körper]] ist.

$(2, x) = \{2, x, 0, 4, 6, 8, ..., x^2, x^3, x^4, ..., 2x, 3x, 4x, 5x, ..., 2x^2, 3x^2, 4x^2, 5x^2, ...\}$

Definiere die Abbildung $\psi: \Z \to \mathbb{F}_0, n \mapsto 0$ wenn gerade, $1$ wenn ungerade
$\psi$ ist nach VL ein Ringhomomorphismus.

$\psi\circ \phi$ ist als Verknüpfung von Homomorphismen ein Homomorphismus. Bezeichne mit $f_0$ den Konstanten Koeffizienten eines Polynoms $f \in \Z[x]$
$\psi\circ \phi(f) = 0 \iff \phi(f)$ ist gerade $\iff$ $f_0$ von $f$ ist gerade $\iff f\in (2, x)$

## b)
Zu Zeigen: $p_1p_2 = q_1 q_2 \implies q_1, q_2$ Primelemente

Gilt $p_1p_2=q_1q_2$, dann teilt $p_1|q_1q_2 \implies p_1|q_1$ oder $p_1|q_2$ $\implies$ o.E $p_1|q_1$ $\implies \exists a\in R: q_1 = p_1 a$
$q_1$ ist irreduzibel und $p_1$ kann als Primelement (also inbesondere Irreduzibles Element) keine Einheit sein. Daher ist $a$ invertierbar. 

$q_1$ ist ein Primelement, wenn $q_1 | xy \implies q_1 |x$ oder $q_1|y$ 
$q_1|xy \implies p_1a|xy \implies p_1|xy\cdot 1/a \implies p_1|xy \cdot 1/a \cdot a \implies o.E. p_1|x \implies p_1|x1/a \implies p_1a|x \implies q_1|x$

Außerdem teilt $p_2|q_1q_2 \implies p_2|q_1$ oder $p_2|q_2$ 
- Angenommen $p_2|q_1$, dann  $\exists b \in R$, sodass $q_1 = p_2b$
Wir setzen in die obere Formel ein: $p_1p_2 = p_2bq_2$
In einem Integritätsring gilt die Kürzungsregel: $p_1 = bq_2$
- Angenommen $p_2|q_2$, dann $\exists b \in R$ sodass $q_2 = p_2b$

In beiden Fällen ist $b$ ist invertierbar und der Beweis, dass $p_2$ ein Primelement ist, geht wie oben.

