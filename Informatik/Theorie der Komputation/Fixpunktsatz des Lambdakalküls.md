TARGET DECK: Universität::Informatik::NaCo

# Beschreibung
Der Fixpunktsatz des Lambdakalküls besagt, dass jede Lambdafunktion einen Fixpunkt hat. Dieser lässt sich explizit angeben und nutzen, um die Kraft des while zu schöpfen. (Wodurch das [[Lambda-Kalkül]] [[Turing-Vollständig]] wird)

Q: Was besagt der Fixpunktsatz des Labdakalküls?
A: Das jede Lambdafunktion einen Fixpunkt besitzt.


# Definition
Jede [[Lambda-Term]] im [[Lambda-Kalkül]] hat einen [[Fixpunkt]].
Für eine Funktion $F \in \Lambda$ ist der Fixpunkt gegeben durch $(Y \, F)$, wobei $Y$ der Combinator definiert durch
$$Y = \lambda f .(\lambda x.f(x \, x))(\lambda x .f( x \, x))$$


#Natural-Computing 
