# Skalare Lineare Differentialgleichung erster Ordnung
## Beschreibung
Eine **Skalare Lineare Differentialgleichung erster Ordnung** so ziemlich die einfachste Differentialgleichung.
Es handelt sich um ein **1-dimensionale [[Reelles Lineares Differentialgleichungssystem]] erster Ordnung**.
Daher ist die **Skalare Lineare Differentialgleichung erster Ordnung** ein Spezialfall von:
- [[Skalare lineare Differentialgleichung]] aber nur von erster Ordnung
- [[Lineares Differentialgleichungssystem erster Ordnung]] aber 1-Dimensional 


*Ein Skalar ist eine Zahl die kein Vektor ist. Die DGL ist eindimensnional, daher nennt man sie Skalar*

# Skalare Lineare Homogene Differentialgleichung erster Ordnung
## Definition
Seien
- $I \subseteq \mathbb{R}$
*$I$ ist der Definitionsbereich von $a$*
- $k \in \mathbb{N}$
*$k$ ist die Ordnung der DGL* 
- $a_i\in C(I, \mathbb{R})$ eine [[Stetigkeit|Stetige Funktion]] für $i \in \{0, ..., k-1\}$[^1]
 
 EIne **1-Dimensionale Lineare Homogene Differentialgleichung k-ter Ordnung** hat die Form
 $$x' = a_0^{(k-1)}(t)x_{k-1} a_1(t)x' + a_0(t)x$$


## Lösung der 1-ten Ordnung
Für die Lineare Homogene Differentialgleichung erster Ordnung
$$x' = a(t)x$$ zum [[Startwertproblem]] $x(t_0)=x_0$ **existiert**
- eine globale Lösung
$$\lambda(t) = x_0e^{\int\limits_{t_0}^ta(\tau) \, d\tau}$$ Die Lösung ergibt sich aus dem [[Trennen der Variablen|Satz zum Trennen der Variablen]][^1]

*Die Lösung muss also nicht eindeutig sein (glaube ich)*


[^1]: Zenk - Beispiel 17.2.4

# Skalare Lineare Inhomogene Differentialgleichung erster Ordnung
## Definition
Seien
- $I \subseteq \mathbb{R}$
*$I$ ist der Definitionsbereich von $a_i$ und $g$*
- $k \in \mathbb{N}$
*$k$ ist die Ordnung der DGL* 
- $a_i\in C(I, \mathbb{R})$ eine [[Stetigkeit|Stetige Funktion]] für $i \in \{0, ..., k-1\}$
- $g\in C(I, \mathbb{R})$ eine [[Stetigkeit|Stetige Funktion]][^1]
 
 EIne **Lineare Homogene Differentialgleichung k-ter Ordnung** hat die Form
 $$x' = a_0^{(k-1)}(t)x_{k-1} a_1(t)x' + a_0(t)x + g(t)$$[^1]


## Lösung der 1-ten Ordnung
Für die Lineare Homogene Differentialgleichung erster Ordnung
$$x' = a(t)x$$ zum [[Startwertproblem]] $x(t_0)=x_0$ **existiert**
- eine auf $I$ globale Lösung
$$\lambda(t) = x_0e^{\int\limits_{t_0}^ta(s) \, ds} + e^{\int\limits_{t_0}^ta(s) \, ds} \int\limits_{t_0}^t e^{\int\limits_{t_0}^ta(r) \, dr}b(s)\,ds$$ Die Lösung ergibt sich aus der [[Variation der Konstanten]] und ist eindeutig[^1]

#Mathe-IV 

[^1]: Zenk - Beispiel 17.2.6

