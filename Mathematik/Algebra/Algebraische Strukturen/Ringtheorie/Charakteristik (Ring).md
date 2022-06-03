## Beschreibung
Die Charakteristik eines Ringes beschreibt seine Größe.

## Definition
Sei $R$ ein [[Ring]]. Die Charakteristik eines Ringes $R$ ist definiert durch
$$char(R) = \begin{cases} n & \text{falls } n\in \mathbb{N} \text{ minimal mit } n\cdot 1_R = 0_R \text{ ist, } \\ 0 & \text{falls } n \cdot 1_R \neq 0_R \text{ für alle } n \in \mathbb{N} \text{ gilt}\end{cases}$$

# Übungen 
## Checkliste Gerkmann
### Aufgabe 1
Wenn $L|K$ eine [[Körpererweiterung]] ist, warum haben $K$ und $L$ dann die gleiche Charakteristik?

$L$ ist ein $K$-Vektorraum. Elemente aus $L$ lassen sich als Linearkombination von Basiselementen aus $K$ beschreiben:
Multipliziert man die Charakteristik von $K$, dann sind alle Komponenten $0$. $L$ enthält desweiteren $K$, die Charakteristik kann durch die Erweiterung also nicht kleiner werden.

### Aufgabe 2
1. Gibt es endliche Körper mti Charakteristik $0$?
2. Gibt es unendliche Körper mit endlicher Charakteristik?

1. Nein, ist die Charakteristik 0, dann kann man aus $1$ immer neue Elemente $na$ erzeugen. Angenommen, die Elemente $n1, m1$ wären gleich, dann wäre $m1-n1 = (m-n)1 = 0$, und der Körper hätte Charakteristik $(m-n)$
2. Ja, zum Beispiel $F_2^{alg}$


#Zahlentheorie 