## Beschreibung
Die Fundamentallösung ist die Lösung einer [[Lineare Homogene MatrixDGL]].


## Definition
Betrachte die [[Lineare Homogene MatrixDGL]] $Y'(t) = A(t)Y(t)$
zum  [[Startwertproblem]] $Y(\tau) = E_d$, dann ist die Fundamentallösung eindeutig und durch die [[Dysonreihe]] gegeben:

$$Y(t) = E_d + \sum_{n=1}^\infty{\int\limits_\tau^t A(t_1) \int\limits_\tau^{t_1} A(t_2)...\int\limits_\tau^{t_{n-1}} A(t_n) \,dt_n ... \,dt_2 \,dt_1}$$

## Spezialfälle
### A(t) ist konstant
Dann ist die Fundamentallösung:
$$Y(t)= e^{t-\tau}A$$

### A(t) ist kommutativ
Gilt $A(s)A(t) = A(t)A(s)$, dann ist die Fundamentallösung:

$$Y = e^{\int\limits_\tau^tA(s)\,ds}$$[^1]

#Mathe-IV 

[^1]: Zenk - Lemma 19.4.6