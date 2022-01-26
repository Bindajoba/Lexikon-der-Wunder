## Definition
Eine Funktion $f: \mathbb{N}^k \to \mathbb{N}$ heißt WHILE-berechenbar, wenn es ein [[WHILE-Sprache|WHILE-Programm]] $P$ gibt, sodass für alle $n_1, ..., n_k \in \mathbb{N}$ und Variablenbelegungen $\rho = \{x_1 \mapsto n_1, ..., x_k \mapsto n_k\}$ gilt:
- Falls $f(n_1, ..., n_k)$ definiert: $(\rho, P) \underset{WHILE}\longrightarrow^* (\rho', \varepsilon) \text{ und } p'(x_0) = f(n_1, ..., n_k)$
- Falls $f(n_1, ..., n_k)$ nicht definiert, dann stoppt das Programm nicht

## Eigenschaften
### LOOP-Sprache

Jede durch ein [[LOOP-Programme]] berechenbare Funktion kann auch durch ein WHILE-Programm berechnet werden.

### LOOP in der Syntax
Jedes LOOP kann in eine WHILE-Konstruktion umgewandelt werden, Daher ist das LOOP überflüssig.

### Berechenbarkeit
Die WHILE-Berechenbaren Sprachen sind genau die [[Turingberechenbarkeit|Turing-berechenbaren Sprachen]][^1]

#FSK 
[^1]: Theorem 10.2.4