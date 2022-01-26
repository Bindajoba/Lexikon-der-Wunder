## Definition
Eine [[Analytische Funktion]], [[Biholomorphe Funktion|Biolomorphe Funktion]] $f: \mathbb{E} \to \mathbb{E}$ heißt ein **Automorphismus des Einheitskreises**.

Dieser ist offensichtlich ein [[Automorphismus]]

## Charaktierisierung
Eine Grundannahme ist, dass **Automorphismen auf dem Einheitskreis** eine Teilmenge der [[Normalisierte Möbiustransformation]] sind.

Wir bemerken zudem, dass Randpunkte wieder auf Randpunkte abbilden müssen.

Damit kann man Automotphismen auf dem Einheitskreis leicht konstruieren: Man wählt einen Punkt $c$ aus, der auf $0$ abgebildet werden soll. Dann kann man noch den Kreis drehen.

Eine Möbiustransformation, die den ersten Schritt kann ist eine Inversion von $c$ auf $0$ (mit einer nachfolgenden Spiegelung, um die [[Konformität (Analysis)]] zu erhalten), die zudem den Einheitskreis auf sich selbst abbildet.
Eine solche Inversion hat $\frac{1}{\overline{c}}$ als Zentrum. Deshalb wird diser Punkt auf $\infty$ abgebildet und die Transformation hat die Gleichung:

$$Aut(\mathbb{E}) = \left\{g_{c, \lambda}. \begin{array}{rcl}\mathbb{E} &\to &\mathbb{E} \\ z &\mapsto & e^{i\lambda} \frac{z-c}{1-\overline{c}z}\end{array}: \lambda \in [0, 2\pi[ \right\}$$
 
 und nach dem [[Schwarzsches Lemma]]:
 
 $$Aut_0(\mathbb{E}) := \{f \in Aut(\mathbb{E}): f(0)=0\} = \left\{f:\begin{array}{rcl}\mathbb{E} &\to &\mathbb{E} \\ z &\mapsto & e^{i\lambda} z\end{array} : \lambda \in [0, 2\pi[\right\}$$[^1]
 
 ## Eigenschaften
 Hat $f \in Aut(\mathbb{E})$ zwei [[Fixpunkt|Fixpunkte]], so ist $f = id_{\mathbb{E}}$[^2]
 
#Mathe-IV
#Needham 

[^1]: Zenk - Satz 25.2.2 
[^2]: Zenk - Lemma 25.2.3