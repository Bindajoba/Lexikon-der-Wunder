## Beschreibung
Die Menge aller Punkte, die von dem [[Fluss]] einer [[Autonome Differentialgleichung]] durchlaufen wird, nennt man .**Trajektorie** (auch **Phasenkurve**)

Am Beispiel eines geworfennen Balls, kann man sich das als die Fluglinie vorstellen.

Dachte ich zumindest! Wandelt man die Autonome DGl in ein [[Lineares Differentialgleichungssystem erster Ordnung]] um, so ist die Trajektorie ist eigentlich die Menge allerdurchlaufenen Zustände, die während einer Physiksimulation mit fortschreitender Zeit auftaucht. D.h. eine [[Weg|Kurve]] im [[Phasenraum]].

Die Trajektorie ist ein Spezialfall einer [[Lösungskurve]], jedoch ohne Zeit.


## Definition[^1]
Sei
- $D \subseteq \mathbb{K}^d$ ein offener und zusammenhängeder Raum von [[Zustand|Zuständen]]
-  $v: D \to \mathbb{K}^d$ die lokal [[Lipschitzstetigkeit|lipschitzstetige]] rechte Seite der DGL

Eine Teilmenge $T \subset D$ heißt Trajektorie von $x'=v(x)$, wenn
$$T(\xi) = \varphi(J_\xi, \{\xi\})$$


### Positive Halbtrajektorie

DIe Trajektorie zu positiven Zeiten.
$$T^{+}(\xi) = \{\varphi(t, \xi)\in D: t \in J_\xi, t \geq 0\}$$


### Negative Halbtrajektorie
DIe Trajektorie zu negativen Zeiten.
$$T^{-}(\xi) = \{\varphi(t, \xi)\in D: t \in J_\xi, t \leq 0\}$$

### Invarianz
Eine Menge von [[Zustand|Zuständen]] heißt Invariant, wenn alle Trajektorien der in der Menge enthaltenen [[Zustand|Startzustände]] vollständig in der Menge liegen.

$M \subseteq D$ heißt invariant (bzgl. $\varphi$), wenn mit jedem $\xi \in M$ auch die Trajektorie $T(\xi) = \{\varphi(t, \xi):t\in J_\xi\}\subseteq M$ ist

Eine Menge von [[Zustand|Zuständen]] heißt positiv invariant, wenn alle Trajektorien der in der Menge enthaltenen [[Zustand|Startzustände]] vollständig in der Menge liegen.

$M \subseteq D$ heißt positiv invariant (bzgl. $\varphi$), wenn mit jedem $\xi \in M$ auch die Trajektorie $T(\xi) = \{\varphi(t, \xi):t\in J_\xi, t \geq 0\}\subseteq M$ ist

## Eigenschaften
### Zusammenhang mit Einparametrigen Gruppen
Bei [[Phase]] wurde erklärt, wie eine [[Phase]] das gleiche ist wie eine Anwendung einer [[Transformation]] $g^t$ aus einer [[Einparametrige Gruppe|Einparametrigen Gruppe]] auf einen Startwert $\xi$.

Somit ist die Punktemenge, die durch Anwednung aller [[Transformation|Transformationen]] aus $g^t$ entsteht genau die **Trajektorie** des [[Flusses]]

#Mathe-IV #Arnold 

[^1]: Zenk: Definition 20.1.9