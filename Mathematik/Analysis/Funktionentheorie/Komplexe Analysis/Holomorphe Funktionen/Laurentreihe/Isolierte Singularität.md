## Beschreibung
Ein Punkt ist eine Isolierte Singularität, wenn Teil einer punktförmigen Definitionslücke von $f$ ist.

## Definition
Seien
- $\emptyset \neq U \subseteq \mathbb{C}$ offen
- $f: U \to \mathbb{C}$ analytisch

$a \in \mathbb{C}\backslash U$ heißt **isolierte Singularität von $f$**, wenn es ein $r> 0$ mit
$$\dot{K}(a,r) := \{z \in \mathbb{C}: 0 > |z-a| < r\} \subseteq U$$ gibt. Auf $\dot{K}(a,r)$ sei dann $f(z) = u(z) + v(z)$ Die Zerlegung der [[Laurentreihe|Laurentreihenentwicklung]] von $f$ in $a$ in Haupt- und Nebenteil.

Wir nennen dann $u(z)$ den **Hauptteil von $f$ in a** und $v(z)$ den **Nebenteil von $f$ in $a$**.

### Hebbare Singularität
Ist der Hauptteil $u(z) = 0$, so heißt a eine [[Hebbare Singularität]]
*Denn dann bleibt ja nur noch der Nebenteil übrig. Setzt man in diesen a ein, bekommt man überall 0 raus.*

### Pol
Ist $u(z)$ ein [[Polynom (Komplexe Analysis)]] in der Variablen $\frac{1}{z-a}$ vom Grad $N \geq 1$, so heißt $a$ ein [[Pol|Pol der Ordnung]] $N$.
*Die Bezeichnung kommt offensichtlich davon, dass man $a$ einen Pol n-ten Grades der Funktion $\frac{1}{(z-a)^n}$ nennt.*

### Wesentliche Singularität
Siehe [[Wesentliche Singularität]]
Ist $u \leq 0$ kein Polynom in der Variablen $\frac{1}{z-a}$, also $c_{-k}\neq 0$ für unendlich viele $k \in \mathbb{N}$, so heißt $a$ eine **wesentliche Singularität von $f$** 

### Residuum
Siehe [[Residuum]]

### Ordnung
Siehe [[Ordnung (Analysis)]]





#Mathe-IV 

[^1]: Zenk - Definition 23.1.8