## Definition
Seien
- $I, U \subseteq \mathbb{R}$
$I$ ist der Definitionsbereich der von $t$ abhängigen Funktion $g$
$U$ ist der Definitionsbereich der von $x$ abhängigen Funktion $f$
- $t_0 \in I$, $x_0 \in I$ der Startzustand
- $f \in C(I, \mathbb{R})$ ein [[Diffeomorphismus]] 
- $g \in C(U, \mathbb{R})$ ein [[Diffeomorphismus]] 

Hat eine [[Explizite Differentialgleichung]] die Form: 

$$x' = \frac{f(x)}{g(t)} \tag{1}$$ und das [[Startwertproblem]] $x(t_0) = x_0$
Dann hat die Differentialgleichung
1. im Fall $h(x_0)=0$ mindestens eine [[Lösung]], nämlich $\lambda: \begin{array}{rcl}: I & \to & \mathbb{R} \\ t & \mapsto & x_0 \end{array}$
2. im Fall $h(x_0) \neq 0$ lokal eine eindeutige Lösung:
D.h. Es gibt ein offenes Intervall $I' \subseteq I$ mit $t_0 \in I'$, sodass $(1)$ genau eine Lösung besitzt. 
$\lambda$ bestimmt sich aus
$$ \int\limits^{\lambda}_{x_0}\frac{1}{g(\tau)} \,d\tau = \int\limits^{t}_{t_0}\frac{1}{f(\xi)} \,d\xi$$ *Hier erkennt man das die Lösung für $f(t), g(t) = 0$ nicht definiert ist. Daher darf das Intervall $I'$ keine Nullstellen enthalten. [^1]*

*Der Grund, warum der zweite Fall nicht eindeutig ist, ist dass im Fall $x' = 0$ Lösungskurven sich aufteilen können. (Das ist sehr komisch aber im Beispiel genauer erläutert.)
Aus dem gleichen Grund, ist im ersten Fall die Lösung nur auf einer Umgebung eindeutig, in der $x'(t) \neq 0$ für $t \in I'$ .*[^2]

**Obacht**: DIe Lösung, die man oben herausbekommt, ist nur auf dem Intervall $I'$ definiert. Da wir durch Trennen der Variablen nicht erfahren, was das Intervall $I'$ ist, müssen wir die Lösung nochmal überprüfen.

Sind $f$ und $g$ [[Glatte Funktion|glatte Funktionen]], dann ist im ersten Fall $h(x_0)=0$ die Lösung sogar eindeutig. (Siehe [[Das Satz von Picard-Lindelöf]])

## Herleitung für glatte Funktionen
Seien
- $I, U \subseteq \mathbb{R}$
$I$ ist der Definitionsbereich der von $x$ abhängigen Funktion $g$
$U$ ist der Definitionsbereich der von $y$ abhängigen Funktion $f$
- $t_0 \in I$, $x_0 \in I$ der Startzustand
- $f: I \to \mathbb{R}$ ist [[Glatte Funktion|glatt]]
- $f: U \to \mathbb{R}$ ist [[Glatte Funktion|glatt]]

DIe [[Phasenkurven]] der Lösung der [[Explizite Differentialgleichung]] 
$$x' = \frac{f(x)}{g(t)}$$ sind genau die [[Integralkurven]] von
$$x'(t) = g(x(t)), x'(t) = f(y(t))\tag{2}$$[^1]

Durch Lösung von $(2)$ ergibt sich eine Schreibweise, die Gleichung unabhängig von $t$ zu beschreiben. Diese Schreibweise ist genau $(1)$[^2]

## Beispiele
Die [[Autonome Differentialgleichung]] $x' = x^{2/3}$ hat zum [[Startwertproblem]] $x(0)=0$ auf jedem Intervall $I' \subseteq I$ mit $t_0 \in I'$ die beiden maximalen Lösungen $\lambda_1(t)=0$ und $\lambda_2(t)=(t/3)^3$.
Das liegt daran, dass $x^{2/3}$ bei $0$ eine unendlich große Steigung hat.

#Mathe-IV
#Arnold


[^1]: Arnold - Kapitel 1 §6 Satz
[^2]: Zenk - Satz 17.2.2