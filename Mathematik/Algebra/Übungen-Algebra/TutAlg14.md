TARGET DECK: Universität::Mathematik::Algebra


![[blatt14.pdf]]
# Aufgabe 0
## a)
Galois Gruppe wird vom Frobenius-Automorphismus des Körpers $L$ erzeugt.
Die Galois-Gr. zyklisch von Ordn. $[L:K]$


## b)
Elemente d. Glaoisgruppe $Gal(\Q(\zeta):\Q$ sind gegeben durch die Automorphismen $\sigma_a$ mit $\sigma_a(\zeta_{12}) = \zeta_{12}^a$, wobei $a$ die Zahlen $\{0, .., 11\}$ mit $ggT(a, 12) = 1$ duchläuft.
Es bleiben $\{1, 5, 7, 11\}$ übrig.

## c)
$Gal(\Q(\zeta_{12}|\Q)) \cong (\Z/12\Z)^\times \cong (\Z/3\Z)^\times (\Z/4\Z)^\times \cong (\Z/2\Z) \times (\Z/2\Z)$ nicht zyklisch

## d)
Galois-Erw. die Isomorph zu $\Z/2\Z \times \Z/2\Z$ besitzt genau drei echte Zwischenkörper
Echte Zwischenkörper sind $\Q(i) = \Q(\zeta_3)$ und $\Q(\sqrt{-3}) = \Q(\zeta_4)$

$\Q(\sqrt 3)$ ist ein weiterer Zwischenkörper aber kein Kreisteilungskörper, da alle Zahlen Reell sind. Beim Hinzufügen einer Einheitswurzel kommt aber immer eine Komplexe Zahl hinzu, (Außer man adjungiert nur um $1$) aber $\Q(\sqrt 3) \neq \Q(1)$ 

# Aufgabe 1
## a)
Hat $\alpha$ die Ordnung $n$, dann ist $\alpha$ Nullstelle von $x^n + 1$.
$f$ ist Minimalpolnom von $\alpha$. Damit gilt $f \mid x^n +1$
$\alpha$ ist desweiteren eine Primitive $n$-te Einheitswurzel.
$x^n + 1$.

$f$ hat Grad $6$. Damit gilt $|\F_2(\alpha)| = 2^6 = 64$.
Dessen Multiplikative Gruppe hat $63$ Elemente und ist eine zyklische Gruppe. Die aus $\alpha$ erzeugte zyklische Gruppe ist eine Untergruppe und hat damit Ordnung $3, 7, 9, 21, 63$.
- $3$ kann es nicht sein, denn sonst wäre $x^3-1$ ein Polynom, das $\alpha$ als Nullstelle hat aber dann gilt nicht $f \mid x^3-1$
- $7$ kann es nicht sein, denn $x^7+1/f$ ist nicht restlos teilbar.
- $9$


# Aufgabe 2
![[blatt14.pdf]]

## a)
Es gibt einen Autmomorphismus, der $\zeta_5$ auf eine andere primitive Einheitswurzel abbildet. Des weiteren muss jeder Automorphismus $\zeta_5$ auf eine andere Einheitswurzel abbilden.

Die Galois Gruppe $Gal(\Q(\zeta)|\Q)$ besteht aus genau diesen Automorphismen.
Da jede 5-te Einheitswurzel auf eine andere Einheitswurzel abgebildet wird. Und diese EInheitswurzel bei Anwendung eines anderen Automorphismus wieder auf eine andere primitive 5-te Einheitswurzel abgebildet werden muss kann die Bahn nicht größer sein, als die Menge aller primitiven 5-ten Einheitswurzeln $\zeta_5, \zeta_5^2, ..., \zeta_5^4$.

Da es einen Automorphismus gibt, der $\zeta_5, \zeta_5^2, ..., \zeta_5^4$ als Bild von $\zeta_5$ haben kann ist $\zeta_5, \zeta_5^2, ..., \zeta_5^4$ genau die Bahn.

*Eine Verknüpfung von Automorphismen ist wieder ein Autmorphismus. Man muss also bloß die Biler von $\zeta_5$ unter allen Automorphismen betrachten.*

### Matthias Lösung
Die Bahn ist definiert durch:
$$G(\zeta_5) = \{\sigma \in Gal(\sigma(\zeta_5):\Q(\zeta_5):\Q)\}$$
Die Bilder von $\zeta_5$ unter den oberen Automorphismen sind alle andere primitive 5-te Einheitswurzeln. Die Bahn ist damit $\zeta_5, \zeta_5^2, ..., \zeta_5^4$.

## b)
Sei $G = Gal(\Q(\zeta))$. $G \cong (\Z/5/\Z)^\times \cong \Z/4\Z$. Damit gibt es nur einen einzen echten Zwischenkörper.
$\Q(\zeta_5^2 + \zeta_5^3) \subset \R$ 


## c)
$\sqrt{5} = \zeta_5^2 + \zeta_5^3$
Damit gilt $\Q(\sqrt 5)$

$\sigma_2$ erzeugt $G$.
$\langle \sigma_2^2 \rangle = \{\sigma_1, \sigma_4\} \implies \sigma_1(\zeta_5) = \zeta_4$ und $\sigma_4(\zeta_5) = \zeta_5^4$
$\alpha = \zeta_5 + \zeta_5^4$
$\sigma_2^2(\alpha) = \alpha \implies \alpha$ ist im Fixkörper von $\langle \sigma_2^2\rangle$
Es gilt $id_{\Q(\zeta_5)} \subset \langle \sigma_2^2 \rangle \subset \langle \sigma_2 \rangle = G$ 
Nach dem Hauptsatz ist der Fixkörper eine eindeutig bestimmte echte Zwischenerweiterung von $\Q(\zeta_5)|\Q$.

Spiele mit $\alpha^2$:
$\alpha^2 = 1+\a \implies \alpha$ ist die Nst. des Polynoms $x^2-x-1$. Wir wenden die Mitternachtsformel an und erhalten:
$$\alpha = \frac{1}{2} \pm \frac{1}{2}\sqrt{5}$$


$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


#Algebra 





