## Beschreibung
Ein **nichtdeterministischer endlicher Automat mit $\varepsilon$-Übergängen** ist ein [[Nichtdeterministischer Endlicher Automat]], der zusätzlich $\varepilon$-Übergänge erlaubt.

## Definition
Ein **nichtdeterministischer endlicher Automat mit $\varepsilon$-Übergängen** ist ein 5-Tupel $(Z, \Sigma, \delta, S, E)$ wobei
- $Z$ ist eine endliche Menge von **Zuständen**
- $\Sigma$ ist das (endliche) Eingabe-[[Alphabet]]
- $S \subseteq Z$ ist die Menge der **Startzustände**
- $E \subseteq Z$ ist die Menge der **Endzustände**
- $\delta: Z \times \Sigma \to \mathcal{P}(Z)$ ist die **Zustandsüberführungsfunktion**[^1]

### Epsilon-Hülle eines Zustands
Die Epsilon Hülle eines Zustands ist die Menge an Zuständen, die man durch $\varepsilon$-Übergänge von diesem Zustand erreichen kann.

Die Epsilon-Hülle des Zustands $z$ ist folgendermaßen induktiv definiert:
1. $z \in clos_\varepsilon(z)$
2. Wenn $z'\in clos_\varepsilon(z)$ und $z''\in \delta(z', \varepsilon) \implies z'' \in clos_\varepsilon(z)$[^2]
### Epsilon Hülle einer Zustandmenge
$$clos_\varepsilon := \begin{cases} X, & \text{wenn } \underset{z\in X}{\bigcup}\delta(z, \varepsilon) \\ clos_\varepsilon(X \cup \underset{z\in X}{\bigcup}\delta(z, \varepsilon)), &\text{sonst} \end{cases}$$[^2]

### Akzeptierte Sprache

Wir definieren $\tilde\delta: (\mathcal{P} \times \Sigma^*) \to \mathcal{P}(Z)$ induktiv durch:
$$\tilde\delta(X, \varepsilon):=X \text{ und } \tilde\delta(X, aw):= \underset{z \in X}{\bigcup} \tilde\delta(clos_\varepsilon(S), w) \cap E \neq \emptyset$$[^3]

## Variation Eindeutige Start und Endzustände
Jeden **nichtdeterministischer endlicher Automat mit $\varepsilon$-Übergängen** kann man so umwandeln, dass er eindeutige Start und Endzustände hat.
Erzeuge dazu einen neuen Startzustand am Anfang und erzeuge $\varepsilon$-Übergänge von dem neuen zu den ehemaligen Startzuständen. 
Erzeuge dazu einen neuen Endzustand am Ende und erzeuge $\varepsilon$-Übergänge von dem neuen zu den ehemaligen Endzuständen. 

#FSK 

[^1]: Sabel - Defintion 4.6.1
[^2]: Sabel - Definition 4.6.3
[^3]: Sabel - Definition 4.6.5