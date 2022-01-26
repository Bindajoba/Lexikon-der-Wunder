## Definition
Seien
- $\emptyset \neq U \subseteq \mathbb{C}$ [[Offene Menge|offen]]
- $f: U \to \mathbb{C}$ [[Analytische Funktion|analytisch]]

Sei $a$ eine [[Isolierte Singularität]].
Der erste Koeffizient $c_{-1}$ des **Hauptteils von $f$ in a** heißt das **Residuum von $f$ im Punkt $a$** (Notiert: $Res(f, a)$).

## Eigenschaften
### Eigenschaft 1
Ist $a \in U$ ein [[Pol|Pol 1. Ordnung]] von $f: U \backslash \{a\} \to \mathbb{C}$, dann ist
$$Res(f, a)= \underset{z\in U \backslash \{a\}}{\underset{z \to a}{\lim}}{(z-a)f(z)}$$[^1]

### Eigenschaft 2
Ist $\emptyset \neq U \subseteq \mathbb{C}$ offen, $a \in U$ ein [[Pol]] m-ter Ordnung von $f: U \backslash \{a\} \to \mathbb{C}$ und $G: U \to \mathbb{C}$ die analytische Fortsetzung von $f: \begin{array}{rcl}U \backslash \{a\} &\to &\mathbb{C} \\ z & \mapsto & (z-a)^mf(z) \end{array}$, dann gilt:
$$Res(f, a) = \frac{1}{(m-1)!}G^{(m-1)}(a)$$



#Mathe-IV 

[^1]: Zenk - Lemma 23.1.16