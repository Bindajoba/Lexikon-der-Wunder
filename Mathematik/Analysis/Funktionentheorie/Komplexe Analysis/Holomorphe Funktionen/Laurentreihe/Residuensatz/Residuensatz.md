# Residuensatz I
## Definition
Es sei 
- $U \in \mathbb{C}$ [[Offene Menge|offen]] und [[Einfach Zusammenhängende Menge|einfach zusammenhängend]], 
- $S \subseteq U$ sei eine Menge, die keinen Häufungspunkt in $U$ besitzt
- $f:U \backslash S \to \mathbb{C}$ sei [[Analytische Funktion|analytisch]], dann gilt:

$$\int\limits_\gamma f(z)\,dz = 2 \pi i \sum\limits_{s \in S}n(\gamma, s) Res(f, s)$$ für jeden [[Stückweise Differenzierbare Schleife|stückweisen differenzierbare Schleife]] $\gamma: [\alpha, \beta] \to U \backslash S$[^1]

*Beobachte: in der Summe kann es nur endlich viele von 0 verschiedene Summanden geben, da in das [[Innere einer Schleife|Innere]] einer [[Schleife]] nur endlich viele Punkte passen, ohne, dass sich ein [[Häufungspunkt]] bildet.*

(vgl. [[Residuum]])

### Homologieversion
Es sei 
- $U \in \mathbb{C}$ [[Offene Menge|offen]], 
- $S \subseteq U$ sei eine Menge, die keinen Häufungspunkt in $U$ besitzt
- $f:U \backslash S \to \mathbb{C}$ sei [[Analytische Funktion|analytisch]],
- $\gamma: [\alpha, \beta] \to U \backslash S$ sei [[Nullhomologie|nullhomolog]] in $U$, dann gilt:

$$\int\limits_\gamma f(z)\,dz = 2 \pi i \sum\limits_{s \in S}n(\gamma, s) Res(f, s)$$[^2]



## Folgerungen
Ist $S \subset \mathbb{C}$ eine Menge ohne Häufungspunkt, und $f: \mathbb{C}\backslash S \to \mathbb{C}$ analytisch, so gilt für jeden geschlossenen, stückweisen, differenzierbaren Weg $\gamma:[\alpha, \beta] \to \mathbb{C}\backslash S$
$$\int\limits_\gamma f(z)\,dz = 2 \pi i \sum\limits_{s \in S}n(\gamma, s) Res(f, s)$$ Das ist anscheinend eine Folgerung der ersten beiden Sätze.[^3]

#Mathe-IV 

[^1]: Zenk - Satz 23.2.2
[^2]: Zenk - Satz 23.2.3
[^3]: Zenk - Bemerkung 23.2.4