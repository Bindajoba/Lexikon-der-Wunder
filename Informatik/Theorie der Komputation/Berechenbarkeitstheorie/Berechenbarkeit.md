## Beschreibung
Die Berechenbarkeit beantwortet die Frage, wann etwas von einem Computer berechnet werden kann und wie man das beweist

## Geschichte
In den 1930er versuchten Mathematiker/Informatiker den Begriff der Berechenbarkeit zu formalisieren.
Besonders relevant waren:
- [[Alan Turing]]: [[Turingmaschine]]
- [[Alanzo Church]]: [[Lambda-Kalkül]]

## Definition
Eine Funktion $f: \mathbb{N}^k \to \mathbb{N}$ nennen wird **berechenbar**, wenn es einen Algorithmus einer modernen Programmiersprache gibt, der $f$berechnet:
- Bei Eingabe $(n_1, ..., n_k)$ stoppt der Algorithmus nach endlich vielen Berechnungsschritten und liefert den Wert von $f(n_1, ..., n_k)$ als Ausgabe.
- Wenn $f(n_1, ..., n_k)$ undefiniert ist ($f$ ist also eine [[Partielle Funktion]]), dann soll der Algorithmus nicht stoppen.

## Beispiele
### Beispiel 1
Der Algorithmus

    Eingabe: Zahl $n \in \mathbb{N}$
    Beginn
		solange true tue
			skip
berechnet $f_1:\mathbb{N} \to \mathbb{N}$ mit $f_1(x)=$ undefiniert für alle $x$

### Beispiel 2
Der Algorithmus

    Eingabe: Zahl $n_1, n_2 \in \mathbb{N}$
    Beginn
		hilf := n_1 + n_2
		return hilf
berechnet $f_1:\mathbb{N}^2 \to \mathbb{N}$ mit $f_1(x, y) = x + y$ undefiniert für alle $x$

### Beispiel 3

$$f_3 = \begin{cases} 1, &\text{falls }n\text{ ein Teilwort der Ziffern der Dezimaldarstellung von } \pi \text{ ist.} \\ 0, & \text{sonst} \end{cases}$$

Unklar, da man nicht weiß, ob das Prgramm terminiert oder nicht ([[Ziffern PI]])


### Beispiel 4

$$f_4 = \begin{cases} 1, &\text{falls die Dezimaldarstellung von }\pi\text{ das Wort } 3^m=33...3 \text{ mit } m\geq n \text{ als Teilwort besitzt.} \\ 0, & \text{sonst} \end{cases}$$

$f_4$ ist berechenbar, denn wenn $3^m$ in $\pi$ enthalten ist, dann gilt $f_4(n) = 1$.
Hat $\pi$ höchstens $m_0$ 3en hintereinander, dann ist $f_4(n) = 1$, wenn $n \leq m_0$ und sonst 0.  

Wir müssen also keinen Algorithmus angeben, sondern nur beweisen, dass er existiert.

### Beispiel 5
$$f_4 = \begin{cases} 1, &\text{falls }n\text{ ein Präfix der Ziffen der Dezimaldarstellung von } r \text{ ist.} \\ 0, & \text{sonst} \end{cases}$$

Ist $f^r$ für jedes $t\in \mathbb{R}$ berechenbar?
**Nein**: Wir bräuchten für jedes $r$ einen Algorithmus. Wir bräuchten also überabzählbar viele. Da man aber jeden Algorithmus einer Programmiersprache aufzählen kann, gibt es nur abzählbar viele Algorithmen, und manche $f^r$ können daher nicht berechenbar sein.

#FSK 