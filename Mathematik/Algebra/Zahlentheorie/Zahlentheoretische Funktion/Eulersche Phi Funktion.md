## Beschreibung
Die Eulersche $\varphi$-Funktion $\varphi(n)$ gibt die Anzahl der [[Teilerfremdheit|Teilerfremden Zahlen]] zwischen $1$ und $n$ zurück 

## Definition
$$\varphi(n) = |\{k \in \mathbb{Z} | 0 \leq k < n, ggT(k, n) = 1\}|$$

## Eigenschaften
## Primzahlen
Für jede [[Primzahl]] $p$ kommt als Ergebnis
$$\varphi(p) = p-1$$
da jede Zahl Teilerfremd zu einer Primzahl ist

## Rechenregeln
Sind $n, m$ teilerfremd und $m, n \geq 2$. Dann gilt:
$$\varphi(mn) = \varphi(m)\varphi(n)$$
**Beweis:**
Auf Grund des chinesischen Restsatzes und der Produkteigenschaft der [[Einheitengruppe]] gilt:
$$\mathbb{Z}/mn\mathbb{Z} \cong (\mathbb{Z}/m\mathbb{Z}\times \mathbb{Z}/n\mathbb{Z})^\times \cong (\mathbb{Z}/m\mathbb{Z})^\times\times (\mathbb{Z}/n\mathbb{Z})^\times$$
Die [[Prime Restklassengruppe]] links enthält $\varphi(mn)$, die Menge rechts enthält $\varphi(n)\varphi(m)$ Elemente.[^1]

## Summatorische Funktion
Siehe [[Summatorische Funktion#Eulersche Phi Funktion]]

# Berechnung
## Mit Möbiusschen Umkehrsatz
Der Möbiussche Umkehrsatz gibt eine Möglichkeit, die Summatorische Funktion umzukehren. Tun wir das, erhalten wir:
$$\phi(n) = \sum_{d \mid n}\mu(d)id(\frac{n}{d}) = n\sum_{d \mid n}\frac{\mu(d)}{d}$$

# Übungen
## McEliece Übung 5-5
Sei $p$ eine Primzahl. Berechne $\phi(p^n)$.
Nach Vorlesung $\phi(p^n) = (p-1)p^{n-1}$

Das sieht sehr nach Induktion aus.
Induktionsanfang $n = 1$
$\phi(p^1) = p-1$
Induktionsschritt: $n+1$
$p^{n+1} = \sum_{d\mid p^{n+1}} \phi(d) = \sum_{d\mid p^{n}} \phi(d) + \phi(p^{p+1}) = p^n + \phi(p^{n+1}) \implies = \phi(p^{p+1}) = (p-1)p^n$
*Huch, ich habe gar keine Induktion gebraucht...*

## McElice Übung 6-3
Berechne mit Möbiusschen Umkehrungssatz:
- $\phi(11) = n\prod_{p\mid n}(1-\frac{1}{p}) = \prod_{i = 1}^mp_i^{e_i-1}(p_i-1) = 11-1=10$
- $\phi(101) = 100$
- $\phi(1001) = 6*10*12 = 720$

*Die oben stehende Formel habe ich auf von McElice, ich habe die Herleitung aber nicht ganz verstanden.*

## McEliece 6-6
Nutze $\phi(n) = n\prod_{p \mid n}(1- \frac{1}{p}) = \prod_{i=1}^mp_i^{e_i-1}(p_i-1)$ um folgendes zu zeigen:

## a)
$$\underset{n \to \infty}{\limsup} \frac{\phi(n)}{n} = 1$$
$$\underset{n \to \infty}{\liminf} \frac{\phi(n)}{n} = 0$$
Zum ersten: Es gibt unendlich viele [[Primzahl|Primzahlen]]. Demnach wird immer irgendwann ein $n$ auftauchen für das gilt $\phi(n) = n-1$.
Für die [[Teilfolge]] der Primzahlen gilt daher
$$\underset{n \to \infty}{\limsup} \frac{\phi(n)}{n} = \underset{n \to \infty}{\limsup}\frac{n-1}{n} = 1$$
Zum Zweiten: Oben haben wir Primzahlen verwendet, vielleicht können wir hier dann Anti-Primzahlen benutzen. Definiere $P_n := p_1...p_m$, wobei $p_1...p_{m_n}$ die Primnahlen bezeichnet, die kleiner sind als $n$.
Dann ist $\phi(P_n) = (p_1-1)...(p_{m_n}-1)$. Was ist dann $\underset{n \to \infty}{\limsup} \frac{\phi(P_n)}{n}$?
Bemerkung: Zwischen $2^m$ und $2^{m+1}$ gibt es für $m > 1$ immer mindestens eine Primzahl. Das ist das Bertrandsche Postulat.[^2]

Für alle Primzahlen $p_i, ..., p_j$ zwischen $2^n$ und $2^{n-1}$ gilt $\frac{p_i-1}{p_i}...\frac{p_j-1}{p_j} \leq \frac{2^{n+1}-1}{2^{n+1}}...\frac{2^{n+1}-1}{2^{n+1}}\leq \frac{2^{n+1}-1}{2^{n+1}}$
Damit lässt sich eine obere Schranke finden.
$$\underset{n \to \infty}{\limsup} \frac{\phi(P_n)}{n} = \underset{n \to \infty}{\limsup} \frac{(p_1-1)...(p_{m_n}-1)}{p_1...p_{m_n}} \leq \underset{n \to \infty}{\limsup} \prod_{l \in \N, 2^l<p_{m_n}}\frac{2^l-1}{2^l}$$
Ich komme nicht drauf, vielleicht mache ich etwas falsch...

## b) 
Finde das kleinste $n$, sodass $\phi(n)/n > 0,99$.
$n$ muss eine Primzahl sein, denn sonst gäbe es eine Zerlegung in $n = p^ma$, wobei $p$ eine Primzahl ist und es gilt $\phi(n)/n < \phi(p^m)/p^m < \phi(p)/p$. Das heißt es gab davor schon eine Zahl, deren Phi Funktion größer war.
Suche die erste Primzahl, die größer ist als $100$. Diese ist $101$. Damit ist $\phi(101)/101 = 100/101 >0,99$

## c)
Finde das kleinste $n$, sodass $\phi(n)/n < 0,1$.
Nach ähnlichem Argument, wie in b), muss $n$ eines dieser $P_n$ aus a) sein.
Probiere einfach ein bisschen herum, bis eine Zahl gefunden ist, die gut genug ist:
- $1/2*2/3*4/5*6/7 * ...$

Ich denke, so etwas müsste ich programmieren, da habe ich aber echt keine Lust drauf.

#Algebra #Zahlentheorie 

 [^1]: Gerkmann - Proposition 9.6  
[^2]: https://de.wikipedia.org/wiki/Bertrandsches_Postulat