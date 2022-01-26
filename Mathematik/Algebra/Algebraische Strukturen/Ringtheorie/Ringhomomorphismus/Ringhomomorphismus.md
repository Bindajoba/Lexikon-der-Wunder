TARGET DECK: Universität::Mathematik::Algebra

## Beschreibung
Ein Ringhomomorphismus ist ein [[Homomorphismus]], der die Struktur eines [[Ring|Ringes]] beibehält.

## Definition
Seien $(R, +_R, \cdot_R)$ und $S, +_S, \cdot_S$ [[Ring|Ringe]]. Eine Abbildung $\phi: R \to S$ heißt Ringhomomorphismus von $(R, +_R, \cdot_R)$ nach $S, +_S, \cdot_S$, wenn die Gleichung $\phi(1_R)=1_S$ gilt und außerdem
$$\phi(a+_R b) = \phi(a) +_S \phi(b)$$ und
$$\phi(a \cdot_R b) = \phi(a) \cdot_S \phi(b)$$

*Die Erhaltung des Nullelements muss nicht zusätzlich gefordert werden.*

Q: Welche Eingenschaften muss man zeigen, damit man einen Ringhomomorphismus erhält.
A: - Ring auf Ring
- Erhaltung des Einselement
- Erhaltung der Addition
- Erhaltung der Multiplikation
<!--ID: 1642761436811-->


 

## Eigenschaften
### Fortsetzung auf Quotientenkörpers
Sei $R$ ein [[Integritätsbereich]] und sei $K$ ein [[Quotientenkörper]] von $R$

Ist $\phi: R \to S$ ein Ringhomomorphismus, der nur $0_R$ auf $0_S$ abbildet, dann gibt es eine eindeutige Fortsetzung $\hat\phi$ auf den Quotientenkörper $K$.

*Das bedeutet, $\hat\phi:K \to S$ ist ein Ringhomomorphismus mit $\hat\phi|_R = \phi$*

### Erhaltung von Idealen
1. Das Urbild eines [[Ideal]] unter einem **Ringhomomorphismus** ist ein Ideal
2. Ist der Ringhomomorphismus [[Surjektive Abbildung|surjektiv]], dann ist das Bild eines Ideal wieder ein Ideal

#Zahlentheorie 