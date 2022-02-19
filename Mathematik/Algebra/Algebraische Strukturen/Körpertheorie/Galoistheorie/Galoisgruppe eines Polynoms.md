TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$

# Beschreibung
Die Galoisgruppe eines Polynoms $f$ ist die Gruppe der [[Körperautomorphismus|Körperautomorphismen]] im [[Zerfällungskörper]] von $f$. Es handelt sich also einfach um eine [[Galoisgruppe]]

# Definition
Sei $K$ ein Körper und $f \in K[x]$ ein nicht-konstantes Polynom, dessen irreduzible Faktoren alle separabel sind, und sei $L$ ein Zerfällungskörper von $f$ über $K$. Dann bezeichnet man $Gal(L|K)$ aus als die **Galoisgruppe $Gal(f|K)$ des Polynoms $f$**.[^1]

## Konventionen
Wenn man sagt, die **Galoisgruppe von $f$** meint man für gewöhnlich die Erweiterung über dem kleinsten Körper, der alle Koeffizienten von $f$ enthält.

# Eigenschaften
Sei $f \in K[x]$ ein Polynom mit oberer Definition und $L$ ein Zerfällungskörper von $f$ über $K$. Seien $\alpha_1, ..., \alpha_n \in L$ die verschiedenen Nullstellen von $f$ in $L$. Dann gibt es eine [[Einbettung (Gruppe)]]
$$\phi:Gal(f|K) \to S_n \text{ mit } \sigma(\alpha_k) = \alpha_{\phi(\sigma)(k)} \text{ für } k \in \{1, ..., n\}$$
*Das bedeutet jeder Automorphismus ist eine Permutation von Nullstellen.*[^2]



# Beispiel
## Zyklische Galoisgruppe
Die [[Galoisgruppe]] von $f = (x^p-1)/(x-1)$ ist [[Zyklische Gruppe|zyklisch]], und hat [[Ordnung (Gruppe)|Ordnung]] $p-1$.

**Beweis:**
$(x^p-1)$ hat als Nullstellen die $p$-ten [[Einheitswurzel|Einheitswurzeln]]. Da $p$ prim ist, sind $p-1$ davon primitiv. Also alle außer $1$.
Sei $\zeta$ eine Einheitswurzel, die nicht $1$ ist. 

Ich möchte erst zeigen, dass $f$ irreduzibel ist. Aber das habe ich zum Glück schon in einer früheren Übung gezeigt. Damti gibt es einen eindeutigen $\Q$-Homomorphismus für das Bild von $\zeta$ auf jede andere der $p-1$ Wurzeln.

Diese Homomorphismen erfüllen offensichtlich die Eigenschaft, eine zyklische Gruppe zu sein. [^3]

## Symmetrische Galoisgruppe
Polynome, deren Galoisgruppe die Symmetrische Gruppe ist, d.h. alle Poermutationen seiner Nullstellen ist relativ schwer zu finden.
Polynome mit solcher Eigeschaft sind aber:
Sei $f$ ein [[Irreduzibles Polynom]] über $\Q$ von Primzahlgrad $p$, welches genau $p-2$ reelle Nullstellen hat, dann ist dessen Galoisgruppe $S_p$.

Die Idee ist folgende: Sei $\zeta$ eine der Nullstellen. EIndem man eine Nullstelle auf die nächste abbildet erhält man eine 


#Algebra 


[^1]: Gerkmann - Definiton 17.10
[^2]: Gerkmann - Satz 17.11
[^3]: Hadlock - Aufgabe 3.2.1