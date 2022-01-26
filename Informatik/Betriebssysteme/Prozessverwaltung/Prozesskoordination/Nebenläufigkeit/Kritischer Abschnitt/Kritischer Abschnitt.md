# Beschreibung
Es gibt Ressourcen, die als ganzes oder bzgl. einzelner Operationen nur exklusiv, d.h. zu einem Zeitpunkt nur durch einen einzigen [[Thread]] (oder beim [[Multiprocessing]]: [[Prozess]])  nutzbar sind. (z.B. Das Bankkonto im Beispiel der [[Race Condition]])

Die Phase (= Teil eines [[Programm]]), in der ein Prozess auf exklusive Ressourcen zugreift, wird als **Kritischer Bereich** bezeichnet.

Ein Kritischer Bereich ist also die Phase, bei der auf eine globale Variable zugegriffen wird.


Kritische Bereiche erfordern [[Wechselseitiger Ausschluss|Wechselseitigen Ausschluss]] konkurrierender Prozesse.


# Gefahren
Durch den Ausschluss von Prozessen können [[Verklemmung|Verklemmungen]] entstehen.

# Lösung
Ein Kritischer Bereich kann nur entstehen, wenn beide Prozesse [[Unabhängige und Abhängige Abläufe|abhängig]] und [[Parallelität|parallel]] (also [[Nebenläufigkeit|nebenläufig]]) sind.

- Parallelität kann man durch [[Scheduler|Preemptives Scheduling]] verhindern
- Abhängigkeit verhindert man durch Einsatz eines [[Ringpuffer]]


# Beispiel 
## Beispiel für wechselseitigen Ausschluss
![[Kritischer Abschnitt Beispiel.png]]



#Betriebssysteme 