## Definition
Ein Ring ist ein Tripel $(R, +, \cdot)$ bestehend aus einer Menge $R$ und zwei Verknüpfungen $+: R \times R \to R$ und $\cdot: R \times R \to R$, genannt Addition und Multiplikation, so dass die folgenden Bedingungen erfüült sind:
1. Das Paar $(R, +)$ ist eine [[Abelsche Gruppe|abelsche Gruppe]]
2. Das Paar $(R,\cdot)$ ist ein kommutatives [[Monoid]]
3. Es gilt das Distributivgesetz $a(b+c) = ab+ac$

### Nullelement
Das neutrale Element der Additionsverknüpfung wird Nullelement genannt.

### Einselement
Das neutrale Element 


## Eigenschaften
### Notation
Ist $\mathbb{R}$ ein Ring, $r \in \mathbb{R}$ und $n \in \mathbb{Z}$, dann bezeichnet $n\cdot r$ die n-te Potenz in $(\mathbb{Z}, +)$

Bsp.: $3r = r+r+r$

### Startring
Für jeden Ring $R$ existiert ein eindeutig bestimmter [[Homomorphismus]] $\mathbb{Z}\to R$ von Ringen[^1]

## Beispiele
### Nullring
Das Tripel $(\{0\}, +, \cdot)$

# Übungen
## Zahlentheorie Klausur 2019 Aufgabe 1
![[Zahlentheorie Klausur 2019 Aufgabe 1 .png]]
### a)
- $0 = (0, 0, 0)$
- $1 = (1, 1, 1)$
- $\{(1, 1, -1), (1, -1, 1), (1, -1, -1), (-1, 1, 1), (-1, 1, -1), (-1, -1, 1), (-1, -1, -1)\}$

### b)
Es ist kein Integritätsbereich, denn $(1, 0, 0) = (0, 1, 1) = (0, 0, 0)$ also ist $0$ nicht der einzige Nullteiler.


### c)
$char(R) = 0$

## Zth Klausur 2018 Aufgabe 1
![[Zth Klausur 2018 Aufgabe 1.png]]
### a)
$R$ ist kein Integritätsbereich, da es die beiden Nullteiler $(1, 0), (0, 1)$ besitzt und damit auch kein Körper.

### b)
$(1, 1), (1, -1), (-1, 1), (-1, -1)$

### c)
$((0, 1))$

### d)
- Ringhomomorphismus
$\phi((1, 1)) = (1, 1)$
$\phi((a, b)+(c, d)) = \phi((a+c, b+d)) = (b+d, a+c) = (b, a)+(d, c) = \phi(a, b)+\phi(c, d)$
$\phi((a, b)(c, d)) = \phi(ac, bd) = (bd, ac) = (b, a)(d, c) = \phi(a, b)\phi(c, d)$
- Bijektivität
$\phi(R) = R$ und $R$ endlich, d.h. $\phi$ bijektiv
Alternativ über Umkehrfunktion



#Zahlentheorie

[^1]: Gerkmann 2.3