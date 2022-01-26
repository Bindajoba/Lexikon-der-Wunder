## Beschreibung
Das **Quotientenkriterium** ist ein Kriterium, mit dem man den [[Konvergenzradius]] einer [[Reihe]] berechnen kann.

## Definition
### Allgemeine Definition
Sei eine Reihe $S = \sum_{n \in \mathbb{N}}a_n$.

Gilt
$$\lim \underset{k \to \infty}{\sup} \left|\frac{a_{k+1}}{a_k}\right|<1$$
dann konvergiert die Reihe.

Gilt
$$\lim \underset{k \to \infty}{\inf} \left|\frac{a_{k+1}}{a_k}\right|>1$$
dann divergiert die Reihe.

Gilt keine der oberen Bedingungen, lässt sich keine Aussage treffen.

### Potenzreihen
Potenzreihen haben die Form $S = \sum_{n \in \mathbb{N}}a_n z^n$.
Anwenden der obere Formel für zu:

Gilt
$$\lim \underset{k \to \infty}{\sup} \left|\frac{a_{k+1}}{a_k}\right||z|<1$$
dann konvergiert die Reihe.

Daraus ergibt sich ein [[Konvergenzradius]]:
$$r = \frac{1}{\lim \underset{k \to \infty}{\sup} \left|\frac{a_{k+1}}{a_k}\right|}$$



#Mathe-I