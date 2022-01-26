## Beschreibung
Eine autonome DGL ist eine [[Gewöhnliche Differentialgleichung]], bei der die Änderung der Phase nicht von der Zeit abhängig ist.

## Definition
Sei
- $D \subseteq \mathbb{K}^d$ ein offener und zusammenhängeder Raum von [[Zustand|Zuständen]]
-  $v: D \to \mathbb{K}^d$

Eine DGL der Form
$$x' = v(x) \tag{1}$$
heißt autonom.

*Merke, das das DGL hier ein [[Lineares Differentialgleichungssystem erster Ordnung]] ist. In Arnold war das nicht zwingend notwendig, solange die DGL zeitunabhängig ist.


## Lösung
### Nulllösungen
Eine Lösung der autonomen DGL $(1)$ ist genau dann konstant mit dem Wert $c \in \mathbb{K}^d$, wenn $g(c) = 0$ 
### Zeitliche Invarianz
Ist $\lambda(t)$ eine Lösung von $(1)$ dann ist auch $\lambda(t + a)$ eine Lösung von $(1)$

## Stabilität um Ruhelagen
Sei $v: D \to \mathbb{K}^d$ differenzierbar und $v(\xi)=0$ eine [[Ruhelage]]
Berechne die Jacobimatrix $(Dg)(xi)$ und dessen [[Eigenwert|Eigenwerte]] $\mu_1, ..., \mu_k$
- Ist $Re \mu_j < 0$ für alle Eigenwerte, dann ist $\xi$ eine [[Asymptotische Stabilität|asymptotisch stabile]] [[Ruhelage]] von $(1)$ 
- Ist $Re \mu_j > 0$ für einen Eigenwert, dann ist $\xi$ eine [[Stabilität|instabile]] [[Ruhelage]] von $(1)$ 

*Die Idee ist, dass sich die [[Phasengeschwindigkeit|Phasengeschwindigkeiten]] einer Umgebung einer Ruhelage durch eine lineare Abbildung, die gerade die Ableitung in $\xi$ ist approximieren lässt. 
Somit lässt sich das Problem auf die Überprüfung der Stabilität eines [[Lineares Differentialgleichungssystem erster Ordnung]] reduzieren.*

#Mathe-IV 