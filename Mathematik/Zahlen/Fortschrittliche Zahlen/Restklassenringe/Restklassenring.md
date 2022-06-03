TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Restklassenringe sind die Ring, die man durch die Modulooperation erhält.
Sie sind bekannt dafür im Allgemeinen nicht mal ein [[Integritätsbereich]] zu sein.

# Übungen
## Zth Klausur 2019 Aufgabe 5
![[Zth Klausur 2019 Aufgabe 5.png]]

### a)
- $5^3 = 25*5 = 11 * 5 = 55 = 13$
- $5^{-1} = 3$, denn $3*5 = 15 = 1$
- $5^{-2} = (5^{-1})^2 = 9$

### b)
- $\alpha^2 = x^2+(f) \neq 1$, da ganzzahlige Division ergibt $x^2 = 0*f + x^2$, denn $grad(x^2) < f$. aber $x^2 \neq 1$
- $\alpha^2 = x^2+(f)=-1$, da ganzzahlige Division ergibt $x^2 = 0*f + x^2$, denn $grad(x^2)<f$ aber $x^2 \neq 1$.
- $\alpha^4 = x^4 + (f) = 1$, da ganzzahlige Division: $x^4 = 1*f + 1$

## McEliece Übung 5-4
$x^2-1$ hat in $\Z/8\Z$ vier Nullstellen.

### a)
Wie viele Nullstellen hat $x^2-1$ in $\Z/16\Z$?
$4$, nämlich $1, 7, 9, 15$, wie man durch Ausprobieren feststellen kann:
- $1^2 = 1$
- $3^2 = 1*8+1$
- $5^2 = 3*8+1$
- $7^2 = 6*8+1$
- $9^2 = 10*8 +1$
- $11^2 = 15*8+1$
- $13^2 = 21*8+1$
- $15^2 = 28*8+1$

### b)
Wie viele Nullstellen hat $x^2-1$ in $\Z/2^n\Z$?
Damit $a$ eine Nullstelle ist, muss $x$ ungerade sein. Eine Gerade Zahl im Quadrat ist in $\Z/2^n\Z$ wieder gerade und kann damit nicht $1$ sein.
$a$ kann also geschrieben werden als $a = 2b+1, b \in \{1, ..., 2^{n-1}\}$.
$a^2- 1 = (2b+1)^2 = 4b^2+4b+1 -1 = 4(b^2+b) = 0 \iff (b^2+b) = b(b+1)$ ist durch $2^{n-2}$ teilbar. Das ist genau dann erfüllt, wenn entweder $b$ oder $b+1$ durch $2^{n-2}$ teilbar ist (da immer mindestens einer der Faktoren ungerade ist und damit diese Eigenschaft nicht besitzen kann). Es gibt zwei Zahlen in $\{1, ..., 2^{n-1}\}$, die durch $2^{n-2}$ teilbar sind, nämlich $2^{n-2}, 2^{n-1}$.
Die Zahlen $2^{n-2}-1, 2^{n-2},2^{n-1}-1, 2^{n-1}$ bilden damit die einzigen Zahlen mit denen $(2b+1)^2-1$ durch $2^n$ teilbar ist.




#Zahlentheorie 


