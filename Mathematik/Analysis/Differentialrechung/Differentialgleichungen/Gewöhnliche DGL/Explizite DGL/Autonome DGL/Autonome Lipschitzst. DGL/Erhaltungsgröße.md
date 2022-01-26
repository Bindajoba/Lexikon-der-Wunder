## Beschreibung
Eine Erhaltungsgröße ist eine Funktion, die entlang jeder Trajektorie einer [[Autonome Lipschitzst. DGL]] den gleichen Wert annimmt.

Man kann es sich als die Energieerhaltung vorstellen: Die Energie in einem System ist nur abhängig vom [[Zustand|Startzustand]].

Erhaltungsgrößen werden auch **erstes Integral** genannt.

## Definition
Sei $$x'=v(x)\tag{1}$$ eine [[Autonome Lipschitzst. DGL]].

$E\in C^1(D, \mathbb{K})$ ist eine Erhaltungsgröße wenn
$$(grad E)(x) \circ v(x) = 0$$
*D.h. Wenn die Richtung der größten Steigung von $E$ senkrecht zur [[Phasengeschwindigkeit]] von $(1)$ verläuft.
Bzw. Wenn die Richtung, in der sich $E$ nicht ändert gleich der Richtung der [[Phasengeschwindigkeit]] von $(1)$ ist*
*Es sei denn $E$ ist an der Stelle 0*

## Eigenschaften
Eine Erhaltungsgröße zu einer [[Autonome Lipschitzst. DGL]] ist längst jeder [[Trajektorie]] konstant:
$$E(\varphi(t, \xi))=E(\xi)$$ für alle $t\in J_\xi$ 
wobei $J_\xi$ das [[Autonome Differentialgleichungen/Existenzintervall]] von $\varphi(\cdot, \xi)$ zu $(1)$

#Mathe-IV 