## Beschreibung
Ein  [[Nichtdeterministischer Kellerautomat mit Endzuständen]], bei dem jede Zustandsänderung, in nur einen anderen Zuständ überführt wird **Deterministischer Kellerautomet mit Endzuständen **(auch **DPDA**) .
Epsilon-Übergänge sind zwar immer noch erlaubt aber von einem Zustand, von dem ein Epsilon-Übergang wegführt, daft kein anderer Zustand wegführen.

## Definition
Ein [[Nichtdeterministischer Kellerautomat]] mit Endzuständen $M = (Z, \Sigma, \Gamma, \delta, z_0, \#, E)$ ist deterministisch (DPDA), wenn für alle $(z, a, A)\in (Z, \Sigma, \Gamma)$ gilt:

$$|\delta(z, a, A)|+|\delta(z, \varepsilon, A)| \leq 1$$

Also, wenn ein Zustand durch ein Zeichen des Wortes und Stapel in maximal einen anderen Zustand wechseln kann, wobei Epsilon-Zustände mit berücksichtigt werden.
 
 
 
## Kommentare
Die von DPDAs akzeptierten Sprachen heißen [[Deterministisch Kontextfreie Sprache|deterministisch kontextfrei]]

#FSK 