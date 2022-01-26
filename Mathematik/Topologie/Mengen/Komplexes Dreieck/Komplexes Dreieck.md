## Beschreibung
Ein Dreieck ist ein Dreieck im Komplexen Raum

## Definition
Seien $z_1, z_2, z_3$ die Ecken des Dreiecks.

$$D:=\{c_1z_1+c_2z_2+c_3z_3:c_1, c_2, c_3\in \mathbb{R}, c_1, c_2, c_3 \geq 0, c_1+ c_2+ c_3 = 1\}$$*Diese Definition mag auf den ersten Blick sehr undurchsichtig wirken, ergibt aber etwas mehr Sinn, wenn man sich einfache Beispiele ansieht.*

## Beispiel
Wähle $z_1 = 0, z_2 = 1, z_3 = i$:
Dann reduziert sich die obere Definition zu:
$$D:=\{c_2+c_3i:c_1, c_2, c_3\in \mathbb{R}, c_1, c_2, c_3 \geq 0, c_1+ c_2+ c_3 = 1\}$$

Sehen wir uns erstmal alle Punkt an, die entstehen, wenn $c_1 = 0$ ist:
Aus der Bedingung $c_1 + c_2+ c_3 = 1$ folgt 
$$c_2 \cdot 1 + (1-c_2) \cdot i \in D$$ was genau die Strecke zwischen $c_2z_2$ und $c_3z_3$ ist.
![[Komplexes Dreieck - Skizze 1.png]]
Lassen wir jetzt $c_1$ größer werden, dann muss $c_2$ oder $c_3$ kleiner werden, wodurch sich die Strecke von $c_2z_2$ zu $c_2z_2$ in Richtung $z_0$ bewegt.
Alle Punkte auf dieser Strecke sind im $D$ enthalten, damit entsteht ein Rechtwickliges Dreieck.  

Siehe auch:
- [[Dreieck (Didaktik)]]

#Mathe-IV 