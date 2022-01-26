TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Das Problem befasst sich mit der Frage, ob es möglich ist, mit einem Lineal und Zirkel einen beliebigen Winkel zu dritteln.

Die Frage gehört zu den [[Klassische Probleme der Antike|klassischen Problemen der Antike]]. Es ist bewiesenermaßen nicht möglich, einen Winkel nur mit [[Euklidische Werkzeuge]] zu dritteln.

# Beweis
Die Aussage lautet, man nehme einen beliebigen Winkel, dann kann man diesen dritteln.

Findet man also einen Winkel, den man nicht dritteln kann, ist die Aussage widerlegt.
Wir wählen den Winkel 60°, da er konstruierbar ist (d.h. aus einer Einheitslänge generierbar und damit keine Zusatzinformationen liefert.). 
Könnte man 60° durch Konstruktion dritteln, dann könnte man 20° konstruieren. Könnte man 20° konstruieren, dann auch cos(20°).

Wir zeigen aber nun, dass cos(20°) nicht mit Zirkel und Lineal konstruierbar ist.
Wir versuchen $cos(20°)$ als Nullstelle eines Polynoms darzustellen.

Das geht indem wir die [[Sinus und Kosinus#Additionstheoreme|Additionstheoreme]] anwendet:
$$\frac{1}{2} = \cos(60°) = 4\cos^3(20°)-3\cos(20°)$$
Wir substituieren $x = 2\cos(^20°)$, modifizieren und erhalten:
$$0 = x^3 - 3x - 1$$
Man kann aber zeigen, dass die Nullstelle dieser Gleichung nicht rational ist und auch nicht durch [[Quadratische Erweiterung]] erhältlich ist. Da man mit [[Euklidische Konstruktion]] nur mehrfache Quadratische Erweiterungen von den Rationalen Zahlen generieren kann, ist $x$ also auch $cos(20°)$ nicht konstruierbar.
Damit ist auch $20°$ nicht konstruierbar.


#Hadlock 