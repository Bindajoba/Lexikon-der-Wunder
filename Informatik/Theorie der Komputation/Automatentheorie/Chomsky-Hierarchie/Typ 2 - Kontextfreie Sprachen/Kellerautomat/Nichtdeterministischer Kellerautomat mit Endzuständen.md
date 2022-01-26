## Beschreibung
Ein **nichtdeterministischer Kellerautomat mit Endzuständen** (auch **pushdown automaton, PDA**) ist so etwas wie ein [[Nichtdeterministischer Endlicher Automat]], der um einen [[Keller]] (Stack) erweitert wurde.
Bei jedem Zustandwechsel kann das oberste Element des Kellers gelesen werden oder beliebig viele neue Objekte auf den Keller gelegt werden.
Das ermöglicht dem Automaten jetzt kompliziertere Dinge zu speichern.

## Definition
Ein (nichtdeterministischer) Kellerautomat ist ein [[Tupel]] $M = (Z, \Sigma, \Gamma, \delta, z_0, \#, E)$, wobei
- $Z$ ist eine endliche Menge von **Zuständen**
- $\Sigma$ ist das (endliche) Eingabe-[[Alphabet]]
- $\Gamma$ ist das (endliche) Kelleralphabet
- $\delta: Z \times (\Sigma \cup \varepsilon) \times \Gamma \to \mathcal{P}_e(Z \times \Gamma^*)$ ist die **Zustandsüberführungsfunktion**
- $z_0 \subseteq Z$ ist der **Startzustand**
- $\# \in \Sigma$ ist der **Startzustand** im Keller
- $E\subseteq Z$ ist die Menge der Endzustände[^1]

### Akzeptierte Sprache
Die durch $M$ akzeptierte Sprache $L(M)$ ist definiert als
$$L(M) := \{w \in \Sigma^*:(z_0, w, \#) \vdash^* (z, \varepsilon, W)\text{ und } z\in E\}$$
*Das bedeutet, dass ein Wort nicht bei einem leeren Keller akzeptiert wird. Im Gegenteil, ist der Keller leer, kann kein Zustand mehr gewechselt werden. Das Wort wird nicht akzeptiert, wenn der Zustand auf dem man steht kein Endzustand ist.*

## Umwandlungen
Jeder **Kellerautomat mit Endzustand** kann in einen normalen [[Nichtdeterministischer Kellerautomat]] umgewandelt werden.[^2]

Dazu müssen zwei Probleme gelöst werden:
- Der Automat kann nicht mit leerem Stapel in einen Nicht-Endzustand kommen
*Das wird gelöst, indem durch einen neuen Startzustand unter den Stapel ein neues Symbol \$ gelegt wird, dann kann der Stapel nicht mehr leer gehen*
- An einen Endzustand muss der Automat die Möglichkeit haben, seinen Stapel zu leeren. 
*Dazu wird eine einfache Konstruktion an den Endzustand angehängt*

#FSK 

[^1]: Sabel - Definition 5.7.7
[^2]: Sabel - Lemma 5.7.8