## Beschreibung
Der Satz von Myhill und Nerode gilt genau bei [[Reguläre Sprache|Regullären Sprachen]]. 
Es lässt sich damit also feststellen, ob eine [[Formale Sprache]] eine [[Reguläre Sprache]] ist.

## Definition
### Nerode-Relation
Sei $L$ eine formale Sprache über $\Sigma$. Die **Nerode-Relation** $\sim_L \subseteq \Sigma^* \times \Sigma^*$ zu $L$ ist definiert für alle [[Wort|Worte]] $u, v \in \Sigma^*$ durch:
$$u \sim_L v \iff \forall w \in \Sigma^*: uw\in L \iff vw \in L$$
D.h.: $u$ und $v$ sind äquivalent, wenn beide in der Sprache oder nicht in der Sprache $L$ enthalten sind, wenn man sie um den gleichen Suffix $w$ erweitert.[^1]

Die Rerode Relation ist folglich eine [[Äquivalenzrelation]][^2]

### Satz von Myhill und Nerode
Eine [[Formale Sprache]] $L$ ist genau dann [[Reguläre Sprache|regulär]], wenn der [[Index einer Äquivalenzrelation]] von $\sim_L$ endlich ist.[^3]

*Der Beweis geht ungefähr so:
Jede reguläre Sprache lässt sich durch einen [[Deterministischer Endlicher Automat]] darstellen.
Lässt man diesen Automaten ein Worte $u\in \Sigma^*$ lesen, dann befindet sich der Automat für jedes Wort in einem bestimmten Zustand.
Landet der Automat bei zwei verschiedenen $u, v\in \Sigma^*$ Worten im gleichen Zustand, dann ist offensichtlich, dass beim Anhängen eines Suffixes der Automat entweder in einem Endzustand oder nicht in einem Endzustand landet.

Nochmal zurück, wird ein Wort eingelesen, dann ist der Automat in einem bestimmten Zustand. Da ein endlicher Automat aber nur endlich viele Zustände geben, kann die Zahl der [[Äquivalenzklasse|Äquivalenzklassen]] der Nerode Relation auch höchstens endlich sein.*


#FSK 

[^1]: Sabel - Definition 4.10.1
[^2]: Sabel - Satz 4.10.2
[^3]: Sabel - Theorem 4.10.3