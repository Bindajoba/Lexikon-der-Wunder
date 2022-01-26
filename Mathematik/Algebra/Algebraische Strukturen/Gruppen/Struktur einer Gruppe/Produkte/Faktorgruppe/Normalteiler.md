
# Definition
Sei $G$ eine [[Gruppe]]. Eine [[Untergruppe]] $U$ von $G$ wird Normalteiler von $G$ genannt (Schreibweise $U \trianglelefteq G$) wenn $gU = Ug$ für alle $g \in G$ gilt.

*Also, wenn die Links- und [[Nebenklasse|Rechtsnebenklasse]] gleich ist.*

## Einfache Gruppen
Ist $G$ eine Gruppe, dann sind $\{e\}$, $G$ Normalteiler
Man nennt sie die sog. trivialen Normalteiler.
Gibt es keine weiteren Normalteiler in $G$, so nennt man $G$ eine einfache  Gruppe. (Manchmal wird $G = \{e\}$ als einfache Gruppe angeschlossen.)

*Primzahlen sind beispielsweise solche Gruppen*

# Charakterisierungen
Sei $G$ seien Gruppe und $U$ eine Untergruppe. Dann sind ie folgenden Bedingungen äquivalent
- $U$ ist Normalteiler von $G$
- Es gilt $gUg^{-1} \subseteq U$ für alle $g \in G$, wobei $gUg^{-1} = \{gug^{-1} : u \in U\}$ ist
- Es gilt $gUg^{-1} = U$ für alle $g \in G$

# Eigenschaften
1. Ist $G$ eine Gruppe und $U$ eine Untergruppe mit $(G:U) = 2$, dann gilt $U \trianglelefteq G$
2. Ist $G$ eine Gruppe und $(N_i)_{i\in I}$ eine Familie von Normalteilern, dann ist auch $N = \bigcap_{i \in I} N_i$ ein Normalteiler von $G$
3. Sei nun $\phi: G \to H$ ein [[Gruppenhomomorphismus]]. Ist $N$ ein Normalteiler von $H$, dann ist $\phi^{-1}(N)$ ein Normalteiler von $G$
4. Ist $\phi$ surjektiv und $N$ Normalteiler von $G$, dann ist $\phi(N)$ Normalteiler von $H$[^1]

## Zum direkten Produkt
Sei $A \times B$ eine Gruppe.
Dann sind $A$ und $B$ ein Normalteiler.

## Zerlegung von Konjugationsklassen
Ist $g$ im **Normalteiler** $N$, dann ist auch die ganze [[Konjugationsklasse]] von $g$ in $N$. In Folge ist $N$ eine Zerlegung von Konjugationsklassen.

Kennt man alle Konjugationsklassen einer Gruppe und berücksichtigt die Tatsache, dass die [[Ordnung]] einer [[Untergruppen]] immer ein [[Teilbarkeit|Teiler]] der [[Ordnung]] der ganzen Grupp ist erhält eine starke Einschränkung zum Finden von Normalteilern 

#Algebra 

[^1]: Gerkmann - Satz 5.3