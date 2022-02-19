TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung


# Definition
Sei $p$ eine ungerade Primzahl und $a \in \Z$. Das Legendre-Symbol modulo $p$ ist definiert durch
$$(\frac{a}{p}) = \begin{cases} 1 & \text{falls }a\text{ quadratischer Rest modulo }p\text{ und } p \nmid a \\
0 &\text{falls } p \mid a \\
-1 &\text{falls }a\text{ quadratischer Nichtrest modulo }p\end{cases}$$
# Eigenschaften
## Rechenregeln
Sei $p$ eine ungerade Primzahl und seien $a, b \in \Z$. Dann gilt
$$(\frac{ab}{p}) = (\frac{a}{p})(\frac{b}{p}) \text{ und }(\frac{a}{p}) = (\frac{b}{p}) \text{ falls } a \equiv b \mod p$$
## Eulersches Kriterium
Sei $p$ eine ungerade Primzahl. Dann gilt $(\frac{a}{p}) \equiv a^{(p-1)/2} \mod p$ für alle $a \in \Z$[^1]

## Erster Ergänzungssatz
Für jede ungerade Primzahl $p$ gilt.
$$(\frac{-1}{p}) = (-1)^{(p-1)/2} = \begin{cases} 1 &\text{falls } p \equiv 1 \mod 4 \\
-1 &\text{falls } p\equiv 3 \mod 4\end{cases}$$

## Zweiter Ergänzungssatz
$$(\frac{2}{p}) = (-1)^{(p^2-1)/8} = \begin{cases} 1 &\text{falls } p \equiv 1, 7 \mod 4 \\
-1 &\text{falls } p\equiv 3, 5 \mod 4\end{cases}$$

## Quadratisches Reziprozitätsgesetz
Siehe [[Quadratisches Reziprozitätsgesetz]]

# Beispiel
Berechne die Legendre-Symbole modulo $7$:

| $a$             | -2  | -1  | 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   |
| --------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| $(\frac{a}{p})$ | -1  | -1  | 0   | 1   | 1   | -1  | 1   | -1  | -1  | 0   | 1   | 1    |

Die Zahlen erhält man, indem man alle Zahlen aus $\Z/7\Z$ quadriert:
- $1^2 = 1$
- $2^2 = 4$
- $3^2 = 2$
- $4^2 = 2$
- $5^2 = 4$
- $6 = 1$

Wie man sehen kann, wiederholen sich die Bilder des Legrenge-Symbols alle $p$ Elemente.



#Zahlentheorie 


[^1]: Gerkmann - Satz 14.4