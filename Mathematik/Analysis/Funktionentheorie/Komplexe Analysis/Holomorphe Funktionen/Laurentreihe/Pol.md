## Definition
Eine [[Isolierte Singularität]] $a$ heißt ein **Pol der Ordnung $N$** von der [[Analytische Funktion|analytischen Funktion]] $f$, wenn der [[Isolierte Singularität|Hauptteil]] von $f$ in $a$ ein [[Polynom (Komplexe Analysis)]] in der Variablen $\frac{1}{z-a}$ vom Grad $N \geq 1$ ist.
*Die Bezeichnung kommt offensichtlich davon, dass man $a$ einen Pol n-ten Grades der Funktion $\frac{1}{(z-a)^n}$ nennt.*

## Eigenschaften
### Charakterisierung Pol
Sei 
- $U \subset U, a\in U$
- $f: U \backslash \{a\} \mathbb{C}$ analytisch.

$a$ ist genau dann ein Pol, wenn $\underset{z\in U}{\underset{z \to a}{\lim}}|f(z)| = \infty$ für alle Folgen die gegen $a$ gehen


### Charakterisisrung Pol m-ter Ordnung
Sei 
- $U \subset U, a\in U$
- $f: U \backslash \{a\} \to \mathbb{C}$ analytisch.

$a$ ist genau dann ein **Pol m-ter Ordnung**, wenn 
- Es gibt eine analytische Funktion $g: U \to \mathbb{C}$ mit $g(a) \neq 0$, sodass
$$f(z) = (z-a)^{-m}g(z)$$ für alle $z \in U \backslash \{a\}$ erfüllt ist.
*Diese Äquivalenz ist ziemlich offensichtlich, wie mir gerade auffällt. Der Hauptteil von $f$ ist endlich lang, daher müsste man einfach das $\frac{1}{z-a}$ ausklammern können.*[^1] ODER
- Es gibt eine Umgebung $V \subseteq U$ von $a$ und $c, C \in ]0, \infty[$, sodass
$$c|z-a|^{-m} \leq |f(z)| \leq C|z-a|^{-m}$$ für alle $z \in U \backslash \{a\}$ erfüllt ist. 
*Das erinnert mich sehr an die [[Polynom (Komplexe Analysis)#Abschätzung|Abschätzung eines Polynoms]]* ODER
- Für $k \in \{0, 1, ..., m-1\}$ ist
$$\underset{z\in U \backslash \{a\}}{\underset{z \to a}{|(z-a)^kf(z)|}} = \infty$$ und 
$$\underset{z\in U \backslash \{a\}}{\underset{z \to a}{|(z-a)^mf(z)|}} \in \mathbb{C}$$ existert
- Die [[Ordnung (Analysis)]] von $f$ ist $-m$:
$\omega(f, a) = -m$ [^2]

### Charakterisierung Pol erster Ordnung
Sei
- $U \subseteq \mathbb{C}$ offen
- $g: U  \to \mathbb{C}$, $h: U  \to \mathbb{C}$ 
- $a \in U$

mit 
- $h(a) = 0$
- $g(a) \neq 0$
- $h(z) \neq 0$ für $z \in U \backslash \{a\}$
- $h'(a) \neq 0$

Dann ist $a$ ein Pol 1.Ordnung von $\frac{g(z)}{h(z)}$ und $Res(\frac{g}{h}, a) = \frac{g(a)}{h'(a)}$


#Mathe-IV 

[^1]: Zenk - Satz 23.1.10 
[^2]: Zenk - Lemma 23.1.15