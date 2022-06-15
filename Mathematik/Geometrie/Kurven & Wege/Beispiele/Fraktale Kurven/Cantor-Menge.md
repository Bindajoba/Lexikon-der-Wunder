TARGET DECK: Universität::Mathematik::Geometrie

# Beschreibung
Die **Kantormenge** ist ein lustiges Fraktal.

# Konstruktion
## In Bildern
![](https://upload.wikimedia.org/wikipedia/commons/thumb/2/26/Cantor5.svg/1280px-Cantor5.svg.png)
Wir erzeugen Mengen indem wir immer das mittlere Drittel entfernen. Der Schnitt all dieser Mengen wir die **Cantor-Menge** $C$ genannt


## In Formeln
$$C = \ges{\sum_{i=1}^{\infty} a_i \frac{1}{3^i}:a_i \in \ges{0, 2}} $$
Also ist jede Zahl ist dadurch bestimmt, ob sie im linken oder im rechten Teilstück liegt.


# Eigenschaften
## Eindeutige Darstellung aller Elemente als Folge
Es gibt eine [[Bijektive Abbildung]] $C \to \ges{\text{ Folgen }(a_i)_{i+1}, a_i \in \ges{0, 2}} =: F$

*Diese Folge ist wie eine Addressierun gin einem [[Binärbaum]]!*


## Abstand zwischen zwei Punkten
Falls $(a_i), (b_i) \in F$ und $a_i = b_i$ für alle $i \leq n$ aber $a_n \neq b_n$
$\implies \| \sum \frac{a_i}{3^i}-\sum \frac{b_i}{3^i}\| \geq \frac{1}{3^i}$

Dieser Abstand definiert sogar eine [[Metrik]] auf $F$.

## Andere Metrik
Man kann auch folgende Metrik definieren
$$d((a_i), (b_i)) = \frac{1}{3^n}$$
wobei $n$ der erste Index ist, bei dem sich $a_i$ und $b_i$ unterscheiden.

## Abbildung auf $[0, 1]$
Es gibt eine [[Stetigkeit|stetige]] [[Surjektive Abbildung]] Abbildung $C \to [0, 1]$.

Jedes Element $(a_i)_{i \in \N} \in F$ ist um Grunde eine [[Binärzahl]] (sie hat nur Werte 0 und 2). Bilde diese Zahl auf die Binärdarstellung einer reellen Kommazahl ab.

*Das ganze ist nicht bijektiv, da die Cantorzahlen $0,1$ und $0,011111111...$ auf die gleiche reelle Zahl abbilden.*

## Surjektive Abbildung auf $C^2$
Es gibt eine [[Bijektive Abbildung|bijektive]], stetige Abbildung $u: C \to C^2$

Sei $b = (b_i)_i, c=(c_i)_i \in F$. Indem wir $b$ und $c$ so verschränken, dass das nächste Element alle zwei Folgenglieder auftaucht, erhalten wir eine neue Folge $a = (b_1, c_1, b_2, c_2, ...)$.

Die Abbildung $u$ kehrt diesen Prozess um. Sie nimmt eine Folge $a$ und teilt diese in zwei Folgen, d.h. auf zwei Elemente $b, c$ auf. Dadurch können wir jede zwei Elemente $b, c \in F^2 = C^2$ durch ein Element $a \in F = C$ erhalten.

Das ganze ist stetig, da für sehr nahe Elemente $a$ und $a'$ auch die Elemente $(b, c), (b', c')$ sehr nah sind.

Die Umkehrung dieses Vorgehens gibt uns eine surjektive Umkehrfunktion.

## Stetige Fortsetzung von $C \to [0, 1]^2$ auf $[0,1] \to [0, 1]^2$
Die Abbildung $C \to [0, 1]^2$ ist bereits surjektiv. Wir können sie stetig machen, indem wir die Lücke zwischen zwei Punkten von $C$ auf eine Kurve zwischen deren Bildpunkten abbilden.
Die resultierende Funktion ist natürlich immer noch surjektiv aber jetzt außerdem stetig.

#Geometrie





$\newcommand{\ges}[1]{\left\{ #1 \right\}}$
$\newcommand{\wink}[1]{\left\langle #1 \right\rangle}$
$\newcommand{\klam}[1]{\left( #1 \right)}$
$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$
