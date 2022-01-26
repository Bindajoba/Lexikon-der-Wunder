## Beschreibung
Eine **Analytische Funktion mit Stammfunktion** ist eine [[Analytische Funktion]], für die eine [[Stammfunktion (Analysis)|Stammfunktion]] existiert.

## Definition
Seien
- $U \subseteq \mathbb{C}$ der Definitionsbereich von $f$ und Wertebereich von $\gamma$
- $f:U \to \mathbb{C}$ eine komplexwertige Funktion

$f$ ist genau dann eine **Analytische Funktion mit Stammfunktion** wenn:
- $f$ hat auf $U$ eine Stammfunktion[^2] [^3] 

## Aquivalente Definition I
$f:U \to \mathbb{C}$ hat eine Stammfunktion wenn 
$f$ ist stetig und für jeden [[Komplexer Stückweise Differenzierbarer Weg]] $\gamma: [0,1] \to U$ gilt:
$$\int\limits_\gamma f(z) \, dz = 0$$[^2] [^3] 

## Hinreichende Bedingungen
### Einfach Zusammenhängende Menge
 Eine [[Analytische Funktion]] $f:U \to \mathbb{C}$ hat eine Stammfunktion wenn $U\subseteq \mathbb{C}$ [[Einfach Zusammenhängende Menge|einfach zusammenhängend]] ist.



## Eigenschaften
### Schleifenintegrale
Alle [[Wegintegral|Schleifenintegrale]] bei Funktionen mit Stammfunktion haben den Wert 0. 
$$\int\limits_\gamma f(z) \, dz = 0$$ [^1]




## Beispiel
Die Funktion $f(z) = \frac{1}{z}$ hat auf $\mathbb{C}\backslash \{0\}$ keine Stammfunktion, da [[Wegintegral|Schleifenintegrale]] um den [[Pol]] nicht 0 sind. 
Das kann man gut erkennen, indem man die Formel für die [[Umlaufzahl]] etwas variiert.

#Mathe-IV 

[^1]: Zenk - Satz 22.4.2
[^2]: Zenk - Satz 22.4.4
[^3]: Zenk - Satz 22.4.5