# Beschreibung
Hier geht es um die didaktische Behandlung von der [[Ableitung]]

# Grundvorstellungen
- Differentialquotient als lokale Änderungsrate
und Differenzenquotient als mittlere Änderungsrate 
*(Anwendungsbezogene Vorstellung, z.B. bei Blitzern gemessene Geschwindigkeit)*
- Differenzenquotien als Steigung von Sekanten
Differentialquotient als Steigung des Graphen 
*(Am Graphen orientierte Vorstellung)*
- Differenzenquotient als Steigung approximierender Funktionen
Differentialquotient als Steigung einer optimal approximierenden Funktion
*Die Approximierung passiert durch das Hereinzoomen. Vergrößert man eine Funktion genug, sieht sie aus wie eine eine lineare Funktion. Im Gegensatz zur zweiten Vorstellung ist diese sehr global. Eine Funktion lässt sich leicht an beliebigen Prunkten vergrößern.*




# Beispiele
## Nicht-Differenzierbare Funktionen
- $|x|$
- $\cos(1/x)$
- $x\sin(1/x)$

## Differenzierbare Funtionen
- $x^2\sin(1/x)$

# Aufgaben
## Feedbackaufgabe
![[Ableitung Feedbackaufgabe.png]]
Es wird die Grundvorstellung einer Sekante verwendet, deren zwei Definierende Schnittpunkte mit den x-Werten $x, x_0$ immer näher aneinander rücken. 
Berechne die Steigung dieser Sekante:
$$m(x_0) = \underset{x \to x_0}{\lim}\frac{f(x_0)-f(x)}{x_0-x} = \underset{x \to x_0}{\lim}\frac{\frac{1}{x^2_0}-\frac{1}{x^2}}{x_0-x} = \underset{x \to x_0}{\lim}\frac{\frac{x^2-x_0^2}{x^2x^2_0}}{x_0-x} = -\underset{x \to x_0}{\lim}\frac{x+x_0}{x^2x^2_0} = -\frac{2}{x^3}$$

# Übungen
## Klausur 2020 Aufgabe 6
![[Klausur 2020 Aufgabe 6.png]]
$\frac{125m^3-0m^3}{1h-0h} = 125\frac{m^3}{h}$ (Differentialquotient als mittlere Änderungsrate)
$f'(x) = 3t^2-48t+144, f'(1) = 3-48+144 = 99$ (Differentialquotient als lokale Änderungsrate)
