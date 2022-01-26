## Beschreibung
Bei einem **nichtdeterministischen endlichen Automat**, kann ein [[Automat]], durch ein Zeichen in zwei verschiedene Zustände gleichzeitig wechseln. Der Automat muss sich dann für einen Zustand "entscheiden".

*Ich persönlich finde es viel intuitiver und logischer, dass der Automat, in mehreren (oder keinen) Zuständen gleichzeitig sein kann. Dann wäre der Automat aber wieder deterministisch, da er sich für beliebige Eingaben vorhersehbar verhält.
Da stinkt irgendwas...*

## Definition
Ein **nichtdeterministischer endlicher Automat** (**nondeterministic finite automaton**, **NFA**) ist ein 5-Tupel $(Z, \Sigma, \delta, S, E)$ wobei
- $Z$ ist eine endliche Menge von **Zuständen**
- $\Sigma$ ist das (endliche) Eingabe-[[Alphabet]]
- $S \subseteq Z$ ist die Menge der **Startzustände**
- $E \subseteq Z$ ist die Menge der **Endzustände**
- $\delta: Z \times \Sigma \to \mathcal{P}(Z)$ ist die **Zustandsüberführungsfunktion**
Die Funktion kann diesmal eine Menge, also mehrere Zustände gleichzeitig zurückgeben.[^1]

### Rekursive Zustandsübergangsfunktion
Sei $M = (Z, \Sigma, \delta, S, E)$
Wir definieren $\hat\delta$ induktiv durch:
$$\begin{array}{ll}\hat\delta(X, \varepsilon) &:= X \text{ für alle }X \subseteq Z\\ \hat\delta(X, aw) &:= \underset{z \in X}{\bigcup}\hat\delta(\delta(z, a), w) \text{ für alle }X \subseteq Z \end{array}$$ Die von $M$ akzeptierte Sprache ist $L(M) := \{w \in \Sigma^*:\hat\delta(S, w) \cap E \neq \emptyset\}$[^2]


## Eigenschaften
### Umwandlung in NFA
Jeder [[Deterministischer Endlicher Automat|deterministische endliche Automat]] kann in einen NFA umgewandelt werden. 
Dazu betrachtet man den DFA, als wäre er in mehreren Zuständen gleichzeitig. Beim Einlesen eines Zeichens bewegt sich der NFA auf vorhersehbare Weise in den nächsten Zustand.
Ausgehend von dieser Beobachtung kann man einen DFA konstruieren, bei dem jeder Zustand eine Zustandsmenge des vorherigen NFAs beschreibt.

Der DFA beginnt in der Zustandsmenge der Anfangszustände.
Befindet sich der DFA nach seinem Lauf in einer Zustandsmenge, die einen Endzustand enthält, dann wird das Wort erkannt.[^3]

## Varianten
### NFA mit $\varepsilon$-Übergängen
Siehe [[Nichtdeterministischer Endlicher Automat mit Epsilon-Übergängen]]


#FSK 

[^1]: Sabel - Definition 4.3.1
[^2]: Sabel - Definition 4.3.2
[^3]: Sabel - Theorem 4.5.1