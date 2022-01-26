## Beschreibung
Der **Satz der Variablentransformation** besagt, dass sich zu einer [[Diffeomorphismus|diffeomorphen]] Deformation der [[Lösungskurve|Integralkurven]] eine [[Explizite Differentialgleichung]] finden lässt, dessen Lösungen genau diese deformierten [[Lösungskurve|Integralkurven]] sind. 

## Definition
Seien
- $J \subseteq I \subseteq \mathbb{R}$ Intervalle
$I$ ist das Intervall, auf der eine Lösung definiert sein könnte
$J$ ist die Definitionsmenge der Lösung
- $V \subseteq I\times \mathbb{K}^d$ ein [[Gebiet]]

Sei für alle $t \in I$: $V_t:=\{x \in \mathbb{K}^d: (t, x) \in V\}$
$V_t$ beschreibt alle möglichen Zustände, die zum Zeitpunkt $t$ möglich sind.
*Man kann es sich so vorstellen, dass $V_t$ ein [[Phasenraum]] ist. Die Phasenräume verändern sich aber im Laufe der Zeit.*

Sei $\varphi \in C^1(V, \mathbb{K}^d)$ derart, dass für für jedes $t\in$ die Abbildung
$$\varphi_t:=\varphi(t, \cdot): \begin{array}{rcl} V_t & \to & \varphi(t, V_t) \\ x & \mapsto & \varphi(t,y) \end{array}$$ ein $C^1$-Diffeomorphismus ist. 
*$\varphi$ ist also eine Funktion die in Abhängigkeit vom aktuellen Zeitpunkt die Punkte des aktuellen Phasenraums $V_t$ verzerrt. *

Sei noch $\lambda: J \to \mathbb{K}^d$ eine Funktion, dann ist äquivalent:
1. $\lambda: J \to \mathbb{K}^d$  ist eine Lösung von $$x' = f(t,x)$$
2. $\mu: \begin{array}{rcl} & \to & \mathbb{R}^d \\ t & \mapsto & \varphi(t, \lambda(t)) \end{array}$ ist eine Lösung von $$y'= [D\varphi_t^{-1}(y)]^{-1}f(t, \varphi_t^{-1}(y)) + \frac{\partial \varphi}{\partial t}(t, \varphi_t^{-1}(y))$$[^1]

*Der Satz ist vielleicht etwas unintuitiv. Ich denke, der braucht noch ein Beispiel.* 

## Beispiel I
Sei $d=1$,, d.h. Die Dimension der DGL 1.
Versuchen wir als $\varphi$ zu visualisieren.
Was bedeutet es, dass die Diffeomorphe Funktion $$\varphi$$ den Phasenraum deformiert?
Und was ist $\varphi_t$?

Betrachte zum Beispiel die Funktion $\varphi(t, x) = 2x$.
Dann ist $\varphi_t(x) = \varphi(t, x) = 2x$

Der Punkt $1$ wird also von $\varphi_t(x)$ auf $a$ abgebildet. 

Um darzustellen, wie sich alle Punkte unter $\varphi_t$ für alle $t$ verändern, wählen wir folgende Visualisierung:

![[Pasted image 20210603164324.png]]

Der rote Punkt zeigt die Abbildung von $x=1$ auf $x=2$ durch Anwendung von $\varphi_t$ zum Zeitpunkt $t$.

Statt einzelne Punkt zu betrachten, kann man auch ansehen was für jede vertikale Linei $V_t$ passiert, wenn man $\varphi_t$ anwendet: Er wird um das doppelte gestreckt. Da wird durch die grauen Linien repräsentiert, die jetzt doppelt so weit von der Abzisse entfernt sind wie vorher. 

Die $t$-Achse ist auf der rechten Seite theoretisch nicht nötig, wir behalten sie aber bei, da man damit einen interessanten Sachverhalt beobachten kann.
Eine Gerade (z.B. grün/blau) bleibt nach Anwendung von $\varphi_t$ im Bild eine Gerade. Insbesondere ist sie doppelt so steil.
Das wird später wichtig.

Sei jetzt $x' = f(t, x)$ eine [[Explizite Differentialgleichung]].
Die Gleichung oben bedeutet, dass man die Steigung eines Graphen im Punkt $(t, x)$ kennt.
Das kann man exemplarisch in einer Skizze festhalten

![[Pasted image 20210603165408.png]]

Auf diese Skizze könnten wir jetzt wieder $\varphi_t(x) = 2x$ anwenden. 
Was dann passiert ist sehr interessant. Die Steigung in jedem Punkt verdoppelt sich.

Das liegt daran, dass ein Lösung $\lambda$, tangential durch die eingezeichneten Linien verlaufen muss. Jede Lösung lässt in einem Punkt du eine Tangente annähern, die dann die Steigung $x' = f(t, x)$ haben muss. Wir haben aber bereits gezeigt, dass alle Geraden doppelt so steil sind. 

usw.

## Spezialfall I
Es sei $\alpha, \beta, \gamma \in \mathbb{R}, \beta>0$ und $g: \mathbb{R} \to \mathbb{R}$ stetig.
Erzeuge damit eine [[Explizite Differentialgleichung]] der Form
$$x' = g(\alpha t + \beta x + \gamma)\tag{1}$$

Wähle $\varphi(t, x) = \alpha t + \beta x + \gamma$
oder kurz: $y = \alpha t + \beta x + \gamma$

Dann ist $\lambda: J \to \mathbb{K}^d$  genau dann eine Lösung von $(1)$, wenn
$\mu: \begin{array}{rcl} \mathbb{R} & \to & \mathbb{R}^d \\ t & \mapsto & \varphi(t, \lambda(t)) \end{array}$ ist eine Lösung von $$y'= \alpha+\beta g(y)$$ ist[^2]

## Spezialfall II
Sei 
- $U \in \mathbb{R}\times \mathbb{R}$ eine [[Offene Menge|Offene]] Menge 
- $f: U  \to \mathbb{R}$ eine Funktion

Gelte zudem: 
- $U \cup \{(0, x): x \in \mathbb{R}\} = \emptyset$ 
*D.h. die Gleichung ist nicht für den Zeitpunkt 0 definitiert.* **und** 
- $f(\sigma t, \sigma x) = f(t, x)$ für alle $(t, x) \in U$ und alle $\sigma \in \mathbb{R}\backslash \{0\}$

Definiere die [[Explizite Differentialgleichung]] 
$$x' = f(t, x) \tag{2}$$

Wähle $\varphi(t, x) = \frac{x}{t}$
oder kurz: $y = \frac{x}{t}$

Dann wird $(2)$ in $$y' = \frac{f(1, y)-y}{t}$$ überführt. Die Gleichung kann dann leicht mit [[Trennen der Variablen]] gelöst werden

*Sehen die Lösungen oder der Phasenraum einer Differentialgleichung so aus, als würden sie sich in geraden vom Mittelpunkt weg oder hin bewegen, könnte diese Beispiel nützlich werden. *[^3]

## Spezialfall Bernoulli Differentialgleichung
Sei 
- $I \in \mathbb{R}$ ein Intervall
- $\alpha \in \mathbb{R}\backslash \{0,1\}$
- $a, b \in C(I, \mathbb(I, \mathbb{R}))$

Eine [[Explizite Differentialgleichung]] 
$$x' = a(t)x(t) * b(t)x^\alpha \tag{2}$$ wir durch $\varphi(t, x) = x^{1-\alpha}$ oder kurz: $y = x^{1-\alpha}$ in
$$y' = (1-\alpha)(a(t)y+b(t))$$ übergeführt.
Diese Gleichung ist eine [[Skalare Lineare Differentialgleichung erster Ordnung]] und kann leicht gelöst werden. [^4]

#Mathe-IV 

[^1]: Zenk - Satz 17.2.7
[^2]: Zenk - Beispiel 17.2.8
[^3]: Zenk - Beispiel 17.2.9 
[^4]: Zenk - Beispiel 17.2.10