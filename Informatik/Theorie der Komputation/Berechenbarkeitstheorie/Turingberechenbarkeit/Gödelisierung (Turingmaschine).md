## Beschreibung
Die **Gödelisierung einer Turingmaschine** ist ein Verfahren, mit der sich die gesamte Struktur einer [[Turingmaschine]] in eine Zahl umgewandeln lässt.

## Verfahren
Sei $(Z, \Sigma, \Gamma, \delta, z_0, \square, E)$ eine DTM mit $\Sigma = \{0,1\}$ und
- $\Gamma = \{a_0, ..., a_k\}$ wobei $a_0 = \sqare, a_1 = \#, a_2 = 0, a_3 = 1$
- $Z = \{z_0, ..., z_n\}$
- E = $\{z_n\}$

Für $\delta(z_p, a_i) = (z_q, a_j, D)$ erzeuge Wort über Alphabet $\{0, 1, \#\}$
$$w_{p, i, q, j, D} = \#\#bin(p)\#\#bin(i)\#\#bin(q)\#\#bin(j)\#\#bin(D_m)$$ 
mit $D_m = 0$, falls $D = L$, $D_m = 1$, falls $D = R$, $D_m = 2$, falls $D = N$

Dann ist $w_\delta$ das Hintereinanderschreiben aller codieren Zustandübergänge.

Codiere zuletzt das Alphabet $\{\#, 0, 1\}$ durch $\{0 \mapsto 00, 1 \mapsto 01, \# \mapsto 11\}$ und wende dies auf $w_\delta$ an.