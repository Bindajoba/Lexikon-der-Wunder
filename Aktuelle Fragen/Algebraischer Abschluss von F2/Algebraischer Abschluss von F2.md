$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$


# Abstract
Was Algebraischer Abschluss von $\mathbb{F}_2$?

# Koncret (damit es Flo von Artifexian auch durchließt)
In der Mathematik kann man Gleichungen aufstellen, in denen nur $+, -, :, *$ verwendet wird, z.B.:
$$\frac{x+\frac{4}{5}}{x^2 + 4} = x^3 + \frac{x^2}{5*7}$$
Jede dieser Gleichungen kann durch Äquivalenzumformungen schrittweise vereinfacht werden.
$$\begin{align} \frac{x+\frac{4}{5}}{x^2 + 4} &= x^3 + \frac{x^2}{35}\\
x+\frac{4}{5} &= (x^3 + \frac{x^2}{35})(x^2 + 4)\\
(x+\frac{4}{5})35 &= (35x^3 + x^2)(x^2 + 4)\\
35x+28 &= 35x^5+x^4+140x^3+4x^2\\
0 &= 35x^5+x^4+140x^3+4x^2 - 35x -28
\end{align}$$
Jede der oben stehenden Gleichungen wird durch das Einsetzen der Gleichungslösungen erfüllt. Diese Lösungen verändern sich, da wir Äquivalenzumformungen verwendet haben, nicht.
Das bedeutet überraschenderweise, dass die Nullstellen des Polynom ganz unten die oberste Gleichung lösen.

Das Beispiel eben war exemplarisch gewählt aber tatsächlich kann man jede Gleichung mit nur einer Variablen, die nur $+, -, *, :$ verwendet in ein Polynom vereinfachen.

Deshalb sind Nullstellen von Polynomen in Mathematik so wichtig und Mathematiker interessieren sich dann auch dafür, ob diese Nullstellen rational, reell oder sogar etwas anderes sein könnten.

*In der oberen Erklärung müsste man Nullen im Nenner mit berücksichtigen, das habe ich der Einfachkeit halber übergangen.*

## Was ist ein Algebraischer Abschluss?
Der Traum des Mathematikers ist, dass jedes Polynom mit rationalen Koeffizienten (z.B. $\frac{3}{2}x^2 + \frac{1}{27}x +1$) auch (1) **rationale Nullstellen** hat und in (2) **Nullstellenform** gebracht werden kann.

*Wären die Nullstellen von Polynomen mit rationalen Koeffizienten rational, dann hätte man eine Einschränkung, wie die Nullstellen aussehen und das Erfinden eines Algorithmuses zu Finden solcher Nullstellen wäre auch leichter.*

Leider ist das nicht so, wie man am Polynom $p(x) = x^2 -2$ gut erkennt. $p$ kann zwar in Nullstellenform gebracht werden $p(x) = x^2-2 = (x+\sqrt{2})(x-\sqrt{2})$ kann aber wie man sieht die nicht-rationalen Nullstellen $\pm \sqrt{2}$.

Wie sieht es mit $\mathbb{R}$ aus? Hat ein Polynom mit reellen Koeffizienten auch reelle Nullstellen und kann in Nullstellenform gebracht werden?
Das Polynom $p_1(x) = x^2+1$ kann in Nullstellenform gebracht werden, wenn wir uns der Zahl $i = \sqrt{-1}$  der komplexen Zahlen bedienen:
$$p_1(x) = x^2+1 = (x+i)(x-i)$$
(Die Gleichung ist mit der Binomischen Formel und Anwendung der Regel $i^2 = -1$ leicht zu zeigen).
Das Polynom hat, wie man aus der Nullstellenform ablesen kann, die Nullstellen $\pm i$. Die sind aber nicht reell.

Es scheint so, als ob die Eigenschaft (1) und (2) nicht gleichzeitig erfüllt sein kann, da man immer Arten von Zahlen als Nullstellen herauskommen könnten, die ganz anders sind als die, aus denen wir unser Polynom konstruieren.

**
Daher ist folgender Satz eventuell überraschend: Wenn die Koeffizienten von Polynomen komplexe Zahlen sind, dann sind auch die Nullstellen komplexe Zahlen und das Polynom kann immer in Nullstellenform gebracht werden.
Man braucht nicht zu verstehen, was komplexe Zahlen sind und welche Eigenschaften sie haben. Relevant ist, der eben formulierte Satz. Eine Menge, die die Eigenschaft (1) und (2) erfüllt nennt man **algebraisch abgeschlossen** (*das wird nicht mehr auftauchen es steht nur der Vollständigkeit halber da*).

Der **Algebraische Abschluss** ist ein verwandtes Konzept.
Der Algebraische Abschluss von $\mathbb{R}$ sind alle Zahlen, die Nullstellen von Polynomen sind, welche rationale Koeffizienten haben. 
Das beinhaltet alle Zahlen aus den vorherigen Beispielen. z.B.:
- die Nullstellen $\pm \sqrt{2}$ von $x^2-2$ sind Element des Algebraischen Abschlusses von $\mathbb{R}$ 
- die Nullstellen $\pm i$ von $x^2+1$ sind Element des Algebraischen Abschlusses von $\mathbb{R}$ 
- die Nullstellen von $\pi x^2+e$ sind Element des Algebraischen Abschlusses von $\mathbb{R}$ 
- die Nullstellen von $\frac{3}{2}x^2 + \frac{1}{27}x +1$ sind Element des Algebraischen Abschlusses von $\mathbb{R}$ 

## Was ist $\mathbb{F}_2$?
$\mathbb{F}_2$ ist die Menge $\{0, 1\}$. Lustigerweise kann man auf dieser Menge (fast) sinnvoll addieren, subtrahieren, multiplizieren und dividieren.

Die Regeln sind folgende:
Addition:
- $0+0 = 0$
- $0+1=1+0=1$
- $1+1 =0$

Subtraktion
- $0-0 = 0$
- $1-0 = 1$
- $0-1 = 1$
- $1-1 = 0$

*Man bemerkt, dass Addition und Subtraktion gleich ist. Warum das so sein muss, erkennt man wenn man bei der Subtraktion eine Äquivelenzumformung anwendet $0-1 = 1 \implies 0 = 1+1$. Die Operationen +, - sind so definiert, dass Äquivelenzumformungen von Gleichungen funktionieren.*
Das bedeutet, dass man das $+$ Zeichen durch ein $-$ Zeichen ersetzen kann, ohne das Ergebnis zu verändern.


Multiplikation
- $0*0 = 0$
- $0*1 = 1*0 = 0$
- $1*1 = 1$

Division
- $0:0 = 1:0 = undefiniert$ (Wir erlauben auch hier keine Division durch null)
- $0:1 = 0$
- $1:1 = 1$

*Vielleicht ist aufgefallen, dass die Addition sich wie eine logisches XOR-Gatter verhält und die Multiplikation wie ein logisches AND-Gatter. Eventuell kann man damit die Anwendungswelt der Menge $\{0,1\}$ und seiner Operationen langsam erahnen.*

## $\mathbb{F}_2$-Polynome
Ab nun läuft die Verallgemeinerung der Mathematik Amok. Wir suchen die gelernten zwei Konzepte zwangvoll zu verknüpfen. Ich bin mir nicht sicher, welche Verwendung das Ergebnis haben könnte aber es ist meiner Meinung nach eine interessante Übung und ein Beispiel, auf das man sich beim Algebrastudium zurückerinnern kann.

Wir definieren nun Polynome die als Koeffizienten $0$ oder $1$ haben.
Diese speziellen Polynome gehorchen den oberen Rechenregeln. z.B.:
$$(1x^2 + 1x + 1) + (1x^2 + 1x + 0) = (1+1)x^2 + (1+1)x + (1+0) = 0x^2 + 0x + 1 = 1$$
oder
$$(1x + 1) + (1x + 1) = (1+1)x + (1+1) = 0x + 0 = 0$$
Wie man sehen kann, haben die Polynome die kuriose Eigenschaft, dass sie sich Auslösche, wenn man sie mit sich selbst addiert.

Desweiteren haben auch diese speziellen Polynome Nullstellen und können in Nullstellenform gebracht werden:
$$x^2 + x = x(x + 1) = (x+0)(x+1)$$
oder
$$x^2+1 = (x+1)(x+1)$$
wie man mit der binomischen Formel nachrechnen kann.

Die Frage des Abstract besagt: Gibt es Polynome, die nicht 0 oder 1 als Nullstelle haben und wenn ja, kann man sich eine Nullstelle für sie ausdenken?


# Eigentlicher Teil
[[Algebraischer Abschluss|Algebraische Abschlüsse]] sind vielleicht ein bisschen schwierg zu erhalten. Wir wissen aber, dass jede Lösung eines Polynoms im Algebraischen Abschluss liegt. Es wäre somit keine dumme Idee einfach mal den [[Zerfällungskörper]] $L$ über alle Polynome zu berechnen.

Da wir dadurch einen Körper erhalten, dessen Elemente Lösungen von $\mathbb{F}_2[x]$-Polynomen sind, ist die [[Körpererweiterung]] $L|\mathbb{F}_2$ algebraisch.
Ist dieser zusätzlich [[Algebraisch Abgeschlossener Körper|algebraisch abgeschlossen]], so haben den Algebraischen Abschluss gefunden!

# Zerfällungskörper von $\mathbb{F}_2$ durch Untersuchung aller Polynome
Nach VL lässt sich in einem Zerfällungskörper ein Polynom in Linearfaktoren aufteilen. Probieren probieren wir das einfach, indem wir alle Polynomen $\mathbb{F}_2[x]$ der Reihe nach klassifizieren.
"Der Reihe nach" bedeutet, dass die Koeffizienten $a_k \in \mathbb{F}_2$ zu einer Binärzahl zusammengesetzt werden und der Größe nach sortiert werden. 

## Simple Polynome
Wir gehen alle Polynome nach oben angesprochener Ordnung durch. 
$$\begin{align}10:&&1x + 0  &= x+0\\
11:&&1x+1 &= x+1\\
100:&&1x^2 + 0x + 0 &= (x+0)^2\\
101:&&1x^2 + 0x + 1 &= (x+1)^2\\
110:&&1x^2 + 1x + 0 &= (x+0)(x+1)
\end{align}$$
## Erste exotische Nullstelle
Jetzt kommen wir zu dem ersten Polynom, was nicht $0$ oder $1$ als Nullstelle hat.
Nennen wir die beiden Nullstellen erstmal $\alpha_1$ und $\alpha_2$. Es entsteht die Zerlegung:
$$111:x^2+x+1 = (x-\alpha_1)(x-\alpha_2)$$
Es wäre interessant zu wissen, ob die Nulltellen $\alpha_1, \alpha_2$ gleich sein können. Nehmen dazu an, sie wären gleich. Dann gilt:
$$x^2 + x + 1 = (x-\alpha_1)(x-\alpha_1) = x^2 -2\alpha_1x + \alpha_1^2 = x^2 + \alpha_1^2$$
das Polynom links und das Polynom rechts sind nicht gleich, wie man durch Koeffizientenvergleich erkennt, wir erhalten einen Widerspruch.

### Exkurs: Kann ein Minimalpolynom zweiten Grades in zwei gleiche Nullstellen zerfallen?
Sei $\mu_{K, \alpha}(x) = x^2 + bx + c$ ein in $K$ irreduzibles Polynom mit der einzigen Nullstelle $\alpha \notin K$.
In $K(\alpha)$ zerfällt das Minimalpolynom zu $\mu_{K, \alpha}(x) = (x - \alpha)(x-\alpha)$
Dann gilt:
$$\mu_{K, \alpha}(x) = x^2 + bx + c = (x-\alpha)^2 = x^2 -2\alpha x + \alpha^2$$
Daraus folgt durch Koeffizientenvergleich:
$$b = -2\alpha \text{ und } c = \alpha^2 \implies c = \frac{1}{4}b^2$$
Einsetzen in $\mu_{K, \alpha}$ ergibt: $\mu_{K, \alpha}(x) = x^2 + bx + c = x^2 +bx + \frac{1}{4}b^2 = (x+\frac{1}{2}b)^2$

*D.h. ein Polynom von Grad 2 mit einer doppelten Nullstelle muss die Form $x^2 +bx + \frac{1}{4}b^2$ und die Nullstelle $-\frac{1}{2}b$ haben. Da $\frac{1}{4}b \in K \implies -\frac{1}{2}b \in K$ kann ein Polynom zweiten Grades mit einer doppelten Nullstelle nicht irreduzibel sein.*

### Eigenschaften der ersten exotischen Nullstelle
Wir wenden wieder den gleichen Trick an, um mehr Informationen zu erhalten.
$$x^2 + x + 1 = (x-\alpha_1)(x-\alpha_2) = x^2 -(\alpha_1+\alpha_2)x + \alpha_1\alpha_2$$
Durch Koeffizientenvergleich erhalten wir:
$$I: \alpha_1 + \alpha_2 = 1 \text{ und }II: \alpha_1\alpha_2 = 1$$
*Die Struktur Eigenschaften erinnern mich an die Elementarsymmetrische Polynome von denen Charles Hadlock erzählt hat. Vielleicht werden die noch relevant.*

Gleichung $I$ gibt uns ziemlich expliziten Aufschluss darüber, wie $\alpha_1$ und $\alpha_2$ miteinander in Verbindung stehen: $\alpha_2 = \alpha_1 +1$

Übrigens, für reelle Wert kann man die Gleichungen in zwei Variablen $(\alpha_1, \alpha_2)$ als Ortslinien visualisieren. Schneiden sich die Ortlinien, so ist der Punkt eine Lösung. 
![[Ortslinie Gleichungen.png]]
*Die Ortslinien sind Achsensymetrisch. Das hat damit zu tun, dass das Einsetzen von (exemplarisch) $(1, 2)$ in die linke Seite der Gleichungen das gleiche Ergebnis gibt wie wenn man $(2,1)$ einsetzt. Das ist eine grundlegende Eigenschat der Elementarsymmetrischen Polynome, interessant, nicht wahr?*

### Exkurs: Mitternachtsformel auf Körpern
Statt der oberen Gleichungen könnten wir auch direkt versuchen, die Nullstellen zu berechnen.
Die $p,q$-Formel (eine spezielle Form der Mitternachtsformel für normierte Polynome) wurde bisher nur in Teilmengen der komplexen Zahlen benutzt. Vielleicht lässt sich aber die Herleitung auf alle Körper verallgemeinern.

Die Herleitung der Formel ist:
![[Herleitung p,q-Formel.png]]
Wir bemerken schon im dritten Schritt, dass es nicht möglich ist, diese Formel in $\mathbb{F}_2$ herzuleiten. Damit das möglich ist, bräuchte es ein $\frac{1}{2}$, also ein multiplikatives Inverses zu $2=0$, was im Körper ausgeschlossen wird.

Hat man aber einen Körper, mit dem Element $2 \in K$, welches nicht zugleich die Null ist, dann gibt es dazu ein multiplikatives Inverses und die Formel sollte sich genauso herleiten können.
Eine Wurzel zu definieren ist dabei gar nicht so schwierig, die Wurzeln $\pm\sqrt{a}$ sind die Nullstellen des Polynoms $x^2 -a$, was eventuell eine algebraische Erweiterung erfordert aber trotzdem in jedem Körper existieren sollte.

Die Mitternachtsformel funktioniert also meistens, nur in unserem Fall ist sie nutzlos. Schade, setzen wir die Analyse von $\alpha_1, \alpha_2$ fort.

### Berechnung von $\mathbb{F}_2(\alpha_1)$, und $\mathbb{F}_2(\alpha_1, \alpha_2)$
Sofort den ganzen Zerfällungskörper zu berechnen ist ein bisschen ermüdend. Es wäre einfacher  Eigenschaften von Teilkörpern des Zerfällungskörpers zu bestimmen.
Außerdem bemüht sich ein großer Teil der Algebra-Vorlesung darum [[Einfacher Algebraisch Erzeugter Zwischenkörper|einfache algebraische Erweiterungen]] zu verstehen, es wäre blöd, das Wissen nicht anzuwenden.

$\alpha_1$ hat wie wir bereits festgestellt haben das Minimalpolynom $\mu_{\mathbb{F}_2, \alpha_1} = x^2+x+1$.
Daraus folgt die Größe der Erweiteung $[\mathbb{F}_2(\alpha_1) : \mathbb{F}_2] =2$ und $\{1, \alpha_1\}$ ist eine $\mathbb{F}_2$-Basis von $\mathbb{F}_2(\alpha_1)$.

#### Ein paar Linearkombinationen
Daher lässt sich jedes Element im Körper $\mathbb{F}_2$ und damit auch eine Potenz als Linearkombination der Basisvektoren schreiben $\alpha_1^2 = a\alpha_1 + b$ mit $a, b \in \mathbb{F}_2$

Oben haben wir festgestellt, dass $\alpha_2 = \alpha_1+1$, d.h. $\alpha_2 \in \mathbb{F}_2(\alpha_1) \implies \mathbb{F}_2(\alpha_1) = \mathbb{F}_2(\alpha_1, \alpha_2)$

Welche Werte kommen für $\alpha_1^2$ in Frage?
1. $\alpha_1^2 = 0$: Ist nicht möglich, da damit $\alpha_1$ ein [[Nullteiler]] wäre
2. $\alpha_1^2 = \alpha_1$: Würde aufgrund des Kürzungssatzes $\alpha_1 = 1$ implizieren, was der Tatsache widerspricht, dass $1$ und $\alpha_1$ linear unabhängig sind
3. $\alpha_1^2 = 1$: Aus Gleichung $I$: $\alpha_1\alpha_2 = 1 \implies \alpha_1^2\alpha_2^2 = 1 \implies \alpha_2^2 = 1 \implies (\alpha_1+1)^2 = 1 \implies \alpha_1^2 + 1 = 1 \implies \alpha_1^2 = 0$, Widerspruch 
4.  $\alpha_1^2 = \alpha_1 + 1 = \alpha_2$: Nach Ausschlussprinzip die richtige Antwort

Was kann man dann über $\alpha_1^3$ aussagen?
$$\alpha_1^3 = \alpha_2\alpha_1 = (\alpha_1+1)\alpha_1 = \alpha_1^2 + \alpha_1 = (\alpha_1 + 1)+\alpha_1 = 1$$

### Visualisierung mit Cayley-Daigrammen
Ich habe bisher noch keine hilfreichen Diagramme zur Visualisierung von Körpern gesehen. Daher visualisiere ich einfach die Additive und Multiplikative Gruppe von $\mathbb{F}_2(\alpha_1, \alpha_2)$

Visualisieren wir in einem Cayley-Diagramm, was passiert, wenn man auf ein Element $1$ oder $\alpha_1$ dazuaddiert: 
![[Algebraischer Abschluss F2 Cayle I.png]]
Wir erhalten dieses Diagramm, welches genau die gleiche Struktur hat wie das Diagramm der [[Klein 4-Gruppe|Kleinschen 4-Gruppe]]. Damit sind die beiden [[Gruppe|Gruppen]] [[Gruppenisomorphismus|isomorph]] zueinander!

Visualisieren wir die Multiplikative Gruppe:
![[Algebraischer Abschluss F2 Cayley II.png]]
Entfernt man die Null, sieht die Gruppe aus, wie eine Zyklische Gruppe von Ordnung 3!
$\alpha_1$ besitzt deshalb große Ähnlichkeit mit der komplexen dritten Wurzel von $1$: $\zeta:= \sqrt[3]{1} = \cos(2\pi/3) + i\sin(2\pi/3)$.

*Warnung: Dass wir die komplexen Zahlen hinzuziehen, dient nur einer Analogie. Die Komplexen Zahlen sind eine Erweiterung von $\mathbb{R}$. Sie sollten nichts mit $\mathbb{F}_2$ zu tun haben.*

Wir missachten aber die Warnung und stellen die Punkte trotzdem im komplexen Gitter dar:
![[Algebraischer Erweiterung  a Kmplexes Gitter.png]]
*Wir addieren 1 auf die Punkte (orange) oder multiplizieren mit $\alpha_1$ (grün). Ein grüner Pfeil wurde wegen techniker Einschränkungen weggelassen.*
![[Algebraische Erweiterung Koplexes Gitter II.png]]
*Wir addieren $\alpha_1$ auf die Punkte (orange) oder multiplizieren mit $\alpha_1$ (grün)*

Wir können folgende Operationen erkennen.
- Multipliziert man eine Zahl mit $\alpha_1$, so wandert das Ergebnis einen Punkt gegen den Uhrzeigersinn weiter.
- Multipliziert man eine Zahl mit $\alpha_2 = \alpha_1^2$, so wandert das Ergebnis einen Punkt im Uhrzeigersinn weiter.
- Die Addition hat einen faszinierenden Effekt, abhängig davon, welche Zahl $b \in \mathbb{F}_2$ auf welche Zahl addiert wird. Das zweifache Addieren der gleichen Zahl $b$ hat zur Folge, dass man zur Ursprungsposition zurückkehrt. 
Betrachtet man die Addition von $b$ auf allen Punkten gleichzeitig, dann vertauscht die Addition jeweils zwei Punktpaare. 
Beim Addieren von $b$ werden immer die beiden Punkt gegenüber von $b$ vertauscht!
d.h. Addieren von $1$ vertauscht $\alpha_1$ und $\alpha_2$.
Addieren von $\alpha_1$ vertauscht $1$ und $\alpha_2$

Ich bin mir sicher ein ähnliches Verhalten wird sich auch in den anderen Nullstellen größerer Minimalpolynome finden. 

## Weitere simple Polynome
Setzen wir die Polynome fort:
$$\begin{align}
x^3 &= (x+0)^3\\
x^3 + 1 = (x+1)(x^2+x+1) &= (x+1)(x-\alpha_1)(x-\alpha_2)\\
x^3 + x = x(x^2+1) &= (x+0)(x+1)^2\\
\end{align}$$
## Nächste Exotische Nullstelle
Das nächste Polynom hat ebenfalls keine Nullstellen, die wir schon kennen. $\alpha_1, \alpha_2$ sind keine Nullstellen, das können wir nachprüfen, indem wir eine Polynomdivision durchführen (die Nullstellen $\alpha_1, \alpha_2$ haben ein Minmalpolynom von Grad 2): $x^3+x+1:x^2+x+1 = x, R:x^2+1$. 

Ein Polynom von Grad 3 sollte in drei Linearfaktoren zerlegbar sein. Geben wir den neu entdeckten Nullstellen einen Namen. (z.B. $\beta_1, \beta_2$ und $\beta_3$)
Inzwischen sollte aber absehbar sein, dass durch den Zerfällungskörper unendlich viele Nullstellen kommen könnten. Benennen wir die Nullstellen nach dem Alphabet, gehen uns irgendwann die Zeichen aus. Wir nennen die Nullstellen daher $\xi_{3, 1, 1}, \xi_{3, 1, 2}, \xi_{3, 1, 3}$ mit der Konvention $\xi_{k, i, j}$, wobei
- $k$ für den Grad des Minimalpolynoms der gefundenen Nullstelle steht
- $i$ für die Durchnummerierung der Nullstellen-Grüppchen ist, falls wir bei einem Polynom gleichen Grades noch mehr neue Nullstellen finden (wir werden mehr Grüppchen finden)
- $j$ für die Durchnummerierung und Unterscheidung innerhalb eines Grüppchen.

Passen wir $\alpha_1$ und $\alpha_2$ an das System an:
$\alpha_1$ hat als Minimalpolynom wie oben festgestellt, $x^2+x+1$, also Grad 2. Es gibt nur ein Nullstellen-Grüppchen bei den Polynomen von Grad 2, da wir alle Polynome von Grad 2 klassifiziert haben. Innerhalb dieses Grüppchens legen wir $\alpha_1$ als das erste Element fest.
Damit erhält $\alpha_1$ die neue Bezeichnung $\xi_{2, 1, 1}$ und $\alpha_2$ die Bezeichnung $\xi_{2, 1, 2}$.

Grüppchen können so nur durch die ersten zwei Zahlen und einem $\xi$-Majuskel $\Xi$ bezeichnet werden. z.B. $\Xi_{3,1} = \{\xi_{3,1,1}, \xi_{3,1,2}, \xi_{3,1,2}\}$

## Eigenschaften der Nullstellen $\Xi_{3,1}$
Matthias hat mir folgenden Trick gezeigt:
Die Nullstellen lösen $x^3 + x+1$. Damit müssen sie $x^3 = x+1$ erfüllen.
Sei $\beta$ eine Nullstelle, die die Gleichung löst.


Dann ist $\F(\beta)$ ein $\F$-Vektorraum mit der Basis $\{1, \beta, \beta^2\}$.
Somit hat es die Elemente: $\F(\beta) = \{a\beta^2+b\beta+c:a,b,c\in \F\} = \{0, 1, \beta, \beta+1, \beta^2, \beta^2+1, \beta^2+\beta, \beta^2+\beta+1\}$.
Mich würde interessieren, welche dieser Werte $f(x) = x^3+x+1$ löst.
Es gilt: $\beta^3 = \beta + 1$ und damit auch $\beta^4 = \beta^2 + \beta, \beta^5 = ...$
- $\beta$ löst es nach Definition
- $f(\beta+1) = (\beta+1)^3+(\beta+1)+1 = (\beta^3+\beta^2+\beta+1)+(\beta+1)+1 =\beta^3+\beta^2+1=\beta^2+\beta\neq 0$
- $f(\beta^2) = \beta^6 + \beta^2 + 1 = \beta^4+\beta^3+\beta^2+1 = \beta^2+\beta+\beta+1+\beta^2+1 = 0$
- $f(\beta^2+1) = (\beta^2+1)^3+(\beta^2+1)+1 = (\beta^6+\beta^4+\beta^2+1)+\beta^2$$=(\beta^4+\beta^3)+(\beta^2+\beta)+1 = (\beta^2+\beta+\beta+1)+(\beta^2+\beta)+1 =\beta \neq 0$
- $f(\beta^2+\beta) = (\beta^6+\beta^5+\beta^4+\beta^3)+(\beta^2+\beta)+1=((\beta^4+\beta^3)+(\beta^3+\beta^2)+\beta^4+\beta^3)+(\beta^2+\beta)+1$$=\beta^3+\beta+1 = 0$

Wir haben drei Werte gefunden, die das Polynom lösen: $\{\beta, \beta^2, \beta^2+\beta\}$
Außerdem gibt es noch drei andere Werte, die übrig bleiben: $\{\beta+1, \beta^2+1, \beta^2+\beta+1\}$

WIr könnten uns nun fragen, welches Minimalpolynom diese haben. Dazu bestimmen wir mit der Gradformel den Grad des Polynoms.
Sei $\gamma$ einer der drei Werte. Wegen $\gamma \in \F(\beta)$ gilt:
$$3=[\F(\beta):\F]=[\F(\beta):\F(\gamma)]\cdot[\F(\gamma):\F]$$
$[\F(\gamma):\F]$ muss $3$ teilen. Wäre $[\F(\gamma):\F]=1$, dann wäre $\F(\gamma)=\F$, was nicht sein kann. Somit ist $[\F(\gamma):\F] = 3$.
Die einzigen drei Polynome dritten Grades, die wir noch nicht untersucht haben sind:
- $x^3+x^2$
- $x^3+x^2+1$
- $x^3+x^2+x$
- $x^3+x^2+x+1$

Das gesuchte Minimalpolynom muss irreduzibel sein, d.h. nicht 1 oder 0 als Nullstelle besitzen.
Übrig bleibt: $x^3+x^2+1$.

Setzt man $\{\beta+1, \beta^2+1, \beta^2+\beta+1\}$ in $x^3+x^2+1$ ein, kommt 0 heraus.

## Visualisierung
Was passiert, wenn wir mit $1$ anfangen und die ganze Zeit $\beta$ mutliplizieren?
![[Visualisierung Beta.png]]
Die Multiplikation hat die Form einer Zyklischen Gruppe. 
Ich habe die Nullstellen die das gleiche Minmalpolynom haben eingefärbt.
Orange hat die Nullstellen $\gamma, \gamma^2, \gamma^4$. Also $\gamma^{2^n}$-Potenzen ($\gamma^8 = \gamma$). Vielleicht ist das kein Zufall.

Die Addition ist aber etwas schwerer zu erkennen. Vielleicht können wir die Position der Kreise ändern.

![[Algebraischer Abschluss Beta Visualisierung.png]]
Frage: Wie kann ich im Bild vorhersehen, wohin mich die Blauen Pfeile bringen.

$$\begin{align}&(x+\xi_{3, 1, 1})(x+\xi_{3, 1, 2})(x+\xi_{3, 1, 3}) =\\&= x^3 + (\xi_{3, 1, 1}+\xi_{3, 1, 2}+\xi_{3, 1, 3})x^2 + (\xi_{3, 1, 1}\xi_{3, 1, 2}+\xi_{3, 1, 1}\xi_{3, 1, 3}+\xi_{3, 1, 2}\xi_{3, 1, 3})x + \xi_{3, 1, 1}\xi_{3, 1, 2}\xi_{3, 1, 3}=\\
&= x^3 +x+1\\
&\implies 1 = \xi_{3, 1, 1}\xi_{3, 1, 2}+\xi_{3, 1, 1}\xi_{3, 1, 3}+\xi_{3, 1, 2}\xi_{3, 1, 3}\text{ und }1 = \xi_{3, 1, 1}\xi_{3, 1, 2}\xi_{3, 1, 3}
\end{align}$$
oder in $\beta$ formuliert:
$$1= \beta\beta^2 + \beta\beta^4 + \beta^2\beta^4 \text{ und } \beta\beta^2\beta^4 = 1$$


## Anderes Polynom
m mal können wir einen Koeffizientenvergleich machen und erhalten:
$$1 = \xi_{3, 1, 1} + \xi_{3, 1, 2}+\xi_{3, 1, 3}\text{ und }1 = \xi_{3, 1, 1}\xi_{3, 1, 2}\xi_{3, 1, 3}$$

$$1=\beta+\beta^2$$