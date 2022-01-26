## Beschreibung
Eine **Beinahe-exakte Differentialgleichung** ist eine [[Implizite Differentialgleichung]] die aussieht wie eine [[Exakte Differentialgleichung]] und die sonstigen Bedingungen fast erfüllt hat aber keine Stammfunktion besitzt.

## Definition
Seien
- $U \subseteq \mathbb{R}^2$ eine [[Sternförmige Menge]]
- $f: U \to \mathbb{R}$ [[Stetigkeit|stetig]] [[Partielle Differenzierbarkeit|partiell differenzierbar]]
- $g: U \to \mathbb{R}$ [[Stetigkeit|stetig]] [[Partielle Differenzierbarkeit|partiell differenzierbar]]

aber $$f(t, x) + g(t, x)x' = 0 \tag{1}$$ nicht **exakt**.


## Lösung
Gibt es eine [[Stetig Differenzierbare Funktion|stetig differenzierbare]] Funktion $M:U \to \mathbb{R} \backslash \{0\}$, sodass
$$f(t, x)M(t, x) + g(t, x)M(t, x)x' = 0 \tag{2}$$ **exakt** ist, dann nennt man $M$ einen **integrierenden Faktor** für $(1)$[^1]

Ist $\lambda$ eine Lösung von $(2)$, dann ist es auch eine Lösung von $(1)$.

### Berechnung des integrierenden Faktors
Ist  $f(t, x) \neq 0$ für alle  $(t, x) \in U$ und es gibt eine Funktion $m$ mit
$$m(x)=h(t, x):=\frac{1}{f(t, x)}\left(\frac{\partial f}{\partial x}(t, x) - \frac{\partial g}{\partial t}(t, x)\right)\text{ für alle }(t, x) \in U$$ so definiert $M(t, x) := e^{- \int\limits_{x_0}^{x}m(s)\,ds}$ einen integrierenden Faktor für $(1)$

Ist  $f(t, x) \neq 0$ für alle  $(t, x) \in U$ und es gibt eine Funktion $m$ mit
$$m(x)=h(t, x):=\frac{1}{f(t, x)}\left(\frac{\partial f}{\partial x}(t, x) - \frac{\partial g}{\partial t}(t, x)\right)\text{ für alle }(t, x) \in U$$ so definiert $M(t, x) := e^{ \int\limits_{t_0}^{t}m(s)\,ds}$ einen integrierenden Faktor für $(1)$


### Startwertproblem
Sei $(t_0, x_0) \in U$ ein Startzustand einer **Exakten Differentialgleichung**

Gilt $g(t_0, x_0) \neq 0$, dann hat das [[Startwertproblem]] $x(t_0) = x_0$ eine lokal eindeutige Lösung $\lambda: ]t_0-\beta, t_ß + \beta[$, die sich durch Auflösen von 
$$F(t, \lambda(t)) = F(t_0, x_0)$$ bekommen lässt.

#Mathe-IV 
[^1]: Zenk - Definition 17.3.6