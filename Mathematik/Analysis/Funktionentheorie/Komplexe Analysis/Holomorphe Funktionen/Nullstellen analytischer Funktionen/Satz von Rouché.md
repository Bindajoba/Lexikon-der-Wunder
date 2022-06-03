## Beschreibung

Der **Satz von Rouché** gibt Voraussetzungen, wann zwei [[Analytische Funktion|analytischer Funktionen]] $f$ und $f+g$ im Inneren eines Weges gleichviele Nullstellen [[Nullstelle|Nullstellen]] haben.

## Definition
Sei
- $\emptyset \neq \subseteq \mathbb{C}$ [[Offene Menge|offen]]
- $f: U \to \mathbb{C}$ und $g: U \to \mathbb{C}$ analytisch
- $\gamma:[0,1] \to U$ [[Nullhomologie|nullhomolog]] mit $|g(z)|<|f(z)|$ für alle $z \in Spur(\gamma)$

Dann haben $f$ und $f+g$ auf $Spur(\gamma)$ keine Nullstellen und es gilt
$$\sum\limits_{a \in \{z \in U: f(z)=0\}}n(\gamma, a)\omega(f, a) = \sum\limits_{a \in \{z \in U: (f+g)(z)=0\}}n(\gamma, a)\omega(f+g, a)$$

Ist die [[Umlaufzahl]] $n(\gamma, \xi) = 1$ für alle $\xi$ im [[Innere einer Schleife|Inneren]] on $\gamma$, so haben $f$ und $f+g$ gleichviele Nullstellen um Inneren von $\gamma$ - gezählt mit Vielfachheiten.

## Beweis
Man stelle sich vor man geht mit einem Hund spazieren. Man begegnet einem Baum, hält die Leine aber so kurz, dass der Hund den Baum nie erreichen kann. Dann kann der Hund den Baum nur umrunden, wenn man selbst den Baum umrundet.

Genauso verhält sich der Satz von Rouche.
Sei der Baum der Ursprung von $\mathbb{C}$ und der Spaziergang dein Bildweg bezüglich $f(z)$, wobei $z$ eine einfache geschlossene Kurve $\Gamma$ durchläuft.
Die komplexe Zahl von mir zum Hund ich $g(z)$ und die Position des Hundes ist damit $f(z)+g(z)$.

Die Forderung, dass die Leine nicht zum Baum reicht ist $|g(z)|<|f(z)|$ auf $\Gamma$
Nach oberer Schlussfolgerung hat der Hund $f(z)+g(z)$ die gleiche Umlaufszahl um $0$ wie du $f(z)$.

Nach dem [[Argumentprinzip]] muss somit die Anzahl an Nullstellen von $f(z)$ und $g(z)+f(z)$ in $\Gamma$ gleich sein. 