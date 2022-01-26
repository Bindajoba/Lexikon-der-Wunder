## Beschreibung
Die Lypunovfunktion ist so etwas wie eine schwächere Version einer [[Erhaltungsgröße]].
Bei einer Lypunovfunktion kann der Wert der Funktion entlang einer Trajektorie auch kleiner werden.
Man kann es sich wieder als Energie vorstellen: Die Energie in einem System ist abhängig vom [[Zustand|Startzustand]], nimmt aber im Laufe der Zeit ab.

## Definition
Sei
$$x'=v(x)\tag{1}$$
eine [[Autonome Lipschitzst. DGL]]

Eine stetig differenzierbare Funktion $V: D \to \mathbb{R}$ heißt **Lyapunov-Funktion** für $(1)$, wenn
$$(grad E)(x) \circ v(x) \leq 0$$
für alle $x\in D$ erfüllt ist.

## Eigenschaften
### Monotonie
Eine Lyapunov-Funktion $V$ ist entlang einer Trajektorie monoton fallend:
$$\begin{array}{rcl} V \circ \varphi &\to &\mathbb{R}\\ t & \mapsto & V(\varphi(t)) \end{array}$$ fällt monoton

#Mathe-IV 