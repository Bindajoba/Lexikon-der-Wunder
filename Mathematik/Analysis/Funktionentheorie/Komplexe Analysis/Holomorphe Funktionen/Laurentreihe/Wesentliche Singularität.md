## Beschreibung

## Definition
Eine [[Isolierte Singularität]] $a$ heißt eine **Wesentliche Singularität** von der [[Analytische Funktion|analytischen Funktion]] $f$, wenn der [[Isolierte Singularität|Hauptteil]] von $f$ in $a$ kein Polynom in der Variablen $\frac{1}{z-a}$, also $c_{-k}\neq 0$ für unendlich viele $k \in \mathbb{N}$ ist.**

*Das heißt, der Hauptteil ist so was wie ein unendlich langes Polynom zur Variable $\frac{1}{z-a}$*

## Eigenschaften
### Satz von Casorati-Weierstraß
Sei
- $U \subseteq \mathbb{C}$ eine [[Offene Menge|offene Menge]]
- $f: U \to \mathbb{C}$ [[Analytische Funktion|analytisch]]
- $a\in \mathbb{C}$ eine [[Isolierte Singularität]] von $f$.

$a$ ist genau dann eine Wesentliche Singularität von $f$, wenn
- für jedes $r>0$: $f(\dot K(a, r) \cap U)$ eine [[Dichte Menge|dichte Teilmenge]] von $\mathbb{C}$ ODER
*Ich konnte mir anfangs nicht Vorstellen, warum das Bild eine dichte Menge von $\mathbb{C}$ ist und nicht einfach gleich $\mathbb{C}$. Was gibt es für eine interessante Menge, die dicht in $\mathbb{C}$ liegt.
Es stellt sich heraus, $\mathbb{C} \backslash \{0\}$ ist genau so eine Menge.*[^2] 
- es zwei Folgen $(w_n)_{n\in \mathbb{N}}$ und $(z_n)_{n\in \mathbb{N}}$ in $U$ gibt mit $a = \underset{n \to \infty}{\lim} w_n = \underset{n \to \infty}{\lim} z_n$, sodass $\underset{n \to \infty}{\lim} f(w_n) \neq \underset{n \to \infty}{\lim} f(z_n)$
*Beachte: Bei $\frac{1}{z}$ gibt es ebenfalls twei Folgen, die nicht gegen den gleichen Wert konvergieren. Aber da geht die Beträge gegen unendlich, daher zählt es anscheinend nicht.*


### Großer Satz von Picard
Sei
- $\emptyset \neq U \subseteq \mathbb{C}$ eine [[Offene Menge|offene Menge]]
- $f: U \backslash\{a\} \to \mathbb{C}$ [[Analytische Funktion|analytisch]]
- $a\in \mathbb{C}$ eine wesentliche Singularität von $f$.

Dann gilt für jede punktierte Umgebung $V$ von $a$:
- $f(V) = \mathbb{C}$ oder
- Es gibt ein $b = b(f, V) \in \mathbb{C}$ mit $\mathbb{C}\backslash \{b\}$

Mit Ausnahme von höchstens einer komplexen Zahl $b(f, V)$ wird jedes andere $c\in \mathbb{C}$ von $f|_{V}$ unendlich oft als Funktionswert angenommen.

D.h. $|\{z \in V: f(z) = c\}| = \infty$

*Das sieht mir nach einer besseren Version des Satzes von Casorati.Weierstraß aus*[^3]




## Beispiele
Die Funktion $f(z)=e^{\frac{1}{z}}$ hat eine wesentliche Singularität bei 0.
Das erkennt man gut, wenn man die [[Exponentialfunktion]] in die Potenzreihendarstellung umwandelt und $\frac{1}{z}$ einsetzt:
$$f(z)=e^{\frac{1}{z}} = \sum_{n=0}^\infty \frac{1}{n!}\frac{1}{z^n} = \sum_{n=-\infty}^0 \frac{1}{(-n)!}z^n$$
Im Bild unten erkennt man gut, warum das Bild eines [[Punktierter Offener Kreis|punktierten offenen Kreises]] dicht in $\mathbb{C}$ liegt.

Der Farbton entspricht dem komplexen Argument des Funktionswertes, während die Helligkeit seinen Betrag darstellt.
![[Wesentliche Singularität.png]]
Man erkennt: Nähert man sich von unten der Singularität, werden alle komplexen Argumente durchlaufen.
Nähert man sich von rechts wird der Betrag unendlich groß.
Nähert man sich von links geht der Betrag gegen 0.

Aufgrund der Stetigkeit sind alle dazwischenliegenden Werte ebenfalls im Bild enthalten. Der einzige Wert, der nicht im Bild ist, ist 0, da dieser genau durch die Annäherung von der linken Seite erlangt werden kann.[^1]

#Mathe-IV 

[^1]:  https://de.wikipedia.org/wiki/Isolierte_Singularit%C3%A4t
[^2]: Zenk - Satz 23.1.12, Satz 23.1.13
[^3]: Zenk - Satz 26.1.1