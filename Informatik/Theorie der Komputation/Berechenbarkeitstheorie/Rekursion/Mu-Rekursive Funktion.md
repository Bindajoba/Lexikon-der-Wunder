## Beschreibung
**$\mu$-Rekursive Funktionen** ist ein neuer Formalismus, um [[WHILE-Berechenbarkeit|WHILE-berechenbare Funktionen]] anders zu beschreiben

Sie sind eine schwächere Version der [[Primitiv Rekursiv berechenbare Funktion]].

## Definition
Eine [[Abbildung|Funktion]] $f: \mathbb{N}^k \to \mathbb{N}$ ist **$\mu$ rekursiv**, wenn sie der induktiven Definition genügt:
- Jede **konstante Funktion** $f(x_1, ..., x_k) = c \in \mathbb{N}$ ist primitiv rekursiv.
- Die [[Projektionsfunktion|Projektionsfunktionen]] $\pi_i^k(x_1, ..., x_k) = x_i$ sind $\mu$-rekursiv
- Die [[Nachfolgerfunktion]] $succ(x) = x + 1$ ist $\mu$-rekursiv.
- **Komposition/Einsetzung**: Wenn $g: \mathbb{N}^m \to \mathbb{N}$ und für $i = 0, ..., m: h_i: \mathbb{N}^k \to \mathbb{N}$ $\mu$-rekursiv sind, dann ist auch $f$ mit 
$f(x_1, ..., x_k) = g(h_1(x_1, ..., x_k), ..., h_m(x_1, ..., x_k))$ $\mu$-rekursiv
- **Primitive Rekursion**: Wenn $g: \mathbb{N}^{k-1}$ und $h: \mathbb{N}^{k+1}\to \mathbb{N}$ $\mu$-rekursiv, dann ist auch $f$ mit 
$$f(x_1, ..., x_k) = \begin{cases}g(x_2, ..., x_k), & \text{wenn } x_1 = 0 \\ h(f(x_1-1, x_2, ..., x_k), x_1-1, x_2, ..., x_k) & \text{sonst}\end{cases}$$ $\mu$-rekursiv
- [[Mu-Operator]]: Wenn $h: \mathbb{N}^{k+1} \to \mathbb{N}$ $\mu$-rekursiv, dann ist auch $f=\mu h$ $\mu$-rekursiv.

## Eigenschaften
Die **Mu Rekursiven Funktionen** sind genau die [[WHILE-Berechenbarkeit|WHILE-berechenbaren]] Funktionen.

#FSK 