TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung


# Definition
Ein [[Polynom (Ring, Körper)]] das durch das Produkt der Linearfaktoren zu primitiven n-ten [[Einheitswurzel|Einheitswurzeln]] entsteht, d.h.
$$\Phi_n = \prod_{\zeta \in \mu_n^\times}(x-\zeta)$$
wird das **$n$-te Kreisteilungspolynom** genannt.

# Eigenschaften
## Grad
Da Kreisteilungspolynome das Produkt von Linearfaktoren errechnet aus [[Primitive Einheitswurzel]] ist, kann man den Grad erhalten, indem die Primitiven Einheitswurzeln zählt. Dazu kann man die [[Eulersche Phi Funktion]] verwenden:
$$grad(\Phi_n(x)) = \phi(n)$$

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
Die Kreisteilungspolynome sind [[Irreduzibles Polynom|irreduzibel]] in $\Z[x]$ und $\Q[x]$ aber nicht notwendigerweise in [[Endlicher Körper]].

## Berechnung
Kreisteilungspolynome lassen sich durch die Formel
$$\Phi_n(x) = \prod_{d\mid n}(x^d-1)^{\mu(n/d)}$$
berechnen, wobei $\mu$ die [[Möbius Mu Funktion]] ist.

**Beweis:**
Es gilt $x^n - 1 = \prod_{d\mid n} \Phi_d$. Das ist bloß eine [[Summatorische Funktion]] mit Multiplikation statt Summe geschrieben. Wir können also den [[Möbiusscher Umkehrsatz|Möbiusschen Umkehrsatz]] anwenden und erhalten die obere Formel.

## Rechenformel
Sei $p$ eine Primzahl und $n$ eine dazu teierfremde Zahl. Dann gilt
- $\Phi_{np^k}(x) = \Phi_{np}(x^{p^{k-1}})$
- $\Phi_{np^k}(x) = \frac{\Phi_n(x^{p^k})}{\Phi_n(x^{p^{k-1}})}$
- $\Phi_{np^k}(n) = \Phi_n(x)^{p^k-p^{k-1}}$ in einem [[Körper]] der [[Charakteristik (Ring)|Charakteristik]] $p$


# Beispiele
## Liste aller Kreisteilungspolynome
| $n$ | Polynom           |
| --- | ----------------- |
| $1$ | $x-1$             |
| $2$ | $x+1$             |
| $3$ | $x^2+x+1$         |
| $4$ | $x^2+1$           |
| $5$ | $x^4+x^3+x^2+x+1$ |
| $6$ | $x^2-x+1$         |
| $7$ | $x^6+x^5+x^4+x^3+x^2+x+1$                  |

### Kreisteilungspolynom 5
$\Phi_5 = x^4+x^3+x^2+x+1$
Verwenden wir die [[Möbiustransformation]]:
$$\Phi_5(x) = \prod_{d \mid 5}(x^d-1)^{\mu(5/d)} = \frac{x^5-1}{x-1}$$
Das hätte man sich eigentlich denken können, denn es müsste $4$ [[Primitive Einheitswurzel]] geben. Wenn man also die Nullstelle $1$ als Linearfaktor aus dem Polynom entfernt, sollte man das gesuchte Polynom erhalten. 
Da $\Phi_5$ ein Polynom von Grad $\phi(5) = 4$ ist, müsste $\Phi_5(x) = \frac{x^5-1}{x-1}\mod x^5$ genauso aussehen, wie $\Phi_5(x)$. Wir können uns das zu Nutze machen, da rechnen in $\mod x^5$ viel leichter ist.
$$\begin{align}\frac{x^5-1}{x-1} &= \frac{(x^5-1)(x^4+1)(x^2+1)(x+1)}{x^8-1}\\ &= (x^4+1)(x^2+1)(x+1) \\&= (x^4+1)(x^3+x^2+x+1) \\&= x^4+x^3+x^2+x+1\end{align}$$
Da $x^5 \equiv x^4 \equiv 0 \mod x^5$ und so weiter.

### Kreisteilungspolynom 6
$\Phi_6 = x^2-x+1$.
Das erhält man, indem man die Formel oben verwendet
$$x^6-1 = \Phi_1\Phi_2\Phi_3\Phi_6$$
und die Gleichung nach $\Phi_6$ auflöst.

## Kreisteilungspolynome Primzahlen
Für eine Primzahl $p$ hat das Kreisteilungspolynom die Form 
$$\Phi_p(x)=x^{p-1}+x^{p-2}+...+x+1$$
**Beweis:**
Die $p$ Nullstellen des Polynom $x^p-1$ sind die $p$-ten [[Einheitswurzel]]. Diese bilden eine [[Zyklische Gruppe]] von [[Ordnung (Gruppe)|Primzahlordnung]] $p$. Damit gibt es $\phi(p) = p-1$ Erzeuger der Gruppe und damit $p-1$ [[Primitive Einheitswurzel]]. $1$ ist eine primitive Einheitswurzel, also sind es alle andere.
Entfernen wir daher den Linearfaktor der Einheitswurzel $1$ aus $x^p-1$, dann müssten wir $\Phi_p(x)$ erhalten.
$$\Phi_p(x) = \frac{x^p-1}{x-1} = x^{p-1}+x^{p-2}+...+x+1$$ denn
$$\Phi_p(x) = x^p-1 = (x-1)(x^{p-1}+x^{p-2}+...+x+1)$$



# Übungen
## McEliece Übung 7-1
Zeige, wenn $n$ ungerade, dann gilt $\Phi_{2n}(x)  = \Phi_n(-x)$

Wenn $n$ ungerade, dann sind $2$ und $n$ teilerfremd und es gilt:
$$\Phi_{n*2^1}(x) = \frac{\Phi_n(x^{2})}{\Phi_n(x^{1})} = \frac{\prod_{d \mid n}(x^{2d}-1)^{\mu(n/d)}}{\prod_{d \mid n}(x^d-1)^{\mu(n/d)}}= \prod_{d \mid n}(x^{d}+1)^{\mu(n/d)}$$
Da $n$ ungerade ist, ist auch $d$ ungerade und es gilt:
$$\prod_{d \mid n}(x^{d}+1)^{\mu(n/d)} = \prod_{d \mid n}(-(-x)^{d}+1)^{\mu(n/d)}= \prod_{d \mid n}(-(1-(-x)^{d}))^{\mu(n/d)}$$
Zerlege den Wert in $\mu$ in Primfaktoren: $\mu(n/d) = \mu(p_1^{e_1}...p_m^{e_m})$.
Gibt es ein $e_i$ mit $e_i>1$, dann ist $\mu(p_1^{e_1}...p_m^{e_m}) = 0$. In dem Fall ist $(-(1-(-x)^{d}))^{\mu(n/d)} = (-(1-(-x)^{d}))^{0}= 1 = (1-(-x)^{d})^{\mu(n/d)}$

Gibt es kein $e_i$ mit $e_1 < 1$, dann ist $\mu(n/d) = \pm 1$. In dem Fall gilt $(-(1-(-x)^{d}))^{\mu(n/d)} = -(1-(-x)^{d})^{\mu(n/d)}$
Für jeden Teiler Faktor $n/d =p_1^0p_2^{e_2}...p_m^{e_m}$ gibt es einen eineindeutigen anderen Teiler $n/d' = p_1^0p_2^{e_2}...p_m^{e_m}$, den man erhält, indem man die Zahl des ersten Promzahlexponenten zwischen $0$ und $1$ wechselt.
Für jeden Faktor $(-(1-(-x)^{d}))^{\mu(n/d)}$ aus dem oberen Produkt gibt es damit einen eineindeutigen anderen Faktor $(-(1-(-x)^{d'}))^{\mu(n/d')}$, sodass $(-(1-(-x)^{d}))^{\mu(n/d)}(-(1-(-x)^{d'}))^{\mu(n/d')} = (1-(-x)^{d})^{\mu(n/d)}(1-(-x)^{d'})^{\mu(n/d')}$
Die Produkte, bei denen $\mu(d/n) = \pm 1$ haben also immer ein Gegenstück, bei dem sich das Minus auslöscht. Damit gilt 
$$\prod_{d \mid n}(-(1-(-x)^{d}))^{\mu(n/d)} = \prod_{d \mid n}(1-(-x)^{d})^{\mu(n/d)} = \Phi_n(-x)$$

Ich glaube, das bringt uns nicht weiter, ich brobiere es stattdessen mit der [[Möbiustransformation]]:
$$\Phi_{2n}(x) = \prod_{d \mid 2n}(x^d-1)^{\mu(n/d)}$$

## McEliece Übung 7-2
Uns fällt auf, dass in allen Kreisteilungspolynom außer im ersten der konstante Term $+1$ ist. Steckt da eine Regel dahinter?

Ja, es ist eine Regel. Man erhält ein Kreisteilungspolynom durch:
$$\Phi_{n}(x) = \prod_{d \mid n}(x^d-1)^{\mu(n/d)}$$
Das ist ein rationaler Bruch von Polynomen der Form $(x^d-1)$. Man kann den Bruch in ein Produkt aus Polynomen umschreiben, indem man den Schritten aus dem Beispiel Kreisteilungspolynom 6 folgt. Der konstante Term ist dann das Produkt aller konstanten Terme der Polynomfaktoren. Diese tauchen, wie ich in [[Kreisteilungspolynom#McEliece Übung 7-1]] gezeigt habe in Paaren auf. Also muss der konstante Term $+1$ sein.

## McEliece Übung 7-4
Berechne einige Polynome

### a) $\Phi_{24}(x)$
$\Phi_{24}(x) = \Phi_{3*2^3}(x)  = \Phi_{6}(x^4) = x^8-x^4+1$

### b) $\Phi(35)$
$\phi(35) = 24$
$$\begin{align}\Phi_{35}(x) \\
&= \frac{\Phi_5(x^7)}{\Phi_5(x)} \\
&= \frac{\Phi_5(x^7)(x-1)}{x^5-1} \\
&= \frac{\Phi_5(x^7)(x-1)(x^5+1)(x^{10}+1)(x^{20}+1)}{x^{40}-1}\\
&= -(x^{28}+x^{21}+x{14}+x^7+1)(x-1)(x^5+1)(x^{10}+1)(x^{20}+1)\\
&= -(x^{22}-x^{21}+x^{15}-x^{14}+x^8-x^7+x-1)(x^5+1)(x^{10}+1)\\
&= -(x^{22}-x^{21}+x^{20}-x^{19}+x^{15}-x^{14}+x^{13}-x^{12}+x^8-x^7+x^6-x^5+x-1)(x^{10}+1)(x^{20}+1) \\
&= -(-x^{24}+x^{23}-x^{21}+x^{20}-x^{19}+x^{18}-x^{17}+x^{16}-x^{14}+x^{13}-x^{12}+x^{11}-x^{10}+x^8-x^7+x^6-x^5+x-1)(x^{20}+1)\\
&= -(-x^{24}+x^{23}-x^{19}+x^{18}-x^{17}+x^{16}-x^{14}+x^{13}-x^{12}+x^{11}-x^{10}+x^8-x^7+x^6-x^5+x-1)\\
&= x^{24}-x^{23}+x^{19}-x^{18}+x^{17}-x^{16}+x^{14}-x^{13}+x^{12}-x^{11}+x^{10}-x^8+x^7-x^6+x^5-x+1)\end{align}$$

### c) $\Phi_{40}$

## McEliece Übung 7-6
Sei $K$ ein Feld der Charakterisitik $2$. Berechne
- $\Phi_{10}(x) = \Phi_5(x^{2-1}) = \Phi_5(x) = x^4+x^3+x^2+x+1$
- $\Phi_{12}(x) = \Phi_3(x^{4-2}) = \Phi_3(x^4+x^2+1)$
- $\Phi_{14}(x) = \Phi_7(x) = x^6+x^5+x^4+x^3+x^2+x+1$
- $\Phi_{16}(x) = \Phi_1(x^{16-8}) = x^{8}-1$




#Zahlentheorie #McEliece 


[^1]: Gerkmann - Lemma 13.4