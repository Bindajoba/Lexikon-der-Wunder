# Beschreibung
Eine Neuverkabelung, (nach Carter Rewiring) ist eine Modifikation eines [[Cayley-Diagramm]], bei dem die Kanten geändert werden.

# Definition
## Erste Definition
Ein Cayley-Diagramm ist eine Neuverkabelung eines anderen, wenn:
1. Die mit dem Gruppenelementnamen beschrifteten Knoten befinden sich auf der gleichen Stelle
2. Die Diagramme können eine Unterschiedliche Anordnung von Pfeilen haben
3. Die durch das Diagramm induzierte algrabraische Zusammenhänge sind die gleichen.

*Also quasi, wenn die Cayley-Diagramme die gleiche Gruppe erzeugen*

## Fortgeschrittene Definition
Die Pfeile im Cayley-Diagramm sind genau die [[Erzeugendensystem|Erzeuger]] der Gruppe. Eine Neuverkabelung ist also eine Abbildung, die:
1. Jeden Erzeuger auf ein Gruppenelement abbildet
2. Die Bilder der Erzeuger die gleiche Gruppe erzeugen.
  
![[Neuverkabelung Definition.png]]

# Charakterisierungen
## Automorphismus
In der Fortgeschrittenen Abbildung haben wir die Verkabelung als eine Abbildung einer Gruppe $G$ zu sich selbst $G$ beschrieben.
Somit ist die Neuverkabelung zumindest ein [[Homomorphismus]].
Da außerdem durch die Erzeuger die gleiche Gruppe erstellt wird und bei Homomorphismen Kombinationen von Urbilderzeugern einer Kombination von Bilderzeugern entspricht, ist die Abbildung bijektiv und damit ein [[Gruppenautomorphismus]] 


# Beispiel
## Die Gruppe $C_3$
![[Neuverkabelung Beispiel.png]]
Der rote Pfeil zeigt nicht mehr auf $a$ sondern auf $a^2$.
Es gelten aber weiterhin die gleichen Beziehungen.

Das erste Diagramm hat zum Beispiel die Beziehung
$$a*a = a^2$$
folgt man nämlich zweimal dem Pfeil der zu $a$ führt, kommt man bei $a^2$ an.

Das zweite Diagramm erfüllt diese Beziehung auch.
Folgt man zweimal dem Weg, der zu $a$ führt (zwei Pfeile), kommt man bei $a^2$ an. (Da man 4 Pfeile läuft)

Tatsächlich sind das die einzigen Neuverkabelungen
*Es sieht so aus, als hätte jede Primzahl nur zwei Verkabelungen.*

## Die Gruppe $V_4$
![[Neuverkabelung Beispiel II.png]]
Hier fällt auf, dass die Pfeile (darunter der unsichtbare $d$-Pfeil) gleich einer Permutation vertauscht werden können, und dabei die gleiche Gruppe erzeugen.

*Ich weiß aber nicht, ob der gleiche Permutation-Trick funktioniert, wenn man mehrere unsichtbare Pfeile hätte. Ich denke nicht.*

Die unterschiedlichen Neuverkabelungen können wieder als Gruppe behandelt werden, was dann so aussieht:
![[Neuverkabelung Beispiel III.png]]
Verbindet man nun die zueinander gehörigen Knoten durch die Blauen Pfeile erhält man das [[Semidirektes Produkt]].

Konkret erhält man das Produkt
$$D_3 \rtimes V_4$$ da man neuverkabelte Kopien von $V_4$ in einem Cayley-Diagramm von $D_3$ hat.

#Carter 