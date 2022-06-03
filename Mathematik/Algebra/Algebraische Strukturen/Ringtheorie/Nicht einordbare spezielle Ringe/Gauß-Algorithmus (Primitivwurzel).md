TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Der Gauß-Algorithmus ist ein Algorithmus um eine [[Primitivwurzel]] einer [[Prime Restklassengruppe]] zu erhalten.

# Algorithmus
Sei $K^\times$ eine Prime Restklassengruppe der Ordnung $q-1$:

Der Gauß-Algorithmus läuft in $4$ Schritten ab:
1. Beginne mit $i = 1$. Sei $\alpha_i$ ein beliebiges Element der Primen Restklassegruppe
Berechne $ord(\alpha_1) = t_1$
2. Wenn $t_i = q-1$, dann ist $\alpha_i$ schon ein Erzeuger von $K^\times$, also [[Primitivwurzel]]
3. Wähle ein Element $\beta$, welches keine Potenz von $\alpha_i$ ist. und berechne $s = ord(\beta)$
Wenn $s = q-1$, setze $\alpha_{i+1} = \beta$. $\alpha_{i+1}$ ist eine Primitivwurzel
4. Suche $d \mid t_1$ und $e \mid s$ mit $ggT(d, e) = 1$ und $d \cdot e = kgV(t_i, s)$
5. Sei $\alpha_{i+1} = \alpha_i^{t_i/d}\beta^{s/e}$, dann gilt $t_{i+1} = ord(\alpha_{i+1}) = kgV(t_i, s)$
Erhöhe $i$ um $1$ und wiederhole ab $2$.

## Erklärung Schritt 3
Wir suchen ein Element $\beta$. Im 4. Schritt wollen wir ein Element $\alpha_{i+1}$ berechnen, welches $\alpha_1$ und $\beta$ durch Potenzieren erzeugt.
Die Ordnung $s$ des neuen Elements $\beta$ kann kein Teiler von $t_i$ sein, da $\beta$ sonst in der von $\alpha_i$ erzeugten Untergruppe läge.

## Erklärung Schritt 4
Die Existenz eines solchen $d, e$ ist nicht auf den ersten Blick offensichtlich.
Durch ein Beispiel lässt sich die Methode, mit der man zwei solche Elemente findet leicht illustrieren:
$t_i = 12, s=18$.
Wir wollen ein $d,e$ finden, sodass $d \mid t_i, e \mid s, ggT(d,e) = 1$ und $d\cdot e = kgV(t_i, s)$
Nehmen wir für $d, e$ einfach $t_1, s$ selbst, dann sind die ersten beiden Anforderungen erfüllt. Will man noch die dritte Erfüllen, können wir so lang Faktoren aus $d, e$ entfernen, bis sie teilerfremd sind, also $ggT(d, e) = 1$ erfüllen.
Entfernen wir alle Faktoren aus $12$. Wir müssten alle Teiler $2, 3$ entfernen da diese auch in $18$ liegen.
Wir erhalten $d = 1, e = 18$, was zar $ggT(d, e) = 1$ erfüllt aber nicht $d\cdot e = 18 = kgV(t_1, s) = 36$
Klar, wir haben auch die letzte Bedingung nicht berücksitigt. 

Wie können wir Faktoren aus $12, 18$ entfernen, sodass wir die letzte Bedingung berücksichtigen?
Für den [[Kleinstes Gemeinsames Vielfaches|kgV]] zweier Zahlen gilt die folgende Regel $t_is = ggT(t_i, s)kgV(t_i, s) \implies kgV(t_i, s) = \frac{t_i, s}{ggT(t_i, s)}$
Wir dürfen nicht einfach beliebig viele Faktoren aus der ersten Zahl entfernen. Wir müssen immer so viele Faktoren entfernen wie $t_i$ und $s$ gemein sind. Damit die beiden Zahlen aber teilerfremd werden ist es notwendig, dass wir die gemeinsamen Faktoren aus der Zahl entfernen, die weniger dieses Faktors hat. So teilen sich die Zahlen $d, e$ keine gemeinsamen Faktoren, d.h. $ggT(d, e) = 1$ und wir sind haben die Faktoren so entfernt, dass $de = kgV(t_i, s)$.
Führen wir die Idee auf $12, 18$ durch:
$t_i = 12 = 2^2*3, s = 18 = 2*3^2$
Wir entfernen die gemeinsame $2^1$ aus $18$ und die gemeinsame $3^1$ aus $12$ und erhalten $d = 4, e = 9$.
Es gilt $ggT(d, e) = 1$ und $4\cdot 9  = 36 = kgV(t_i,s)$

## Erklärung Schritt 5
Warum gilt für $\alpha_{i+1} = \alpha_i^{t_i/d}\beta^{s/e}$, $t_{i+1} = ord(\alpha_{i+1}) = kgV(t_i, s)$?
Nach den Rechenregeln für [[Ordnung (Gruppe)]] gilt:

Für ein $\alpha$ mit $ord(\alpha) = t \implies ord(\alpha^i) = \frac{t}{ggT(t, i)}$

Auf unseren Fall angewendet: $ord(\alpha_i) = t_i \implies ord(\alpha_1^{t_i/d}) = \frac{t_i}{ggT(t_i, t_i/d)} = \frac{t_i}{t_i/d} = d$
Und analog $ord(\beta^{s/e}) = e$
Da $d, e$ teilerfremd sind gilt $ord(\alpha_1^{t_1/d}\beta^{s/e}) = ed$ (Siehe dazu [[Ordnung (Gruppe)]])


# Übungen
## McEliece Übung 3-5
Betriachte den Körper $\F_{73}$

### a)
Was ist $ord(2), ord(3)$?
$|\F_{73}^\times| = 72 = 2*36 = 2^3*3^2$. Die Ordnung muss also $1, 2, 3, 4, 6, 8, 12, 18 , 24, 36, 72$ sein.
- $2^2 = 4$
- $2^4 = 16$
- $2^8 = 256 = 37$
- $2^3 = 8$
- $2^9 = 512 = 1$

Die Ordnung muss $9$ oder ein Teiler davon sein. Alle Teiler im Exponenten ergeben aber nicht $1$, d.h. $ord(2) = 9$

Damit muss $2^{72} = 1$
- $3^2 = 9$
- $3^4 = 81 = 8$
- $3^6 = 72$
- $3^8 = 64$
- $3^3 = 27$
- $3^9 = 46$
- $3^{12} = 1$

$ord(3)$ ist $12$ oder Teiler. Die Teiler sind es aber nicht.

### b)
Finde ein Element $a$ mit $ord(a) = kgV(12, 9) = 36$.
$d = 4, e= 9$.
Dann ist $\alpha_2 = 2^3*3^1 = 24$ mit $ord(24) = kgV(12, 9) = 36$

## c)
Was ist die kleinste Zahl in $\{1, 2, 3, ..., 72\}$ welche keine Potenz von $24$ ist?
- $1$ ist immer Potenz
- $2$ ist Potenz da $9 \mid 36$
- $3$ ist Potenz
- $4^9 = 2^92^9 = 1$, ist also Potenz, da $9 \mid 36$
- $5^3 = 125 = 52$
- $5^9 = 10$
- $5^{18} = 100 = 27$
- $(5^{18})^2 = 5^{36} = 72 \neq 1$ ($5$ kann also keine Potenz von $24$ sein, denn sonst müsste das hier $1$ ergeben. $5$ kann nur Ordnung 24 oder 72 haben)
- $5^{24} = 5^{18}5^6 =27*3 = 6 \neq 1$
- $(5^{18})^4 = 27^4 = 3^{72} = 1$

### d)
Was ist $\sqrt[30]{64}$ und $\sqrt[30]{59}$.
$5$ ist eine [[Primitivwurzel]].

Suche $y$, sodass $64 = 5^y$.
- $5^2 = 25$
- $5^4 = 41$
- $5^8 = 2$
- $(5^8)^6 = 5^{48} = 64$

Suche $x$, sodass $30x = 48 \mod 72$.
Benutze den [[Euklidischer Algorithmus|euklidischen Algorithmus]], um eine sinnvolle Linearkombination zu finden.

| $t_i$ | $s_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 72    |       |
| 0     | 1     | 30    |       |
| 1     | -2    | 12    | 2     |
| -2    | 5     | 6     | 2     |


Damit gilt $72-2*30 = 12$.
In Folge $-2*30 = 12$ und damit $4*(-2)*30 = 4*12 = 48$

$30x = 48 \mod 72 \iff 30x + 72y = 48$.
Das rechte ist ein lineares Gleichungssystem. Die Lösungspunkte sind eine Gerade mit der Gleichung
$(5^{16})^{30} = 5^{48}$

$$y = -\frac{30}{72}x+\frac{48}{72} = -\frac{5}{12}x+\frac{8}{12}$$
Der Punkt $(-8, 4)$ ist ein Punkt auf der Gerade.
Die Gerade hat die Steigung $-\frac{5}{12}$. Die Anderen Ganzzahligen Punkte sind damit
$\{(-8 +12n, 4 - 5n): n \in \Z\}$
Also:
- $(-8, 4)$
- $(4, -1)$
- $(16, -6)$
- $(28, -11)$
- $(40, -16)$
- $(52, -21)$
- $(64 = -8, -26)$

Es gilt 
- $4*30 = 48$
- $16*30 = 48$
- $28*30 = 48$
- $40*30 = 48$
- $52*30 = 48$
- $64*30 = 48$

Das heißt 
$$\begin{align}5^{48} &= (5^{64})^{30} = 37^{30} \\
&= (5^{4})^{30} = 41^{30}\\
&= (5^{16})^{30} = 4^{30} \\
&= (5^{28})^{30} = 36^{30} \\
&= (5^{40})^{30} = 32^{30}\\
&= (5^{52})^{30}= 69^{30}\end{align}$$

Suche $y$, sodass $59 = 5^y$
$59$ ist eine Primzahl. Es gibt also keine billigen Tricks, um an Faktoren heranzukommen.
- $59^2 = 50$
- $59^4 = 18$
- $59^8 = 32 = (5^8)^5 = 5^{40}$
- $59 =5^5$ 

Suche $x$, sodass $30x = 5 \mod 72$.
Eine solche Zahl gibt es nicht. Für alle $x$ ist $30x$ gerade. Insbesondere ist $30x\mod 72$ gerade und kann niemals kongruent zu $5$ sein.




$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#McEliece 

