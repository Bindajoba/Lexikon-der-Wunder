## Beschreibung
Reguläre Ausdrücke sind wie [[Grammatik|Grammatiken]] oder [[Automat|Automaten]] ein Formalismus zur Darstellung von Sprachen.

*Wich wundert es ein bisschen, dass Reguläre ausdrücke der [[Backus-Naur-Form]] so ähnlich sind. Braucht man da noch reguläre Ausdrücke?*

## Definition
Sei $\Sigma$ ein [[Alphabet]]. Ein regulärer Ausdruck über $\Sigma$ ist ein induktiv definiert durch
- $\emptyset$ ist ein regulärer Ausdruck
- $\varepsilon$ ist ein regulärer Ausdruck
- $a$ mit $a \in \Sigma$ ist ein regulärer Ausdruck
- Wenn $\alpha_1$ und $\alpha_2$ reguläre Ausdrücke sind, dann ist auch $\alpha_1\alpha_2$ ein regulärer Ausdruck
- Wenn $\alpha_1$ und $\alpha_2$ reguläre Ausdrücke sind, dann ist auch $(\alpha_1|\alpha_2)$ ein regulärer Ausdruck
Das oder ist assoziativ, daher werden die Klammern bei Verkettung weggelassen
- Wenn $\alpha$ ein regulärer Ausdrücke ist, dann auch  $\alpha^*$[^1]


### Erzeugte Sprache
Die Erzeugte Sprache setzt sich aus den Wörtern zusammen, die man mit dem regulären Ausdruck bilden kann.[^1]

Die erzeugte Sprache sind genau die regulären Sprachen (**Satz von Kleene**)
Der Beweis basiert darauf, dass man jede Operation des Ausdrucks oben in ein **Automatenbaustein** umwandelt und dann zusammensteckt.[^2]


#FSK 

[^1]: Sabel - Definition 4.7.1
[^2]: Sabel - Theorem 4.7.4