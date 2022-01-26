## Beschreibung

Ein deterministischer endlicher Automat (DEA, DFA) ist ein [[Automat]]. Er hat einen einzigen Startzustand. Das Einlesen eines Zeichens hat genau einen Zustandwechsel zur Folge

Ein Deterministischer Endlicher Automat kann als Spezialfall eines [[Nichtdeterministischer Endlicher Automat]] betrachtet werden

## Definition

Ein endlicher Automat ist ein 5-Tupel $M = (\Sigma, Z, \delta, z_0, E)$ wobei:
 - $\Sigma$ ist ein endliches [[Alphabet]]
 - $V$ ist ein eine Menge von **Zuständen**
 - $z_0 \in Z$ ist ein der **Startzustand** aus
 - $E \subseteq V$ ist eine Menge von **Endzuständen** (auch **Akzeptierter Zustand**)
 - $\delta$ ist die **Zustandsüberführungsfunktion** (auch **Überführungsfunktion**)

DFAs werden häufig durch Zustandsgraphen dargestellt.

### Zustandüberführungsfunktion
$\delta$ nimmt als Eingabe den aktuellen Zustand und ein Zeichen $a \in \Sigma^*$ an.
Als Ausgabe bekommt es den Zustand zurück, in dem sich der Automat nach Anwendung des Zeichens befindet.[^3]


### Zustandsgraph
Siehe Wikipedia

### Rekursive Zustandsüberführungsfunktion
Sei $M = (\Sigma, Z, \delta, z_0, E)$
Wir definieren die Funktion $\hat\delta: Z \times \Sigma^* \in Z$ rekursiv durch
$$\hat\delta(z, \varepsilon):=z \text{ und } \hat\delta(z, aw)=\hat\delta(\delta(z, a), w)$$
$\hat\delta$ nimmt als Eingabe den aktuellen Zustand und ein [[Wort]] an.
Als Ausgabe bekommt es den Zustand zurück, in dem sich der Automat nach Durchlaufen des Wortes befindet.

### Akzeptiere Sprache
Sei $M = (\Sigma, Z, \delta, z_0, E)$
Die von $M$ erzeugte Sprache ist
$$L(M):=\{w \in \Sigma^* : \hat\delta(z_0, w) \in E\}$$[^4]

Die von DEA erzeugte [[Formale Sprache|Sprachen]] ist genau die Menge der [[Reguläre Sprache|regulären Sprachen]] [^5]

### Lauf
Eine Folge von Zuständen $(q_0, ..., q_n)$, die ein Automat $M$ beim Lesen eines Wortes $w$ durchläuft nennt man Lauf von $M$ für Wort $w$.

## Variationen


### $\varepsilon$-Produktionen
Fügt man einer regulären Grammatik eine Produktion eine sogenannte $\varepsilon$-Produktion $A \to \varepsilon$ hinzu, so ist die erzeugte Sprache immer noch regulär.[^1]

*Das folgt, indem man eine $\varepsilon$-Produktion zum Start der Sprache hinzufügt und dann die vorher hinzugefügte Produktion wieder entfernt.*[^2]

#FSK 

[^1]: Sabel - Definition 3.2.5
[^2]: Sabel - Satz 3.2.6
[^3]: Sabel - Definition 4.1.2
[^4]: Sabel - Definition 4.1.5
[^5]: Sabel - Theorem 4.4.5