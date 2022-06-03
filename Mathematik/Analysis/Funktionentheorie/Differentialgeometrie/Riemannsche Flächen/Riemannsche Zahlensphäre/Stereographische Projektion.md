## Beschreibung
Die **Stereographische Projektion** ist eine Methode die Oberfläche einer [[n-Sphäre|Sphäre]] bijektiv auf eine Fläche zu übertragen.

## Definition
### Definition (Zenk)
$$P: \begin{array}{rcl} \mathbb{S} & \to & \hat{\mathbb{C}} \\ (u_1, u_2, u_3) & \mapsto & \begin{cases} z = \frac{u_1 + iu_2}{1- u_3} & \text{ für } (u_1, u_2, u_3) \in \mathbb{S} \backslash \{(0,0,1)\} \\ \infty & \text{für } (u_1, u_2, u_3) = (0,0,1)\end{cases} \end{array}$$ 
heißt **stereographische Projektion**.

![[Stereographische Projektion.png]]

*Mit der stereographischen Projektion wird die [[Riemannsche Zahlensphäre]] definiert.*

### Definition als Inversion
Betrachtet man die obere Graphik, merkt man, dass sie einen Kreis auf eine Gerade abbildet. Nach einiger Überlegung, woran uns das erinnert, denken wir an die [[Inversion]] an einer Kugel.

Genauer gesagt die Kugel um den Nordpol mit dem Radius $\sqrt{2}$. Offensichtlich werden die Zahlen des Einheitskreises auf sich selbst abgebildet. Und da die Urbildkugel durch den Mittelpunkt der Inversionkugel geht ist, muss sie auf genau die Ebene abgebildet werden.



### Umkehrabbildung
$P$ hat die [[Umkehrabbildung]] $Q$ mit:
$$Q: \begin{array}{rcl} \hat{\mathbb{C}} & \to & \mathbb{S} \\ (u_1, u_2, u_3) & \mapsto & \begin{cases} \left(\frac{2x}{|z|^2+1}, \frac{2y}{|z|^2+1}, \frac{|z|^2-1}{|z|^2+1} \right) & \text{für } z \in \mathbb{C} \\ (0,0,1) & \text{für } z = \infty\end{cases} \end{array}$$ 

## Eigenschaften
### Isometrischer Isomorphismus
Die **Stereographische Projektion** ist ein [[Mathematik/Algebra/Algebraische Strukturen/Gruppen/Gruppen nach Arnold/Isometrie|isometrischer]] [[Isomorphismus]]

Dass die Projektion eine Isometrie ist, ist ziemlich dämlich, da sie auf $\hat{\mathbb{C}}$ abbildet, dessen [[Metrik]] genau die [[Umkehrabbildung]] der **Stereographischen Projektion** ist.[^1]

### Konformität
Die stereographische Projektion ist [[Konformität (Analysis)|konform]].
D.h. eine Funktion zwischen zwei komplexen Ebenen ist genau dann [[Analytische Funktion|analytisch]], wenn die Abbildung zwischen den [[Riemannsche Fläche]] konform ist.[^2]

#Mathe-IV
#Needham 

[^1]: Zenk - Lemma 24.1.5
[^2]: Needham - Abschnitt 4.6.3