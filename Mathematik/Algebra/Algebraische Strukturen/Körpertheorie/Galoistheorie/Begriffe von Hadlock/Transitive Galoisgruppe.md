TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Die Transitive Galoisgruppe ist ein Begriff, den Hadlock in seinem Buch eingeführt hat. Ich benötige die Seite um Platz für eine Aufgabe zu finden.

Dieser Begriff ist ein Spezialfall von der [[Transitive Gruppenoperation]]. Dabei operieren die Körperautomorphismen auf den Nullstellen eines Polynoms.

# Definition
Eine [[Galoisgruppe eines Polynoms]] $f \in K[x]$ ist transitiv, wenn es für beliebige zwei Nullstellen $a, b$ von $f$ einen [[Körperautomorphismus]] $\sigma\in Gal(f|K)$ mit $\sigma(a) = b$ gibt.


# Eigenschaften
## Galoisgruppen von irreduziblen Polynomen
Jede Galoisgruppe eines irreduziblen Polynoms ist transitiv.

**Beweis:**
Ich würde das ganze echt gerne mit dem Fortsetzungssatz machen. Ich denke aber ich kann nicht annehmen, dass der Zerfällungskörper von $f$ durch Adjunktion einer Nullstelle von $f$ entsteht.
Sei $r_i$ eine Nullstelle von $f$. Seien $\{r_{i_1}, r_{i_2}, ..., r_{i_m}\}$ die Bilder von $r_i$ unter allen Automorphismen $\phi \in Gal(f|\Q)$.
Betrachte nun das Polynom das durch das Produkt der Linearfaktoren oberer Bilder entsteht, d.h. $$\prod_{k=1}^m (x-r_{i_k})$$
Die Koeffizienten dieses Polynoms sind die [[Symmetrisches Polynom|Symmetrische Polynome]] $\sigma_j$.
Das Anwenden von $\phi$ auf $\sigma_j(r_{i_1}, r_{i_2}, ..., r_{i_m})$ gibt:
$$\phi(\sigma_j(r_{i_1}, r_{i_2}, ..., r_{i_m})) = \sigma_j(\phi(r_{i_1}), \phi(r_{i_2}), ..., \phi(r_{i_m}))$$
Was nur die Eingaben permutiert und dementsprechend den Wert der symmetrischen Funktion nicht verändert. Damit muss aber $\sigma_j(r_{i_1}, r_{i_2}, ..., r_{i_m})$ im Fixkörper von $Gal(f|\Q)$, also $\Q$ liegen.

Das obere Produkt ist damit ein Polynom in $\Q$. In dem Fall muss es aber den gleichen Grad wie $f$ haben, sonst wäre $f$ nicht irreduzibel.
Somit gibt es ein Bild von $r_i$ auf jede andere Nullstelle.




$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


#Hadlock 