## Beschreibung
Die Cauchy-Integralformel beschreibt fundamentale Zusammenhänge zwischen der [[Umlaufzahl]] einer [[Nullhomotopie|nullhomotopen]] [Komplexe Stückweise Differenzierbare Schleife]] und einem [[Wegintegral]] über dieser Schleife.

## Definitition
Sei
- $U \subseteq \mathbb{C}$ der Definitionsbereich von $f$ und Wertebereich von $\gamma$
- $f: U \to \mathbb{C}$ eine [[MATHEM~1/Analysis/Funktionentheorie/Klassische Analysis/Analytische Funktion]]
- $\gamma:[\alpha, \beta] \to U$ eine [[Komplexe Stückweise Differenzierbare Schleife]], die in $U$ [[Nullhomotopie|nullhomotop]] ist.

Dann gilt für jedes $z\in U \backslash Spur(\gamma)$:

$$n(\gamma, z)f(z) = \frac{1}{2\pi i} \int\limits_\gamma \frac{f(\xi)}{\xi-z} \, d\xi$$

### Integralformel für Ableitungen
Für jedes $z\in U \backslash Spur(\gamma)$:

$$n(\gamma, z)f^{(k)}(z) = \frac{k!}{2\pi i} \int\limits_\gamma \frac{f(\xi)}{(\xi-z)^{(k+1)}} \, d\xi$$


Eine [[Nullhomologie|Nullhomologe]] Schleife ist [[Nullhomotopie|nullhomotop]], daher kann $\gamma$ auch [[Nullhomologie|nullhomolog]] sein.

#Mathe-IV 