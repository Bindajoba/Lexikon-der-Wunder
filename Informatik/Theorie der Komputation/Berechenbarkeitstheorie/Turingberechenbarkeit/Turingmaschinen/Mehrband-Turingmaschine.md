## Beschreibung
Eine [[Turingmaschine]], die mehrere Bänder statt nur einem hat.
Im Gegensatz zur [[Mehrspuren-Turingmaschine]] können sich die Schreib-Lese-Köpfe auf den Bändern unabhängig voneinander bewegen.

## Definition
Eine **k-Bad-Turingmaschine** ist ein 7-Tupel $(Z, \Sigma, \Gamma, \delta, z_0, \square, E)$ mit
 - $Z$ ist eine endliche Menge von **Zuständen**
 - $\Sigma$ ist das (endliche) **Eingabealphabet**
 - $\Gamma \supset \Sigma$ ist das (endliche) **Bandalphabet**
 - $\delta$ ist die (deterministische/nichtdeterministische) **Zustandüberführungsfunktion**
	 - Für eine DTM: $\delta: (Z \times \Gamma^k) \to Z \times \Gamma^k \times \{L, R, N\}^k$
	 - Für eine NTM: $\delta: (Z \times \Gamma^k) \to \mathcal{P}(Z \times \Gamma^k \times \{L, R, N\}^k)$
 - $z_0 \in Z$ ist der Startzustand
 - $\square \in \Gamma \backslash \Sigma$ ist das Blank-Symbol
 - $E \subseteq Z$ ist die Menge der Endzustände 

Die **k-Mehrband-Turingmaschine** ließt also wieder ein ganzes k-Tupel auf einmal und überschreibt alle auf einmal. Die Bänder können sich aber unabhängig voneinander nach Links, Rechts bewegen.

## Eigenschaften
### Äquivalenz zu Einspuren-Turingmaschinen
Jede Mehrspuren-Turingmaschine kann auf einer 1-Band-Turingmaschine simuliert werden.

#FSK 