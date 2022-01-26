## Beschreibung
Eine **Konkatenation** verknüpft zwei [[Wort|Wörter]]

## Definition
Seien $v = v_1...v_n, w=w_1...w_m$ Wörter.

Dann ist $v \circ w = v_1...v_nw_1...w_m$ die **Konkatenation** der Wörter.
Die Wörter werden aneinandergehängt.[^1]

Das $\circ$ wird häufig auch weggelassen

### k-Fache Konkatenation eines Wortes
Sei $w$ ein Wort und $k\in \mathbb{N}$

$w^ik$ bezeichnet die k-fache Konkatenation von $w$ und wird so induktiv definitiert:
- $w^0 := \varepsilon$
- $w^k := ww^{k-1}$

#FSK 
[^1]: Sabel - Definition 2.1.3