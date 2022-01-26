## Definition
Eine Funktion $f: \mathbb{N}^k \to \mathbb{N}$ heißt LOOP-berechenbar, wenn es ein [[LOOP-Sprache|LOOP-Programm]] $P$ gibt, sodass für alle $n_1, ..., n_k \in \mathbb{N}$ und Variablenbelegungen $\rho = \{x_1 \mapsto n_1, ..., x_k \mapsto n_k\}$ gilt:

$$(\rho, P) \underset{LOOP}\longrightarrow^* (\rho', \varepsilon) \text{ und } p'(x_0) = f(n_1, ..., n_k)$$


## Eigenschaften
### Terminierung
Alle LOOP-Programme terminieren. Daher sind alle LOOP-berechenbaren Funktionen total.

Das erkennt man schon daran, dass die LOOP-Syntax keine Zyklen und Rekursionen erlaubt.

### Erzeugbare Funktionen
Aus dem oberen Grudn ist die Menge der LOOP-Berechenbaren Funktionen eine Teilmenge der [[Turingberechenbarkeit|Turin-berechenbaren Funktionen]]


#FSK 