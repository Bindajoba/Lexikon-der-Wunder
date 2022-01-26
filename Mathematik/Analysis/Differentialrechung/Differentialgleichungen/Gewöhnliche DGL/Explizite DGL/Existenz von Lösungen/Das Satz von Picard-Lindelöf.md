## Beschreibung
Der Satz von Picard-Lindelöf beschreibt Voraussetzungen, unter denen eine [[Explizite Differentialgleichung]] eine eindeutige Lösung hat.

## Picard-Lindelöf auf einem Streifen
Seien
- $d\in \mathbb{N}$ die Dimension der DGL
- $[a, b]$ ein [[kompaktheit|kompaktes]] Intervall mit
$a, b\in \mathbb{R}, a<b$
- $f:[a, b] \times \mathbb{K}^d \to \mathbb{K}^d$ sei stetig und [[Globale Lipschitzstetigkeit|global Lipschitzstetig]] bzgl. $x$
- Sei $(\tau, \xi) \in [a, b]\times \mathbb{K}^d$ ein Startwert

Dann hat die [[Explizite Differentialgleichung]] mit [[Startwertproblem]] 
$$x' = f(t, x), x(\tau)=\xi$$ genau eine globale Lösung $\lambda: [a, b]\to \mathbb{K}^d$ auf $[a, b]$[^1]

*Die Formulierung impliziert, dass mann bei a und b nicht unendlich einsetzen darf und deshalb die Lösung auf ganz $\mathbb{R}$ nicht eindeutig sein muss. Herr Zenk benutzt diesen Satz aber, um Eindeutigkeit auf ganz $\mathbb{R}$ zu zeigen, was mich sehr irritiert.*

## Picard-Lindelöf auf einem Zylinder
Seien
- $d\in \mathbb{N}$ die Dimension der DGL
- $(\tau, \xi) \in [a, b]\times \mathbb{K}^d$ ein Startwert
- $r_t, r_x>0$ die Höhe, bzw. Radius des Zylinders
- $[a, b]$ ein [[kompaktheit|kompaktes]] Intervall mit
$a, b\in \mathbb{R}, a<b$
- $f:Z \to \mathbb{K}^d$ sei stetig und [[Globale Lipschitzstetigkeit|global Lipschitzstetig]] bzgl. $x$ auf ${Z}$ mit Lipschitzkonstante $L$
$f$ ist definiert auf einem abgeschlossenen Zylinder $Z$ um den Startpunkt $(\tau, \xi)$ 
$$Z:=[\tau-r_t, \tau+r_t]\times \overline{K(\xi, r_x)}$$

Dann hat die [[Explizite Differentialgleichung]] mit [[Startwertproblem]] 
$$x' = f(t, x), x(\tau)=\xi$$ genau eine globale Lösung $\lambda: [a, b]\to \mathbb{K}^d$ auf $[a, b]$
auf dem, Intervall $[\tau - \beta, \tau + \beta] =: I$, wobei
- $\beta=\min\{r_t, \frac{r_x}{M}\}$    
- $M = max\{||f(t, x)||: (t, x)\in Z\}$
$M$ ist die größte Steigung, die $x'$ auf $Z$ hat.

## Picard-Lindelöf in qualitativer Fassung
Seien
- $V \subseteq \mathbb{R} \times \mathbb{K}^d$ ein [[Gebiet]]
- $f: V \to \mathbb{K}^d$ [[Lokale Lipschitzstetigkeit|lokal lipschitzstetig]] bzgl $x$
- $(t_0, x_0)\in V$ ein Startpunkt

Dann besitzt die [[Explizite Differentialgleichung]] mit [[Startwertproblem]] $$x' = f(t, x), x(t_0)=x_0$$ ein $\beta = \beta(t_0, x_0)>0$ sodass die [[Lösung]] $\lambda:[t_0-\beta, t_0+\beta] \to \mathbb{R}$ eindeutig ist.

Man sagt, es gibt eine **eindeutig bestimmte lokale Lösung**[^2]



## Beispiele
Die [[Explizite Differentialgleichung]] $$x' = x^2$$ (die Walfischpopulationen und Explosionen modelliert) ist nicht [[Globale Lipschitzstetigkeit|global lipschitzstetig]]. $x^2$ ist nicht auf ganz $\mathbb{R}$ lipsischtzstetig, daher gibt es keine Lösung auf ganz $\mathbb{R}$
Das erkennt man daran, dass die normale Lösung $\lambda(t) = \frac{1}{c-t}$ eine Polstelle bei $c$ hat und damit nicht auf alle $[a, b]$ definitiert ist.[^3]

#Mathe-IV 

[^1]: Zenk - Satz 18.3.1
[^2]: Zenk - Satz 18.3.2
[^3]: Zenk - Korollar 18.3.4