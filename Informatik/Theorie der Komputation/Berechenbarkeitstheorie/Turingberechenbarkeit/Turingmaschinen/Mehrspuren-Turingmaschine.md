## Beschreibung
Eine [[Turingmaschine]], die mehrere Spuren statt nur einer hat.

## Definition
Eine **k-Spuren-Turingmaschine** ist ein 7-Tupel $(Z, \Sigma, \Gamma, \delta, z_0, \square, E)$ mit
 - $Z$ ist eine endliche Menge von **Zuständen**
 - $\Sigma$ ist das (endliche) **Eingabealphabet**
 - $\Gamma \supset \Sigma$ ist das (endliche) **Bandalphabet**
 - $\delta$ ist die (deterministische/nichtdeterministische) **Zustandüberführungsfunktion**
	 - Für eine DTM: $\delta: (Z \times \Gamma^k) \to Z \times \Gamma^k \times \{L, R, N\}$
	 - Für eine NTM: $\delta: (Z \times \Gamma^k) \to \mathcal{Z \times \Gamma^k \times \{L, R, N\}}$
 - $z_0 \in Z$ ist der Startzustand
 - $\square \in \Gamma \backslash \Sigma$ ist das Blank-Symbol
 - $E \subseteq Z$ ist die Menge der Endzustände 

Die **k-Spuren-Turingmaschine** ließt also ein ganzes k-Tupel auf einmal und überschreibt alle auf einmal

## Eigenschaften
### Äquivalenz zu Einspuren-Turingmaschinen
Jede Mehrspuren-Turingmaschine kann auf einer 1-Band-Turingmaschine simuliert werden.

Dazu wird das [[Kartesisches Produkt]] $\Sigma^k$ über dem Bandalphabet gebildet. Die Turingmaschine geht dann mit dieser Menge um, als wäre sie ein ganz normales eindimensionales Alphabet. 
So kann die Turingmaschine mit Tupeln umgehen, obwohl es nur ein Band hat.
