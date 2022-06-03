TARGET DECK: Universität::Informatik::NaCo

# Beschreibung


# Definition
Für einen [[Lambda-Term]] $L$ schreiben wir $[x := M]$ für den $\lambda$-Term, wo jedes freie Auftauchen der Variable $x$ ersetzt wird durch einen $\lambda$-Term $M$. Formal schreiben wir:
- $x[x := M ] = M$
- $y[x :=M] = y$ wenn $y \neq x$
- $(\lambda x.M)[x := N] = (\lambda x.M)$
- $(\lambda y.M)[x := N] = (\lambda y .M[x:=N])$ wenn $x \notin \mathfrak{F}(M)$ oder $y \notin \mathfrak{F}(N)$
- $(\lambda y.M)[x := N] = (\lambda z .M [y := z ])[x :=N]$ wenn $x \in \mathfrak F (M)$ und $y \in \mathfrak{F}(N)$ wobei $z$ eine neue Variable ist
- $(M \,N)[x:=O]= (M[x:=O]\, N[x:= O])$

für $\lambda$-Terme $M, N, O \in \Lambda$ und Variablen $x, y, z \in V$



#Natural-Computing 
