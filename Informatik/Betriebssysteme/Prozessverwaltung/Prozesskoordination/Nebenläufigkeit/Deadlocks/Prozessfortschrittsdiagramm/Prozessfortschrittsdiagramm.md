# Beschreibung
Ein Prozessfortschrittsdiagramm zeigt, wie weit zwei Prozesse abgearbeitet wurden.
Die wird durch Graphen in diesem Diagramm dargestellt.

![[Prozessfortschrittsdiagramm.png]]

## Unmöglicher Bereich
Auffällig ist der unmögliche Bereich. Hierbei handelt es sich um den Bereich, in dem zwei [[Prozess|Prozesse]] das gleiche [[Betriebsmittel]] benötigen.

Dieser Prozess ist unerreichbar, da nie auf von anderen Prozessen beschlagnahmte Betriebsmittel zugegriffen werden kann

## Unsicherer Bereich
Desweiteren gibt es einen unsicheren Bereich. Der Graph kann nur nach links und nach rechts fortgeführt werden. Landen die Prozesse also hier drin, dann ist eine [[Verklemmung]] unvermeidlich

# Lösungen für unsicheren Bereich
## 1. Ressourcen freigeben
Gibt man eine Ressource frei, bevor auf eine andere zugegriffen wird, kann kan unsicherer Bereich entstehen.

![[Unsicherer Bereich verhindern I.png]]

Das kann man aber im allgemeinen nicht einprogrammieren. 
Zum Beispiel braucht man manchmal zwei Ressourcen gleichzeitig. Durch die obere "Lösung" ist das nicht mehr möglich.

## 2. Gleiche Ressource zuerst
Beide Prozesse nehmen die selbst Prozesse zuerst.

![[Unsicherer Prozess vermeiden II.png]]

*Aber so etwas müsste man doch erst in das Programm schreiben, oder? Vielleicht kann auch das Betriebssystem etwas zaubern.*

#Betriebssysteme 
