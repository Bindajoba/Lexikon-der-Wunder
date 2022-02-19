

# Beschreibung
Der Scheduler ist ein [[Programm]] welches darüber entscheidet, in welcher Reihenfolge die [[Prozess|Anwendungsprozesse]] ausgefürt werden.

Scheduling wird notwendig, sobald 
1. mindestens ein Prozess im Zustand [[7-Zustands-Prozessmodell|running]] ist
2. ein oder mehrere andere Prozesse im Zustand ready darauf warten, dass ihnen die CPU zugeteilt wird.

Dies wird mit einem [[Schedulingalgorithmus]] realisiert.


# Varianten des Scheduling
## Nicht preemptives Scheduling
Siehe [[Nicht-preemptives Scheduling]]

## Preemptives Scheduling
Siehe [[Preemptives Scheduling]]

# Arten des Scheduling
Beim Scheduling werden verschiedene Arten unterschieden:

## Short Term Scheduling
Der Teil des Schedulers, der Prozesse zwischen dem Running, Ready und Blocked-Zustand schaltet

## Medium Term Scheduling
Der Teil des Schedulers, der Prozesse zwischen Running, Ready, Blocked und den Suspended-Prozessen schaltet

## Long Term Scheduling
Der Teil des Scheduler, der Prozesse auch von und in den New und Exit-Zustand schalten kann


#Betriebssysteme 