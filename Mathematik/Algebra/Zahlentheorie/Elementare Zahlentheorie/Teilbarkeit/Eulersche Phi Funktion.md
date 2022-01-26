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

#Algebra #Zahlentheorie 

 [^1]: Gerkmann - Proposition 9.6 