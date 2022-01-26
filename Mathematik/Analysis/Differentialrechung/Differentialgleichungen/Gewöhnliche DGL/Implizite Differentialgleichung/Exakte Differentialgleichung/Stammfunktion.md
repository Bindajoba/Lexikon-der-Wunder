## Beschreibung
Eine Stammfunktion ist ein Mittel zur Lösung von Exakten Differentialgleichungen.
Der [[Gradient]] der Stammfunktion im Punkt $(t, x)$ steht senkrecht zur Tangente der Lösung im Punkt $(t, x)$. Daher ist die Stammfunktion entlang jeder Lösung konstant.

Interpretiert man $t$ nicht als Zeit, sondern als Komponente des Zustands und wandelt die [[Exakte Differentialgleichung]] in eine [[Autonome Differentialgleichung]], erhält man eine [[Erhaltungsgröße]], wenn nicht sogar ([[Hamiltonfunktion]])

## Definition
Seien
- $U \subseteq \mathbb{R}^2$ ein [[Gebiet]]
- $f: U \to \mathbb{R}$ stetig
- $g: U \to \mathbb{R}$ stetig

Sei
$$f(t, x) + g(t, x)x' = 0$$ eine  [[Exakte Differentialgleichung]]

Die stetig differenzierbare Funktion $F:U \to \mathbb{R}$ mit der Eigenschaft 
$$(grad F)(t, x)= \begin{pmatrix}f(t, x) \\ g(t, x)  \end{pmatrix} \text{ für alle }(t, x)\in U \tag{1}$$
ist die **Stammfunktion** für $(1)$[^1]

#Mathe-IV 

[^1]: Zenk Definition 17.3