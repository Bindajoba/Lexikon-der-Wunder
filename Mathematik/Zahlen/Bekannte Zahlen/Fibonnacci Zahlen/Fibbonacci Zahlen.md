

## Beschreibung
Die Fibbonacci Zahlen ist die Zahlenfolge, die man erhält, wenn man beginnend mit 0 und 1 rekursiv die zwei letzten Zahlen der Folge addiert.

Man erhält dann: 0, 1, 1, 2, 3, 5, 8, 13, 21, ...


## Verallgemeinerungen
### Negative Zahlen
Durch Ausprobieren erhalten wir die Folge -8, 5, -3, 2, -1, 1, 0, 1, 1, 2, 3, 5, 8.
Diese Fibbonaccie Zahlen sind also auch in die andere Richung fortsetzbar.

### Komplexe Zahlen
Indem man statt natürlichen Indizes, reelle in die untere Formel einsetzt, erhält man Zahlen, die [[Komplexe Zahlen|komplexwertig]] sind.


## Eigenschaften
### Wachstumsfaktor
Die Fibbonacci-Zahlen wachsen mit [[Exponentialfunktion|exponentieller Geschwindigkeit]]. Demnach sollten sie so etwas wie einen relativen Wachstumsfaktor haben.

Nimmt man den Quotient zweier Zahlen, so nähert sich dieser an $\Phi = \frac{1+\sqrt{5}}{2}$ an.

Der Wachstumsfaktor $\Phi = 1,618$ ist nah am Verhältnis zwischen Meilen und Kilometer ($1,609$). Mit Hilfe der Fibbonacci Zahlen, könnte man also zwischen den Maßen umrechnen: $21 Kilometer = 18 Meilen$

### Algebraischer Beschreibung
Die Fibbonacci-Zahlen lassen sich auch durch die Formel
$$fib(n) = \frac{\Phi^n - (-\frac{1}{\Phi})^n}{\sqrt{5}}$$ berechnen.

## ggT konsekutiver Fib- Zahlen
$ggT(fib(n), fib(n+1)) = 1$, denn
$ggT(fib(n), fib(n+1)) = ggT(fib(n), fib(n)+fib(n-1)) = ggT(fib(n), fib(n-1))$
Wählen wir nun den Induktionsanfang $ggT(fib(1), fib(2)) = ggZ(1, 1) = 1$, so sehen wir, das die Aussage stimmt.


## ggT der Fibbonacci Zahlen
Wählt man die Konvention $fib(0) = 0, fib(1) = 1$, dann gilt
$$ggT(fib(a), fib(b)) = fib(ggT(a, b))$$

# Übungen
## McEliece Aufgabe 2-4
### a)
Was ist $ggT(fib(n), fib(n+1))$?
Siehe oben

### b)
Was sind die $q_i, r_1, s_i, t_i$ beim Berechnen des [[Euklidischer Algorithmus]] für $ggT(fib(n), fib(n+1))$?

| $i$   | $s_i$                  | $t_i$                   | $r_i$        | $q_i$ |
| ----- | ---------------------- | ----------------------- | ------------ | ----- |
| -1    | 1                      | 0                       | fib(n+1)     | -     |
| 0     | 0                      | 1                       | fib(n)       | -     |
| 1     | 1                      | -1                      | fib(n-1)     | 1     |
| 2     | -1                     | 2                       | fib(n-2)     | 1     |
| 3     | 2                      | -3                      | fib(n-3)     | 1     |
| 4     | -fib(4)                | fib(5)                  | fib(n-4)     | 1     |
| ...   | ...                    | ...                     | ...          | ...   |
| i     | $(-1)^{i+1}fib(i)$     | $(-1)^i fib(i+1)$       | $fib(n-i)$   | 1     |
| ...   | ...                    | ...                     | ...          | ...   |
| $n-3$ | $(-1)^{n-3+1}fib(n-3)$ | $(-1)^{n-3} fib(n-3+1)$ | $fib(3) = 2$ | 1     |
| $n-2$ | $(-1)^{n-2+1}fib(n-2)$ | $(-1)^{n-2}fib(n-2+1)$  | $fib(2) = 1$ | 1     |
|   $n-1$ | $(-1)^{n}fib(n-1)$ | $(-1)^{n-1}fib(n)$                      | $0$   | 2     |

## c)
Stelle $ggT(fib(n), fib(n+1))$ als Linearkombination dar.
$$ggT(fib(n), fib(n+1)) = (-1)^{n}(fib(n-1)fib(n)-fib(n-2)fib(n+1)) $$

#Spannende-Aufgaben #McEliece 


