TARGET DECK: Universität::Mathematik::Algebra

# Definition
Eine [[Körpererweiterung]] $L|K$ wird **Galois-Erweiterung** genannt, wenn sie [[Normal|normal]] und [[Separable Erweiterung|separabel]] ist. Die Gruppe $Gal(L|K) = Aut_K(L)$ heißt dann die [[Galoisgruppe]] der Erweiterung $L|K$

# Charakterisierung
$L|K$ ist genau dann eine Galois Erweiterung, wenn
- $|Aut_K(L)| = [L:K]$
- $L^{Aut_K(L)} = K$
D.h. $K$ ist der Fixkörper von $Gal(L|K)$


Wobei $L^{Aut_K(L)}$ ein [[Fixkörper]] ist.

*Der unterste stellt die Rechenregel $L^{Gal(L|K)} = K$ auf.*

# Eigenschaften
In einer Galoiserweiterung $L|K$ ist jeder $K$-[[K-Homomorphismus|Homomorphismus]] ein $K$-[[Körperautomorphismus|Automorphismus]]

# Übungen
## Checkliste Gerkmann
### Aufgabe 1
Angenommen, $L|\Q$ ist eine endliche Galois-Erweiterung mit Zwischenkörper $\Q(\sqrt[3]2)$. Kann $Gal(L|\Q)$ dann eine abelsche Gruppe sein?

$L$ soll normal sein. Da $L$ $\sqrt[3]2$ enthält, muss es auch die anderen Nullstellen seines Minimalpolynoms besitzen, also $\sqrt[3]2 \zeta_3$ und $\sqrt[3]2 \zeta_3^2$
Die Körper $\Q(\sqrt[3]2)$ und $\Q(\sqrt[3]2, i)$ sind Zwischenkörper von $L|\Q$.

Es gibt einen Homomorphismus, der $\sqrt[3]2$ auf die anderen Nullstellen abbildet und einen, der $i$ auf $\pm$ abbildet.

Im Grunde bilden sind die drei Nullstellen wie in einer symmetrischen Gruppe vertauschbar, weshalb es keine kommutativen Automorphismen sind.

### Aufgabe 2
Angenommen, wir wissen bereits, dass eine Galois-Gruppe $Gal(L|K)$ isomorph zu $\Z/9\Z$ oder zu $(\Z/3\Z)^2$ ist, und wir haben zwei verschiedene echte Zwischenkörper in $L|K$ gefunden. Welcher Isomorphietyp ist dann der richtige? Und wieviele echte Zwischenkörper besitzt die Erweiterung dann tatsächlich? (richtige Antwort: 4)

$\Z/9\Z$ hat nur eine echte Untergruppe, der zugehörige Körper hat also nur einen echten Zwischenkörper. Also muss die Galoisgruppe des Körpers isomorph zu $(\Z/3\Z)^2$ sein. Diese hat $9$ Elemente. Echte Zwischenkörper haben Ordnung $3$, sind also zyklisch und werden aus einem Einzigen Element erzeugt. In $(\Z/3\Z)^2$ gibt es $8$ Elemente, die eine echte Untergruppe der Ordnung $3$ erzeugen. Jeweils zwei davon erzeugen die gleiche Untergruppe. Also gibt es $4$ nicht-triviale Untergruppen und damit $4$ echte Zwischenkörper.

### Aufgabe 3
Wir betrachten auf den Nullstellen des Polynoms $f = (x-1)(x-3)(x^2+1)$ die Nummerierung $\alpha_1=1, \alpha_2=3, \alpha_3=-i, \alpha_4=i$. Aus welchen beiden Elementen besteht $Gal(f|\Q)$, ausfgefasse als Untergruppe von $S_4$.
Ein Automorphis muss Nullstellen aller irreduziblen Faktoren von $f$ auf ihre [[Konjugierte Elemente|Konujigierten Elemente]] ab. Desweiteren sind sie durch die Bilder einer Nullstelle pro [[Irreduzibles Polynom]] eindeutig. Jede Automorphismus muss $1, 3$ auf $1, 3$ abbilden. Der Freiraum besteht darin $i$ auf $\pm i$ abzubilden. Damit gibt es zwei Automorphismen. Einer ist die Identität und der andere vertauscht einfach $i$ und $-i$.
Damit ist die Untergruppe von $S_4$ einfach $\langle (3\, 4)\rangle$.


#Algebra 


