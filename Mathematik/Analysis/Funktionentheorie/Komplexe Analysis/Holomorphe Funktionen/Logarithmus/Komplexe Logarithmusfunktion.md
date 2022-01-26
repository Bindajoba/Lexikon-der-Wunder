## Beschreibung
Der komplexe Logarithmus ist die [[Umkehrabbildung]] der [[Exponentialfunktion|komplexen Exponentialfunktion]].
Diese Definition bringt aber einige Probleme mit sich: So ist zum Beispiel das [[Urbild]] der Punktmenge $\{e\}$:
$$\exp^{-1}(\{e\}) = \{e + 2\pi i : k \in \mathbb{Z}\}$$ Die Umkehrfunktion von $e^z$ ist also offensichtlich nicht eindeutig.[^1] Die Umkehrfunktion ist aber trotzdem stetig. Was passiert, ist dass die Umkehrfunktion eine Schraube bildet, die sich immer weiter nach unten windet.

![[Komplexer Logarithmus.png]]

## Definition
### Zweig des Logarithmus
Sei $\emptyset \neq U \subseteq \mathbb{C} \backslash \{0\}$ ein [[Gebiet]]. 
Eine [[Stetigkeit|stetige]] Funktion $\log: U \to \mathbb{C}$ heißt ein **Zweig des Logarithmus auf $U$**, wenn
$$e^{\log(z)} = z$$ für alle $z \in U$ gilt.[^2]
*Die Bedingung sieht aus, als wäre log eine Umkehrfunktion, das ist sie aber nicht.*

In dem Fall ist $\log$ [[Analytische Funktion|analytisch]]

### Hauptzweig des Logarithmus
Auf $\mathbb{C} \backslash ]- \infty, 0]$ existiert ein Zweig des Logarithmus, der für reelle Werte genau der [[Logarithmus|natürliche Logarithmus]] ist.
$$Log(z) := \int\limits_{[[[1, z]]]}\frac{1}{\xi}\,d\xi$$[^5]

## Äquivalente Definitionen
### Potenzreihe
Der Hauptzweig des Logarithmus hat die Potenzreihenentwicklung:
$$\ln(z+1) = \sum_{n = 1}^\infty (-1)^{k+1}\frac{z^k}{k} = z-\frac{z^2}{2} + \frac{z^3}{3} - ...$$
Das erhält man, indem man $\frac{1}{z+1}$ als Potenzreihe ausschreibt und integriert.

## Eigenschaften
### Ableitung
Die Ableitung für jeden Zweig des Logarithmus ist $log'(z) = \frac{1}{z}$ für alle $z \in U$[^3]

### Stammfunktion von 1/x
Sei $\emptyset \neq U \subseteq \mathbb{C} \backslash \{0\}$ ein [[Gebiet]]. 
Dann sind äquivalent:
1. Es existiert ein Zweig $log: U \to \mathbb{C}$ des Logarithmus auf $U$
2. $f: \begin{array}{rcl} U &\to & \mathbb{C} \\ z &\mapsto & \frac{1}{z} \end{array}$ besitzt auf U eine [[Stammfunktion (Analysis)|analytische Stammfunktion]].
3. Für jede [[Komplexe Stückweise Differenzierbare Schleife]] $\gamma: [0,1] \to U$ in $U$ ist $n(\gamma, 0) = 0$[^4]

*Das ist ziemlich offensichtlich. Zum einen ist der log die Stammfunktion von $\frac{1}{z}$, also ist es irgendwie klar, dass $\frac{1}{z}$ eine Stamfunktion besitzt. Zum anderen muss $\log$ stetig sein. Und das geht aufgrund der Schraubenform nur dann, wenn man in $U$ keine [[Komplexe Stückweise Differenzierbare Schleife|Schleife]] um $0$ legen kann. (Also $U$ [[Einfach Zusammenhängende Menge|einfach zusammenhängend]] ist) Aber dann ist jedes [[Wegintegral]] um eine [[Komplexe Stückweise Differenzierbare Schleife|Schleife]] gleich $0$.*

### Differenz zweier Zweige
Sei 
- $\emptyset \neq U \subseteq \mathbb{C} \backslash \{0\}$ ein [[Gebiet]].
- $f, g: U \to \mathbb{C}$ Zweige des Logarithmus.

Dann ist $f-g$ eine konstante Funktion, die nur die Werte $2\pi i \mathbb{Z}$ annehmen kann.[^6]

#Mathe-IV 

[^1]: https://www.youtube.com/watch?v=SYxyemNSSm8
[^2]: Zenk - Definition 23.3.1
[^3]: Zenk - Lemma 23.3.2
[^4]: Zenk - Satz 23.3.3
[^5]: Zenk - Bemerkung 23.3.4
[^6]: Zenk - Lemma 23.2.5