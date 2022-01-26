## Beschreibung
Eine Lösung ist eine Funktion, die eine [[Differentialgleichung]] löst.

## Definition für implizite DGLs
Eine Funktion $\gamma: I \to \mathbb{K}^n$ heißt **Lösung** einer [[Implizite Differentialgleichung]], wenn gilt:
1. $I \subset \mathbb{R}$ ist ein Intervall mit nichtleerem Inneren
2. $\lambda \in C^k(I, \mathbb{K}^n)$
3. $(t, \lambda(t), \lambda'(t), ..., \lambda^{(k)}(t)) \in U$ und
$$F(t, \lambda(t), \lambda'(t), ..., \lambda^{(k)}(t))=0 \tag{1}$$ für alle $t\in I$

## Definition für explizite DGLs
Eine Funktion $\gamma: I \to \mathbb{K}^n$ heißt **Lösung** einer [[Explizite Differentialgleichung|Expliziten Differentialgleichung]], wenn gilt:
1. $I \subset \mathbb{R}$ ist ein Intervall mit nichtleerem Inneren
2. $\lambda \in C^k(I, \mathbb{K}^n)$
3. $(t, \lambda(t), \lambda'(t), ..., \lambda^{(k-1)}(t)) \in U$ und
$$\lambda^{(k)}=f(t, \lambda(t), \lambda'(t), ..., \lambda^{(k-1)}(t)) \tag{2}$$ für alle $t\in I$

## Lösungsidentität
$(1)$ und $(2)$ nennt man die **Lösungsidentität**

#Mathe-IV 