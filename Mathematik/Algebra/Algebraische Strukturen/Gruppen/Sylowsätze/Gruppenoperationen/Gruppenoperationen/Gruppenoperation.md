# Beschreibung
Eine [[Gruppe]] operiert auf einer Menge $M$, wenn jeder [[Transformation|Transformationen]] der Gruppe eine andere Transformation auf $M$ zugeordnet werden kann, wobei neutrale  auf neutrale Transformationen und inverse auf inverse Transformationen abgebildet werden.
 

# Definition
## Carter 
## Nach Carter
Ein Gruppe $G$ operiert auf eine Menge $M$, wenn es einen [[Gruppenhomomorphismus]] von $G$ auf die [[Permutationsgruppe]] von $M$ gibt.

## Gerkmann
Eine Gruppenoperation von $G$ auf $X$ ist eine Abbildung $\alpha: G \times X \to X$ mit den Eigenschaften
$$\alpha(e_G, x) = x \text{ und } \alpha(g, \alpha(h, x)) = \alpha(gh, x)$$
Für alle $g, h\in G$ und $x \in X$, wobei $e_G$ das Neutralelement der Gruppe bezeichnet.

Statt $\alpha$ schreibt man auch $e_G \cdot x = x$, bzw $g\cdot(h \cdot x) = gh\cdot x$

## Arnold
Sei $G$ eine [[Gruppe]] und $M$ eine [[Menge]]

$G$ operiert auf $M$, wenn jedem $g\in G$ eine [[Transformation]] $T_g: M \to M$ zugeordnet wird, sodass für $g_1, g_2 \in G$ gilt:
- $T_{g_1g_2} = T_{g_1}T_{g_2}$
- $T_{g_1^{-1}} = T_{g_1}^{-1}$

Da dadurch eine neue Gruppe ensteht, und die Gruppenoperation von einer Transformation auf eine andere abbildet ist eine Gruppenoperation ein [[Homomorphismus]]. 

# Eigenschaften
## Permutation
Ist $\alpha : G \times X \to X$ eine [[Gruppenoperation]] auf $X$.

Dann kann man beobachten, dass eine Gruppenoperation nichts anderes als eine [[Permutation]] auf $X$ ist.
Die Permutation definiert sich durch:
$$\tau_g(x)= a(g, x)$$
Insbesondere ist 
$$G \mapsto Per(X), g \to \tau_g$$
ein [[Gruppenhomomorphismus]].

Umgekehrt lässt sich aus einem Gruppenhomomorphismus eine Gruppenoperation generieren.



# Beispiel
## Dreieck
Betrachte ein Gleichseitiges Dreieck

Die [[Gruppe]] seiner sechs Isometrien (Identität (i), 2 Drehungen (d1, d2), 3 Spiegelungen (s1, s2, s3)) operiert auf der Menge seiner zwei Orientierungen (-1 (Vorderseite) und 1 (Rückseite))

Ordne die Transformationen folgendermaßen zu
- Identität $\implies T_{Identität}(1) = 1, T_i(-1) = -1$
- Drehung $\implies T_{Drehung}(1) = 1, T_d(-1) = -1$
- Spiegelung $\implies T_{Spiegelung}(1) = -1, T_d(-1) = 1$

Die Bedingungen oben sind damit erfüllt. 

## Linkstranslation
Sei $G$ eine [[Gruppe]]. Dann ist durch $$G\times G \to G, g \cdot h =gh$$ eine Gruppenoperation von $G$ auf sich definiert. Man bezeichnet diese als Operation durch Linkstranslation.

*Herr Gerkmann hat gesagt, dass [[Cayley-Diagramm]] genau diese Linkstranslation beschreiben. Eine Gruppe (Pfeile) wirkt auf sich selbst (Knoten).*

## Operation auf Untergruppen
Siehe [[Konjugation (Untergruppen)]]


#Arnold #Carter #Algebra 
