# Beschreibung
Eine Abbildung zwischen zwei [[Körper]], die deren Struktur erhält.

# Definition
Ein Körperhomomorphismus $\phi : K \to L$ ist ein [[Ringhomomorphismus]] zwischen Körpern.
Er hat die zusätzliche Forderung $\phi(1_K) = 1_l$

# Eigenschaften
## Injektivität
Ein Körper ist immer [[Injektive Abbildung|injektiv]].[^1]

**Beweis:**
Ein Körperhomomorphismus ist ein Ringhomomorphismus. Damit ist er injektiv, wenn sein Kern trivial ist.

Für ein $n \in K$ gilt:
$$\phi(n) = \phi(n \cdot 1_K) = n \cdot \phi(1_K) = n \overset{!}{=} 0 \iff n = 0$$


## Gemeinsamer Teilkörper
Sei $\phi: L \to M$ ein Körperhomomorphismus, wobei wir voaraussetzen, dass $L$ und $M$ einen gemeinsamen Teilkörper besitzen. Dann ist auch die Teilmenge $K$ gegeben durch $K = \{a \in L  \phi(a) = a \}$ ein gemeinsamer Teilkörper von $L$ und $M$ und es gilt $\phi \in Hom_K(L, K)$


## Nullstelle auf Nullstelle
Sei $\phi: K \to \tilde K$ ein [[Körperisomorphismus]]. Seien außerdem $L|K$ und $\tilde L | \tilde K$ Körpererweiterungen, $\alpha \in L$ und $f \in K[x]$ ein Polynom mit $f(\alpha) = 0$. 
Ist dann $\psi: K(\alpha) \to \tilde L$ ein Körperhomomorphismus mit $\psi|_K = \phi$, dann ist $\tilde \alpha = \psi(\alpha)$ eine Nullstelle von $\tilde f = \phi(f)$

*Der Satz sagt, dass das Bild einer Nullstelle unter einem Homomorphismus auch eine Nullstelle ist, selbst wenn man den Körper erst erweitern müsste, um die Nullstelle zu erhalten.*


#Zahlentheorie #Algebra 

[^1]: Gerkmann - Proposition 2.7 