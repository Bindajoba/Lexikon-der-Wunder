## Beschreibung

Eine Analytische Funktion f besitzt an jedem Punkt einen offenen Kreis in dem jeder Wert durch eine [[Potenzreihe]] beschrieben werden kann.

Ein fundamentaler Satz zeigt, dass das genau die Funktionen, die **holomorph** sind.
Analytische Funktionen sind Spezialfälle von [[Meromorphe Funktion]]

## Definition
### Analytische Funktion
Seien 
- $U \subset \mathbb{C}$ eine eine [[Offene Menge|offene]] Definitionsmenge von $f$
- $f: U \to \mathbb{C}$

$f$ ist **analytisch**, wenn es zu jedem [[Entwicklungspunkt]] $w\in U$ einen [[Offener Kreis|offenen Kreis]] $K(w, r_w)\subseteq U$ um $w$ mit Radius $r_w>0$ und eine darin [[Konvergenz|konvergente]] [[Potenzreihe]] gibt sodass 
$$f(x)=\sum_{k=0}^\infty{c_k(x-w)^k} \tag{1}$$[^1]

### Holomorphe Funktion
Eine komplexe Funktion ist **holomorph**, wenn sie an jedem Punkt seines Definitionsbereichs [[Differenzierbarkeit|komplex differenzierbar]] ist 

Jede Holomorphe Funktion lässt sich durch eine Potenzreihe darstellen und ist somit eine **Analytische Funktion**

Sei
- $U \subseteq \mathbb{C}$ der Definitionsbereich von $f$ und Wertebereich von $\gamma$
- $f: U \to \mathbb{C}$ eine holomorphe Funktion
- $\overline{K}(a, r) \subseteq U$ ein abgeschlossener Kreis mit Radius $r > 0$ und Mittelpunkt $a \in U$
- $\gamma$ der [[Kreisweg]] mit Radius mit Radius $r$ und Mittelpunkt $a$

Dann hat $f$ die Potenzreihendarstellung
$$f(x)=\sum_{k=0}^\infty{c_k(x-w)^k}$$ mit
$$c_k=\frac{1}{2\pi i} \int\limits_\gamma \frac{f(\xi)}{(\xi - a)^{k+1}} \, d\xi$$[^9]
Der Satz folgt aus der [[Cauchy-Integralformel]]

## Charakterisierungen
### Erhaltung von Quadraten
Differenziert man eine komplexe Funktion erhält man eine lineare Funktion, welche das lokale Verhalten um einen Punkt beschreibt.
Diese lineare Funktion ist eine Drehstreckung. D.h. infinitesimale Figuren werden auf ähnliche infinitesimale Figuren abgebildet. (Quadrate auf Quadrate oder Kreise auf Kreise)[^10]

### Cauchy-Riemannsche Ungleichungen
Erfüllt eine Funktion die [[Cauchy-Riemannsche Differentialgleichungen]], dann ist sie **analytisch**

### Senkrechte Gradienten
Betrachteden Realteil $u$ und Imaginärteil $v$ einer **analytischen Funktion** als Funktionen die eine Ebene auf die reellen Zahlen.

Dann steht die [[Gradient|Richtung der größten Steigung]] dieser beiden Funktionen senkrecht zu einander.

Formal:
$$\nabla u \cdot \nabla v = 0$$

*Ich denke, das ist der Tatsache zuschreiben, dass in der komplexen Ebene der Realteil in linker Richtung und der Imaginärteil in oberer Richtung steigt, also orthogonal zueinander. Analytische Funktionen sind lokal Drehstreckungen, diese Orthogonalität bleibt also erhalten.*[^11]

### Irgendwas mit Dreieck
Eine stetige Funktion $f: U \to \mathbb{C}$ auf der Menge $\emptyset \neq U \subseteq \mathbb{C}$ ist genau dann **analytisch**, wenn:
- Für jedes [[Komplexes Dreieck|Dreieck]] ist das Integral entlang der Kanten gleich 0:
$$\int\limits_\triangle f(z) \, dz = 0$$ mit $\triangle = [[[z_1, z_2]]]\dot +[[[z_2, z_3]]]\dot +[[[z_3, z_1]]]$ **oder**
- Für jeden Punkt $a \in U$ gibt es eine offene Kugel $K(a, r) \subseteq U$, sodass $f|_{K(a, r)}$ eine Stammfunktion besitzt. [^6]

## Sätze
Siehe [[Diverse Sätze zu Analytischen Funktionen]].

## Eigenschaften
### Holomorphie
**Analytische** und **holomorphe Funktionen** und  ist äquivalent

### Taylorreihen
Durch Experimentieren findet man heraus:
Leitet man die Potenzreihendarstellung zum [[Entwicklungspunkt]] $a$
$$f(x)=\sum_{k=0}^\infty{c_k(x-a)^k}$$ n-mal ab und setzt den Punkt a, erhält man
$$f^{(n)}(x)=c_nn! \text{ bzw. } c_n = frac{f^{(n)}(x)}{n!}$$
Dies erinnert uns sehr an die [[Taylorentwicklung]] von $f$.

Daher ist die lokale Potenzentwicklung $(1)$ genau die [[Taylorentwicklung]] von $f$ im Punkt $a$

### Abgeschlossenheit
Seien $f: U \to \mathbb{C}$ und $f: U \to \mathbb{C}$ analytisch.

Wenn U [[Zusammenhängende Menge|zusammenhängend]] ist, dann 
- die Summe von $f$ und $g$ ist analytisch 
- das Produkt von $f$ und $g$ ist analytisch [^4]

### Stammfunktion
Jede **analytische Funktion** f besitzt **lokale Stammfunktionen**, d.h.
eine [[Einschränkung]] $f|_V$ auf die Menge $V \subseteq U$, sodass $f|_V$ eine [[Stammfunktion (Analysis)]] besitzt.  [^5]

Siehe auch [[Analytische Funktion mit Stammfunktion]]

### Konvergenz analytischer Funktionen
Sei
- $(f_n: U \to \mathbb{C})_{n \in \mathbb{N}}$ eine Folge von analytischen Funktionen, die [[Lokal Gleichmäßige Konvergenz|lokal gleichmäßig]] gegen $f: U \to \mathbb{C}$ konvergiert 

Dann ist $f: U \to \mathbb{C}$ analytisch und die Folge $(f_n^{(k)})_{n \in \mathbb{N}}$ der k-ten Ableitungen konvergiert lokal gleichmäßig gegen die k-te Ableitung $f^{(k)}$ von $f$.[^7]

### Eigenschaften Injektive Funktionen
Ist $f$ analytisch und [[Injektive Abbildung|injektiv]], dann gilt $f'(z) \neq 0$ für alle $z \mathbb{C}$[^8]

## Laurentreihe
Jede Analytische Funktion kann durch eine [[Laurentreihe]] dargestellt werden.

## Nullstellen
### Satz von Rouché
Der [[Satz von Rouché]] gibt Voraussetzungen, wann eine im Inneren einer Schleife gleich viele Nullstellen von $f$ und $f+g$ existieren.


### Satz von Hurwitz
Der [[Satz von Hurwitz]] sagt, wann der Grenzwert einer [[Folge]] von analytischen Funktionen [[Nullstelle|Nullstellen]] hat 

## Beispiele
Alle wichtigen Funktionen mit Namen sind meist analytisch. [^2]
- [[Exponentialfunktion]] 
- [[Sinus und Kosinus]]
- [[Polynom (Komplexe Analysis)|Polynome]]
- [[Komplexe Logarithmusfunktion]]
- $f_a: t \mapsto \frac{1}{z-a}$ mit der Potenzreihenentwicklung zum [[Entwicklungspunkt]] $w$:
$$f_a(x) = \frac{1}{w-a}\sum^\infty_{k=0}(\frac{w-z}{w-a})^k$$ und dem Konvergenzradius
$$r = |w-a|$$[^3]



#Mathe-III 
#Mathe-IV 
#Needham 

[^1]: Zenk - Definition 21.1.1
[^2]: 3b1b - https://www.youtube.com/watch?v=sD0NjbwqlYw&t=1072s
[^3]: Zenk - Beispiel 21.1.2
[^4]: Zenk - Lemma 21.2.5
[^5]: Zenk - Satz 22.4.2
[^6]: Zenk - Satz 22.4.8
[^7]: Zenk - Satz 22.8.1
[^8]: Zenk - Lemma 25.1.1
[^9]: Zenk - Satz 22.4.1
[^10]: Needham - Abschnitt 4.4.3
[^11]: Needham - Aufgabe 5.1