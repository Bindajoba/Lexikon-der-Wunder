## Beschreibung
Um die Umlaufzahl einer einfach durchlaufenen [[Komplexe Stückweise Differenzierbare Schleife]] zu berechenen, kann man Kreise an ihrer [[Spur (Kurve)]] konstruieren und durch Vergleichen der Drehrichtung die [[Umlaufzahl]] der zusammenhängenden Mengen berechnen.

## Algorithmus
### Algorithmus nach Zenk
Sei $\gamma: [\alpha, \beta] \to \mathbb{C}$ eine [[Einfach durchlaufene Kurve|einfach durchlaufene]], [[Komplexe Stückweise Differenzierbare Schleife]] 

Nutze für den Algorithmus den [[Orientierung|positiv orientierten]] [[Kreisweg]]
$$\eta: \begin{array}{rcl} [0, 2\pi] & \to & \mathbb{C} \\ t & \mapsto & w + re{it} \end{array}$$
mit dem Radius $r>0$ und dem Mittelpunkt $w \in \mathbb{C}$

Setze den Radius und den Mittelpunkt des Kreises so, dass folgende Bedingungen erfüllt sind:
1. *Der Kreis schneidet die [[Spur (Kurve)]] von $\gamma$ an zwei verschiedenen Punkten $a$ und $b$*
Es gibt $t_1, t_2 \in [\alpha, \beta], t_1<t_2$, sodass $a:=\gamma(t_1)\in Spur(\eta), b:=\gamma(t_2)\in Spur(\eta)$ und $a\neq b$ erfüllt ist.  
2. *Der Teilweg von $\gamma$, der zwischen $a$ und $b$ liegt befindet sich in der Kreisscheibe, die von $\eta$ gezeichnet wird.*
Für $t \in ]t_1, t_2[$ gilt $\lambda(t)\in \in K(w, r)$
3. *Der Teilweg von $\gamma$, der nicht zwischen $a$ und $b$ liegt befindet sich nicht in der Kreisscheibe, die von $\eta$ gezeichnet wird.*
Für $t \in [\alpha, \beta]\backslash[t_1, t_2]$ gilt $\lambda(t)\in \in \mathbb{C}\backslash \overline{K(w, r)}$
4. *Teile die Kreisscheibe mit $\gamma$ in zwei [[Zusammenhangskompente|Zusammenhangskompenten]]*
Ist $\tilde\gamma: \begin{array}{rcl}[t_1, t_2] & \to & \mathbb{C}\\t & \mapsto & \gamma(t) \end{array}$, so hat $\overline{K(w, r)}\backslash Spur(\tilde\gamma)$ genau zwei Zusammenhangskomponenten.

Die restliche Formalisierung steht im Skript, so geht es informell weiter:
*Ist die Orientierung von $\gamma$ und $\eta$ gleich, dann erhöht sich die Umlaufszahl um 1, ist sie gegensätzlich, dann verringert sich die Umlaufzahl um 1*
[^1]


#Mathe-IV 

[^1]: Zenk - Lemma 22.2.11