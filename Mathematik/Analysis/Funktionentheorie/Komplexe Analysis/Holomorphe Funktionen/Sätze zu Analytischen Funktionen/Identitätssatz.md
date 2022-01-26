## Beschreibung
Dank des Identitätssatzes reicht schon die Gleichheit zweier [[Analytische Funktion|analytischer Funktionen]] auf einem start eingeschränkten Bereich, um die Gleichheit auf größeren Definitionsbereichen zu zeigen.

## Definition
### Komplexe Zahlen Zenk
Seien $f: U \to \mathbb{C}$ und $f: U \to \mathbb{C}$ analytisch.
Dann sind äquivalent:
- $f=g$
- Die Menge $\{z\in U: f(z)=g(z)\}$ hat einen [[Häufungspunkt]], der in $U$ liegt.
- Es gibt einen Punkt $\xi \in U$, sodass $f^{(n)}(\xi)= g^{(n)}(\xi)$ für alle $n\in \mathbb{N}$ gilt
*D.h. die Ableitung ist beider Funktionen ist gleich*[^1]

### Komplexes Kurvenstück
Sei $s$ ein winziges Kurvenstück, auf dem die [[Analytische Funktion]] $f$ 0 ist.

Normalerweise stellt man sich die lokale Transformation an einem [[Kritischer Punkt]] ($f(p) = 0$) so vor, dass eine winzige Umgebung um $p$ nicht wirklich zu 0 zusammengezogen wird, sondern nur auf eine sehr viel winzigere Umgebung, sodass es aussieht, als wäre das Bild ein Punkt. 

Da die Umgebung von $p$ nicht wirklich verschwindet sondern sehr stark zusammengezogen wird, sollte man den kritischen Punkt $p$ durch eine endliche Anzahl von Ableitungen entfernen können.
*(Die obere Erklärung ist stark vereinfacht.)*

Betrachtet man aber wieder das Kurvenstück und einen darauf liegenden Punkt $p$, so sieht man, dass $f(z)$ entlang des Kurvenstückes 0 bleibt.
Das Kurvenstück wird diesmal also wirklich auf einen Punkt zusammengezogen!
Da analytische Funktionen aber lokal Drehstreckungen sind, müssen alle Punkte um $p$ zu einem Punkt zusammengezogen werden. Damit ist $f$ lokal konstant 0 und alle ihre Ableitungen sind 0. 
Es kann damit in der Funktion $f$ keine Veränderung stattfinden! $f$ ist damit konstant 0.
(Needham hat eine präzisere Erklärung genannt: Aus der Tatsache, dass alle Ableitungen 0 sind, muss $f$ in einem schlauchförmigen Gebiet um $s$ konstant 0 sein. Dann wäre $f$ aber auch wg. [[Stetigkeit]] am Rand des Schlauches 0. Die obere Argumentation lässt sich dann fortsetzen.)

Seien $f$ und $g$ zwei Funktionen, für die auf einem Kurvenabschnitt $s$ gilt $f(z) = g(z)$. Dann ist $f-g$ auch eine analytische Funktion mit $(f-g)(z) = 0$ auf $s$.
D.h.: $(f-g) = 0$ für alle $z$ und somit $f=g$.

Eine ähnliche Argumentation müsste man auch mit dem Häufungspunkt machen können:
Dass alle Ableitung im Häufungspunkt $p$ 0 sein müssen, da in jeder Umgebung von $p$ ein anderer Punkt mit $f(z) = 0$ existert, kann die lokale lineare Abbildung die Umgebung nicht einfach stark komprimieren, sondern muss die Umgebung auf einen Punkt reduzieren.


### Riemannsche Flächen
Seien
- $X$ und $Y$ [[Riemannsche Fläche|Riemannsche Flächen]]
- $f: X \to Y$ und $f: X \to Y$ [[Holomorphe Funktion (Riemannsche Fläche)|Holomorphe Funktionen]].
Dann sind äquivalent:
- $f=g$
- Die Menge $\{x\in X: f(x)=g(x)\}$ hat einen Häufungspunkt, der in $U$ liegt.[^3]


### Isoliertheit der Nullstellen
Diese Eigenschaft ist ein Spezialfall des Identitätssatzes.
Sei $f:U \to \mathbb{C}$ mit $f \neq 0$ analytisch.

Dann gibt es für jeden Punkt $a\in U$ einen Radius $r$, sodass für alle Werte $z \in K(a, r) \backslash \{a\}$ gilt
$$f(z)\neq 0$$ *D.h. Die Nullstellen liegen nicht dicht*

### Gleichheit auf offenen Mengen
- Sind $f$ und $g$ of einer nichtleeren offenen Einschränkung gleich, dann gilt $f=g$[^1]

#Mathe-IV 
#Needham 


[^1]: Zenk - Satz 21.2.3
[^2]: Zenk - Korollar 21.2.4
[^3]: Zenk - Satz 24.3.7