TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung


# Definition
Ein [[Polynom (Ring, Körper)]] das durch das Produkt der Linearfaktoren zu primitiven n-ten [[Einheitswurzel|Einheitswurzeln]] entsteht, d.h.
$$\Phi_n = \prod_{\zeta \in \mu_n^\times}(x-\zeta)$$
wird das **$n$-te Kreisteilungspolynom** genannt.

# Eigenschaften
## Produkte
Für alle $n \in \N$ gilt $x^n - 1 = \prod_{d\mid n} \Phi_d$[^1] 


## Kreisteilungspolynome sind Ganzzahlig
Es gilt $\Phi_n \in \Z[x]$ für alle $n \in \N$.

In speziellen Fällen lassen sich explizite Formeln angeben.
- Für $p$ [[Primzahl]]
$$\Phi_p = x^{p-1} + ... + x +1$$
- Für $p^r$ Primzahlpotenz
$$\Phi_{p^r} = \sum_{k=0}^{p-1}x^{kp^{r-1}}$$
Zum Beispiel $\Phi_{25} = x^{20}+x^{15}+x^{10}+x^{5}+1$

## Irreduzibel
Die Kreisteilungspolynome sind [[Irreduzibles Polynom|irreduzibel]] in $\Z[x]$ und $\Q[x]$.



# Beispiele
$\Phi_6 = x^2-x+1$.
Das erhält man, indem man die Formel oben verwendet
$$x^6-1 = \Phi_1\Phi_2\Phi_3\Phi_6$$
und die Gleichung nach $\Phi_6$ auflöst.


#Zahlentheorie 


[^1]: Gerkmann - Lemma 13.4
