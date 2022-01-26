## Beschreibung
Ein Produktautomat ist das Ergebnis des Gedankenexperiments, zwei verschiedene Automaten parallel zu durchlaufen.
Damit kann man beispielsweise feststellen, ob ein Wort in beiden Automaten enthalten ist.

## Definition
Seien $M_1 = (Z_1, \Sigma, \delta_1, z_{01}, E_1)$ und $M_2 = (Z_2, \Sigma, \delta_2, z_{02}, E_2)$ [[Deterministischer Endlicher Automat|Deterministische Endliche Automaten]], die $L_1 = L(M_1)$ und $L_2 = L(M_2)$ akzeptieren.
Der Produktautomat von $M_1$ und $M_2$ ist $M = (Z_1 \times Z_2, \Sigma, \delta), (z_{01}, z_{02}, E_1 \times E_2)$ mit $\delta((z, z'), a) = (\delta(z, a), \delta(z', a))$ für alle $a \in \Sigma$ und $(z, z') \in Z_1 \times Z_2$

#FSK 