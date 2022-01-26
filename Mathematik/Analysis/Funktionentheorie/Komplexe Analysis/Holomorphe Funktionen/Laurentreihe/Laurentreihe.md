## Beschreibung
Bisher haben wir eien [[Analytische Funktion]] durch eine Potenzreihe auf einer Kreisscheibe definiert. Anscheinend kann man aber auch eine [[Analytische Funktion]] durch eine Laurentreihe auf einem Kreisring definieren.

Auf diese Weise wird beispielsweise die Problematik mit dem Konvergenzradius der Funktion $\frac{1}{z}$ umgangen. Nähert man sich dem Pol, dann verringert sich der Konvergenzradius der Potenzreihenentwicklung. 

Laurentreihen geben aber eine Beschreibung von $\frac{1}{z}$ für alle definierten Werte, da durch den Kreisring einfach der Pol aufgelassen werden kann.

## Definition
Sei $a \in \mathbb{C}$ ein Entwicklungspunkt, dann heißt eine Reihe der Form
$$\sum\limits_{n=-\infty}^\infty c_n(z-a)^n$$eine Laurentreihe.

*Eine Laurentreihe ist wohl sowas wie eine [[Potenzreihe]], die bei minus unendlich beginnt.*

### Hauptteil
Zur oberen Laurentreihe heißt 
$$\sum\limits_{n=-\infty}^{-1} c_n(z-a)^n$$ der **Hauptteil**

### Nebenteil
Zur oberen Laurentreihe heißt 
$$\sum\limits_{n=0}^{\infty} c_n(z-a)^n$$ der **Nebenteil**

### Isolierte Singularität
Siehe [[Isolierte Singularität]]


## Eigenschaften
### Konvergenz Hauptteil
Die Potenzreihe
$$\sum\limits_{n=1}^\infty c_{-n}(z-a)^n$$ hat einen Konvergenzradius $\rho$ und konvergiert für $|z-a|<\rho$

Deshalb konvergiert der Hauptteil [[Lokal Gleichmäßige Konvergenz|lokal gleichmäßig]]:
$$\sum\limits_{n=-\infty}^{-1} c_n(z-a)^n = \sum\limits_{n=1}^{\infty} c_{-n}\left(\frac{1}{z-a}\right)^n$$ wenn $|\frac{1}{(z-a)}| < \rho$, bzw. $|z-a| > \frac{1}{\rho} =: r$
*Ich nenne $r$ ab sofort den Konvergenzradius des Hauptteils. Beachte, dass $r$ auch $0$ oder $\infty$ sein kann.*

### Konvergenz Nebenteil
Der Nebenteil ist eine einfache Potenzreihe und konvergiert dann wenn $|z-a|<R$, wobei $R$ der Konvergenzradius vom Nebenteil ist.

### Konvergenz
Eine Laurentreihe konvergiert, wenn der Haupt- und Nebenteil konvergiert. D.h. wenn:
$$\sum\limits_{n=1}^{\infty} c_{-n}(z-a)^{-n} \text{ und }\sum\limits_{n=0}^{\infty} c_n(z-a)^n$$ konvergiert.

Das passiert dann, wenn $r < |z-a| < R$. Gilt also
- $r < R$, dann konvergiert die Laurentreihe auf $\{z \in \mathbb{C}: r<|z-a|<R\}$ (Diese Punktmenge nennt man einen [[Kreisring]])
- $R < r$, dann gibt es keinen Punkt auf dem die Laurentreie konvergiert.
- $r = R$, dann erhält man über die Konvergenz auf der Menge $\{z \in \mathbb{C}: |z-a| = r = R\}$ keine Aussage[^1]

### Beschreibung von Analytischen Funktionen
Seien
- $0 < r_0 < r_1 <\infty$, sodass der Abluss des [[Kreisring]] 
$\overline{\mathcal{R}}:=\{z \in \mathbb{C}: r_0 \leq |z-a| \leq z_1\} \subseteq U$ (Der Beweis gilt auch für $0 \leq r_0 < r_1 \leq \infty$)
- $\gamma_0: \begin{array}{rcl} [0,2\pi] &\to & \mathbb{C} \\ t & \mapsto & a+r_0e^{it} \end{array}$ und $\gamma_1: \begin{array}{rcl} [0,2\pi] &\to & \mathbb{C} \\ t & \mapsto & a+r_1e^{it} \end{array}$ [[Kreisweg|Kreiswege]] an den Rändern des Kreisrings.
- $f: U \to \mathbb{C}$ eine auf der offennen Menge $U$ definitierte analytische Funktion.

Dann gibt es:
- Ein auf $\{z \in \mathbb{C}: |z-a| < r_1\}$ lokal gleichmäßig absolut konvergenter Nebenteil einer Laurentreihe
$$g_1(z)= \sum\limits_{n=0}^{\infty} c_n(z-a)^n = \sum\limits_{n=0}^{\infty} (z-a)^n \frac{1}{2\pi} \int\limits_{\gamma_1} \frac{f(\xi)}{(\xi-a)^{k+1}}d\xi$$
- Ein auf $\{z \in \mathbb{C}: z_0 < |z-a|\}$ lokal gleichmäßig konvertenter Hauptteil einer Laurentreihe
$$g_2(z)= \sum\limits_{n=1}^{\infty} c_{-n}(z-a)^{-n} = \sum\limits_{n=1}^{\infty} \frac{1}{(z-a)^n} \frac{1}{2\pi} \int\limits_{\gamma_1} f(\xi)(\xi-a)^{k+1}d\xi$$

sodass $f(z) = g_1(z) + g_2(z)$[^2]
$g_1(z) + g_2(z)$ heißt denn die **Laurentreihenentwicklung von $f$ zum Entwicklungspunkt $a$ auf dem Kreisring $\mathcal{R} = \{z \in \mathbb{C}: r_0 \leq |z-a| \leq z_1\}$**[^3]

#Mathe-IV 

[^1]: Zenk - Satz 23.1.3 
[^2]: Zenk - Satz 23.1.4
[^3]: Zenk - Definition 23.1.5