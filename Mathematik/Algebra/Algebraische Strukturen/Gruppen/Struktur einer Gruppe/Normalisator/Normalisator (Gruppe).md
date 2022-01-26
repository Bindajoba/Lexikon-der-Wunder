# Beschreibung
Beim Untersuchen stellen wir fest, dass manche Untergruppen "normaler" sein können als andere.
Eine [[Untergruppe]] $U$ ist ein [[Normalteiler]], wenn $gU = Ug$ für alle $U$ gilt.

Ist eine Untergruppe kein Normalteiler, dann liegt dass daran, dass es ein $g$ gibt, dessen anwendung auf zwei Elemente von $U$ in zwei unterschiedliche [[Nebenklasse|Nebenklassen]] führen würde.

Das wirft aber die Frage auf: Für welche Elemente $g \in G$ sind Links- und Rechtsnebenklasse von $U$ gleich?

Der Normalisator einer [[Untergruppe]] $U$ von $G$ ist die größte Untergruppe, in der $U$ ein [[Normalteiler]] ist.[^2]

# Definition
Der Normalisator einer Untergruppe $U$ in der Gruppe $G$ ist definiert durch:
$$N_G(U) ) \{g \in G: gU = Ug\}$$[^1]

# Eigenschaften
## Vereinigung von Nebenklassen
- Für ein Element aus $U$ selbst gilt $uU = U = Uu$. Daher ist die Untergruppe $U$ ein Teil von $N_G(U)$
- Sei $gU$ eine Nebenklasse.
Ist $g \in N_G(U)$, dann sind auch alle anderen Elemente von $gU$ in $N_G(U)$

## Untergruppe von G
Der Nomalisierer ist eine Untergruppe von $G$

## Erzeugung eines Normalteiler
$U$ ist ein Normalteiler von $N_G(U)$.
Der Normalisator beantwortet die Frage, wie viel von $G$ entfern werden muss, damit $U$ ein [[Normalteiler]] ist.




# Beispiel
## In Gruppe $D_6$
![[Normalisiator Beispiel.png]]
Im $D_6$ gilt $r^3\langle f \rangle = \langle f \rangle r^3$

#Carter #Algebra 

[^1]: Gerkmann - Definition 10.4
[^2]: Gerkmann - Proposition 10.7