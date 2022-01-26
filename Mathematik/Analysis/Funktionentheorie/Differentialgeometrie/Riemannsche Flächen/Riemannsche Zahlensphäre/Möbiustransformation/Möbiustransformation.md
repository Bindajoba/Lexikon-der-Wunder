## Beschreibung
Die Möbiustransformation ist die Operation, dass man eine [[Riemannsche Zahlensphäre|Riemannsche Sphäre]] auf eine Sphäre [[Stereographische Projektion|projeziiert]], die Sphäre dreht und dann wieder zurück auf eine Ebene projeziiert.

## Definition
### Definition Zenk
Sind $a, b, c, d \in \mathbb{C}$ mit $ad - bc \neq 0$, so heißt für $c \neq 0$ die [[Abbildung]]
$$\varphi_{a, b, c, d}: \begin{array}{rcl} \hat{\mathbb{C}} & \to & \hat{\mathbb{C}} \\ z & \mapsto & \begin{cases} \frac{az+b}{cz+d} & \text{für } z \in \mathbb{C} \backslash \{-\frac{d}{c}\} \\ \infty & \text{für } z = -\frac{d}{c} \\ \frac{a}{c} & \text{für } z = \infty \end{cases} \end{array}$$ bzw. für $c = 0$
$$\varphi_{a, b, c, d}: \begin{array}{rcl} \hat{\mathbb{C}} & \to & \hat{\mathbb{C}} \\ z & \mapsto & \begin{cases} \frac{az+b}{d} & \text{für } z \in \mathbb{C} \\ \infty & \text{für } z = \infty \end{cases} \end{array}$$

*Allem Anschein nach, wird die Zahlensphäre bei $c=0$ nur um den Nordpol rotiert.*

Ich habe auf One-Note einige Tests gemacht.
$a$ beschreibt eine Skalierung/Drehung um einen Mittelpunkt
$b$ beschreibt die Verschiebung des Nullpunkts
$c$ beschreibt die Verschiebung des Unendlichkeitspunkts
$d$ beschreibt eine Skalierung/Drehung um einen Mittelpunkt nach der Verschiebung

### Definition Needham
Sind $a, b, c, d \in \mathbb{C}$, so heißt die [[Abbildung]]
$$\varphi_{a, b, c, d}: \begin{array}{rcl} \hat{\mathbb{C}} & \to & \hat{\mathbb{C}} \\ z & \mapsto & \frac{az+b}{cz+d}\end{array}$$ eine Möbiustransformation. (wobei Rechenregeln der [[Riemannsche Zahlensphäre]] berücksichtigt werden: z.B.: $\frac{a}{0} = \infty$ oder $\frac{a}{\infty} = 0$)

*Man sieht sehr gut, dass die Definition von Needham etwas simpler ist.*

### Singuläre Möbiustransformation
Erfüllen die Paramater einer Möbiustransformation die Gleichung $ad-bc = 0$, dann bilden alle Punkte auf den Punkt $\frac{a}{c}$ ab.
In dem Fall nennt man die Möbiustransformation **singulär**.

*Nach Zenk, ist das nicht mal eine Möbiustransformation.*

### Nicht-singuläre Möbiustransformation
Erfüllen die Paramater einer Möbiustransformation die Gleichung $ad-bc \neq 0$, dann bilden alle Punkte nicht auf einen einzigen Punkt ab.
Die Möbiustransformation heißt deshalb **nicht-singulär**.

### Normalisierte Möbiustransformation
Siehe [[Normalisierte Möbiustransformation]]

### Rotation
Hat die Möbiustransformation die Form
$$z \mapsto \frac{az + b}{ -\overline{b}z + \overline{a}}$$
dann beschreibt die Möbiustransformation eine Rotation der [[Riemannsche Zahlensphäre]]. 
Man erkennt gut, dass die Transformationen einen maximal zweidimensionalen Raum bilden. 

Die Rotationen bilden natürlich ebenfalls eine Gruppe[^6]



## Eigenschaften
### Zerlegung
Eine Möbiustransformation kann als eine Hintereinanderausführung folgender Funktionen betrachtet werden:
- [[Translation]] $z \mapsto z + \frac{d}{c}$
- $z \mapsto \frac{1}{z}$
- Streckung und Drehung $z \mapsto -\frac{(ad-bc)}{c^2}z$
- Translation $z \mapsto \frac{a}{c}$[^7]


### Erhaltung von Kreislinien
**Nicht-singuläre Möbiustransformationen** bilden [[Verallgemeinerte Kreislinie|verallgemeinerte Kreislinien]] – also Kreislinien und Geraden (einschließlich $\infty$) – auf verallgemeinerte Kreislinien ab.[^2]

Man kann zeigen, dass **Möbiustransformationen**  die einzigen komplexen Funktionen mit dieser Eigenschaft sind.[^8]


### Gruppeneigenschaft
Die Menge $\mathcal{M}:= \{\varphi: \hat{\mathbb{C}} \to \hat{\mathbb{C}}: \varphi \text{ nicht-singuläre Möbiustransformation}\}$ aller nicht-singulären Möbiustransformationen bildet mit der Verknüpfung eine [[Gruppe]]:
- Jede nicht-singuläre Möbiustranformation hat eine [[Umkehrabbildung]] $M^{-1}(z) = \frac{dz-b}{-cz+a}$ 
- Die [[Verknüpfung]] zweier nicht-invertierbarer Möbiustranformationen ist wieder eine nicht-invertierbare Möbiustranformation
- $\varphi_{1, 0, 0, 1}$ ist das neutrales Element

### Drei Fixpunkte
Die Fixpunktgleichung 
$$M(z) = \frac{az + b}{cz+d} = z$$ ist eine versteckte [[Quadratische Gleichung]], kann also maximal zwei Lösungen haben, es sei denn $M(z)$ ist die [[Identität (Mathematik)]].

D.h.: Hat eine Möbiustransformation drei Fixpunkte, dann ist sie die [[Identität (Mathematik)|Identität]].


### Biholomorphe Funktionen
Die Menge aller Möbiustransformationen $\mathcal{M}$ ist genau die Menge aller [[Biholomorphe Funktion|biholomorphen Funktionen]] $Aut(\hat{\mathbb{C}})$ von $\hat{\mathbb{C}}$ nach $\hat{\mathbb{C}}$



### Erhaltung von Zusammenhangskomponenten
Sei
- $\varphi: \hat{\mathbb{C}} \to \hat{\mathbb{C}}$ eine Möbiustransformation
- $L \subseteq \hat{\mathbb{C}}$ eine verallgemeinerte Kreislinie

Dann zerfällt $\hat{\mathbb{C}} \backslash L$ in zwei Zusammenhangskomponenten $K_1, K_2$ und $\varphi(\hat{\mathbb{C}} \backslash L)$ in zwei Zusammenhangskomponenten $M_1, M_2$ und es gilt:
$$\varphi(K_1) = M_1 \text{ und } \varphi(K_2) = M_2$$[^3]

### Fixpunkt Unendlich
Ist $\infty$ ein [[Fixpunkt]] der nicht-invertierbare Möbiustransformation $\varphi: \hat{\mathbb{C}} \to \hat{\mathbb{C}}$, dann ist die Möbiustranformation eine [[Ahnlichkeitabbildung]]:  

D.h. es hat die Form:
$$\varphi: \begin{array}{rcl} \hat{\mathbb{C}} & \to & \hat{\mathbb{C}} \\ z & \mapsto & \begin{cases} Az+B & \text{für } z \in \mathbb{C} \\ \infty & \text{für } z = \infty\end{cases}\end{array}$$ oder $\varphi = \varphi_{A, B, 0, 1}$[^4]

### Isometrische Kreise
Bei jeder Möbiustransformation bilden die Kreise mit der Eigenschaft $|z+\frac{d}{c}| = |\frac{1}{c}|$ auf Kreise gleicher Größe ab.
Insbesondere wird jeder Kreisbogen auf einen Kreisbogen gleicher Länge abgebildet.
Man nennt diese Kreise daher Isometrische Kreise.[^5]



#Mathe-IV 
#Needham 

[^1]: Zenk - Satz 24.4.2
[^2]: Zenk - Lemma 24.4.3
[^3]: Zenk - Lemma 24.4.4
[^4]: Zenk - Lemma 24.4.6
[^5]: Needham - Kap. 3, Aufgabe 19
[^6]: Needham - Kap. 3, Aufgabe 21
[^7]: Needham - Formel 3.3
[^8]: Needham - Abschnitt 4.4.3