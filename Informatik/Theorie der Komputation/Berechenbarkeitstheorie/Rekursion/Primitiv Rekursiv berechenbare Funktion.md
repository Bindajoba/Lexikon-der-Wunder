## Beschreibung
**Primitiv Rekursiv Berechenbare Funktionen** ist ein neuer Formalismus, um [[LOOP-Berechenbarkeit|LOOP-berechenbare Funktionen]] anders zu beschreiben

## Definition
Eine [[Abbildung|Funktion]] $f: \mathbb{N}^k \to \mathbb{N}$ ist **primitiv rekursiv**, wenn sie der induktiven Definition genügt:
- Jede **konstante Funktion** $f(x_1, ..., x_k) = c \in \mathbb{N}$ ist primitiv rekursiv.
- Die [[Projektionsfunktion|Projektionsfunktionen]] $\pi_i^k(x_1, ..., x_k) = x_i$ sind primitiv rekursiv
- Die [[Nachfolgerfunktion]] $succ(x) = x + 1$ ist primiiv rekursiv.
- **Komposition/Einsetzung**: Wenn $g: \mathbb{N}^m \to \mathbb{N}$ und für $i = 0, ..., m: h_i: \mathbb{N}^k \to \mathbb{N}$ primitiv rekursiv sind, dann ist auch $f$ mit 
$f(x_1, ..., x_k) = g(h_1(x_1, ..., x_k), ..., h_m(x_1, ..., x_k))$ primitiv rekursiv
- **Primitive Rekursion**: Wenn $g: \mathbb{N}^{k-1}$ und $h: \mathbb{N}^{k+1}\to \mathbb{N}$ primitiv rekursiv, dann ist auch $f$ mit 
$$f(x_1, ..., x_k) = \begin{cases}g(x_2, ..., x_k), & \text{wenn } x_1 = 0 \\ h(f(x_1-1, x_2, ..., x_k), x_1-1, x_2, ..., x_k) & \text{sonst}\end{cases}$$ primitiv rekursiv

## Konstruktionen
### Kompontenten eines Tupels entfernen/vertauschen/vervielfachen
z.B. Wenn $g: \mathbb{N}^4 \to \mathbb{N}$, dann ist auch $f: \mathbb{N}^3 \to \mathbb{N}$ mit 
$$f(n_1, n_2, n_3) = g(n_2, n_3, n_3, n_2)$$ denn
$$f(n_1, n_2, n_3) = g(\pi_2^3(n_1, n_2, n_3), \pi_3^3(n_1, n_2, n_3), \pi_3^3(n_1, n_2, n_3), \pi_2^3(n_1, n_2, n_3))$$

### Rekursion durch das i. Argument
Eine Rekursion 
$$f(x_1, ..., x_k) = \begin{cases}g(x_1, ..., x_{i-1}, x_{i+1}, ..., x_k), & \text{wenn } x_i = 0 \\ h(f(x_1, ..., x_{i-1}, x_{i+1}, ..., x_k), x_1, ..., x_{i-1}, x_{i+1}, ..., x_k) & \text{sonst}\end{cases}$$ kann durch vertauschen der Komponenten umgeformt werden:
$$f(x_1, ..., x_k)=f'(x_i, x_1, ..., x_{i-1}, x_{i+1}..., x_k)$$ Dann ist $f'$ eine Funktion, dessen erster Parameter mit jeder Rekursion kleiner wird.

### Additionsfunktion
$add(x_1, x_2) = x_1 + x_2$ ist primitiv rekursiv, da man die Addition als rekursive Anwendung der Nachfolgerfunktion definieren kann.

### Multiplikationsfunktion
$mult(x_1, x_2) = x_1 \cdot x_2$ ist primitiv rekursiv, da man die Multiplikation als rekursive Anwendung der Addition definieren kann.

### Differenz
Die Differenz $x_1 - x_2$ ist allgemein nicht primitiv rekursiv, da der Fall $x_1 < x_2$ nicht in $\mathbb{N}$ liegt. 

### Angepasste Differenz
Die angepasste Differenz gibt $0$ zurück, wenn das Ergebnis negativ wäre und gibt sonst die normale Differenz zurück.  
Diese kann als rekursive Anwendung einer Vorgängerfunktion definiert werden.

## Eigenschaften
Die **Primitiv Rekursiven Berechenbaren Funktionen** sind genau die [[LOOP-Berechenbarkeit|LOOP-berechenbaren]] Funktionen

#FSK 
