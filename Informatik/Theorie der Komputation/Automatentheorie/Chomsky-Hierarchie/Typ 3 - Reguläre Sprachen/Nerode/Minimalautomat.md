## Beschreibung
Der Minimalautomat (auch Nerode-Automat) ist der **einzige** [[Deterministischer Endlicher Automat]] mit den wenigsten Zuständen, die noch die Sprache $L$ ergibt.[^2]

## Definition
Sei der [[Index]] der [[Nerode-Relation]] $\sim_L$ endlich. Dann gibt es $n \in \mathbb{N}$ [[Wort|Wörter]] sodass $[u_1]_{\sim_L} \cup ... \cup [u_n]_{\sim_L} = \Sigma^*$

$M = (Z, \Sigma, \delta, [\varepsilon]_{\sim_L}, E)$ ein DFA mit
- $Z = \{[u_1]_{\sim_L}, ..., [u_n]_{\sim_L}\}$
- $\delta([u_i]_{\sim_L}, a) = [u_ia]_{\sim_L}$ für alle $a \in \Sigma$
- $E = \{[u_i]_{\sim_L}:i\in\{1, ..., n\}, u_i \in L \}$ 


## Algorithmen
### Umwandlung eines DFA ein einen Minimalautomaten
Beginnt man mit einem DFA der keine unerreichbaren Zustände hat, dann kann man mit Algorithmus 3 einen Minimalautomaten daraus erzeugen.
![[Pasted image 20210607092211.png]]

Die vom Algorithmus 3 berechneten Zustandspaare äquivalent und es gitbt keine weitere Zustandspaare.[^1]
Indem die äquivalenten Zustandspaare verschmolzen werden und die vom Start nicht erreichbaren Zustände entfernt werden entsteht der Minimalautomat.

#FSK 

[^1]: Sabel - Satz 4.11.3
[^2]: Sabel Satz 4.10.7