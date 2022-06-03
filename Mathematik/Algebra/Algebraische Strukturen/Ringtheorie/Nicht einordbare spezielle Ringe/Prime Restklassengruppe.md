# Definition
Die [[Einheitengruppe]] $(\mathbb{Z}/n\mathbb{Z})^\times$ des [[Restklassenring|Restklassenrings]] $\mathbb{Z}/n\mathbb{Z}$ bezeichnet man als **prime Restklassengruppe modulo $n$**
*$n$ muss nicht notwendigerweise prim sein.*
*$^\times$ bezeichnet die [[Multiplikative Gruppe]] des Modulokörpers. Das verringern eines Elements kommt daher, dass $0$ keine Einheit ist.*[^1]

# Eigenschaften
## Anzahl der Elemente
Die Anzahl der Elemente wird durch die [[Eulersche Phi Funktion]] $\varphi (n)$ angegeben.

## Rechenregeln
Sei $p$ eine [[Primzahl]].
- $(\mathbb{Z}/p\mathbb{Z})^\times = \mathbb{Z}/(p-1)\mathbb{Z}$.
- $(\Z/2\Z)^\times \cong \{1\}, (\Z/2^2\Z)^\times \cong \Z/2\Z$
- $(\Z/2^m\Z)^\times \cong \Z/2\Z \times \Z/2^{m-2}\Z$
- $(\Z/p^m\Z)^\times \cong \Z/p^{m-1}(p-1)\Z$ (für ungerade $p$)[^3]

## Isomorphie zur Automorphismengruppe
$(\Z/n\Z)^\times$ ist isomorph zu $Aut(\Z/n\Z)$.

Der Isomorphismus ist $\begin{align} \phi:(\Z/n\Z)^\times &\to Aut(\Z/n\Z) \\ a+n\Z &\mapsto \tau_a \end{align}$, wobei $\tau_a(x) = ax, x\in \Z/n\Z$[^2]

## Erzeugung
Die Prime Restklassengruppe wird durch eine [[Primitivwurzel]] erzeugt.

# Übungen
## Zth Klausur 2019 Aufgabe 3
![[Zth Klausur 2019 Aufgabe 3.png]]
### a)
$(\Z/100\Z)^\times = (\Z/4\Z)^\times \times (\Z/25\Z)^\times = (\Z/2\Z) \times (\Z/20\Z)$.

### b)
Nein, ist sie nicht. Sie hat Ordnung $20$.




#Zahlentheorie #Algebra 


[^1]: Gerkmann - Folgerung 9.5
[^2]: Gerkmann - Satz 3.13
[^3]: Gerkmann - Satz 9.8