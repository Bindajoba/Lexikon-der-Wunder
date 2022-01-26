TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Der Schedulingalgorithmus beschreibt, in welcher Reihenfolge [[Prozess|Prozesse]] ausgeführt werden sollen und bringt den [[Scheduler]] damit erst zum Leben.

# Anforderungen
- **Fairness**
Jeder Prozess sollte einen gerechten Anteil an Prozessorzeit bekommen
- **Policy Enforcement**
Das gewählte Verfahren wird ohne Ausnahmen stets durchgesetzt
- **Balance**
Alle Teile des Systems sind gleichmäßig ausgelastet
- **Datensicherheit**
Es können keine Daten oder Prozesse verloren gehen
- **Skalierbarkeit**
Die mittlere Leistung wird bei wachsender Last (Anzahl Prozesse) beibehalten. Es gibt keine Schwelle ab der das Scheduling sehr langsam oder gar nicht funktioniert
- **Effizienz**
Der Prozessor sollte immer vollständig ausgelastet sein

Q: Nenne 4 von 6 Anforderungen an einen Schedulingalgorithmus
A: - Fairness
- Policy Enforcement
- Balance
- Datensicherheit
- Skalierbarkeit
- Effizienz
<!--ID: 1642897215817-->



# Vergleich von Algorithmen 
Um Scheduling Algorithmen zu vergleichen, muss man einige Kenngrößen kennen.
Diese sind aber in den [[Schedulerkenngrößen]] besser aufgehoben.

Desweiteren gibt es noch mehr Aspekte, unter denen man Algorithmen vergleichen kann. Diese sind aber nicht ganz so wichtig. 

## Batch-Systeme
- Durchsatz
- Verweildauer
- Prozessorauslastung

## Interaktive Systeme
- Antwortzeit
- Verhältnismäßigkeit
- Interaktion

## Echtzeitsysteme
- Sollzeitpunkte
- Vorhersagbarkeit

# Algorithmen
- FIFO
- SPN
- SRPT
- RR
- PS


## Priorisierter FIFO
![[Schedulingalgorithmus.png]]
Die Prozesse werden in Warteschlangen gespeichert. Prozesse aus höheren [[Priorität|Prioritäten]] werden zuerst ausgeführt

Ein solcher Prozess hat aber das Problem, dass Prozesse mit niedriger Priorität verhungern könnten, falls ständig Prozesse mit höheren Prioritäten ausgeführt werden.

## First-Come-First-Served (FIFO)
First-Come-First-Served ist ein [[Scheduler|Nicht-Preemptiver-Scheduling-Algorithmus]]. Ein rechenbereiter Prozess stellt sich in den Ready-Queue einfach hinten an und bei frei werdendem Prozessor kann der jeweils älteste Prozess in den Zustand "running" überführt werden.

**Vorteile**
- Einfach zu Programmieren
- Fair

**Problem**: Wird ein langer Prozess vor einem kurzen Prozess ausgeführt, muss der kurze lange warten.

## Shortest Process Next (SPN) / Shortest Job First
Der kürzester Prozess wird als erstes ausgeführt.
So kann das Problem von FIFO behoben werden. Dadurch wird im Allgemeinen die Geschwindigkeit größer.

**Problem**: Wird erst mit einem großen Prozess begonnen und der kleine Prozess kommt verspätet nach, so muss der kleine Prozess trotzdem warten, bis der große fertig ist.
Das verschlechtert die Antwortzeit.

## Shortest Remaining Processing Time (SRPT)
Dieser Algorithmus löst das obere Problem, indem Prozesse unterbrochen werden dürfen um kleineren Prozessen den Vortritt zu lassen.
Es handelt sich also um ein **Preemptive-Scheduling-Algorithmus**.

**Problem**: Man kann nicht immer wissen, wie lange die Prozesse brauchen

## Round-Robin (RR)
Round-Robin nutzt uhrenbasierte Unterbrechungen. In periodischen Intervallen $Q$ (für Zeitquantum) werden Prozesse in ihrer Abarbeitung unterbrochen.

Die Prozesse werden der Reihe nach für eine kurze Zeitspanne bearbeitet. Kommt man beim letzten Programm an, fängt man wieder am Anfang an.

$Q$ sollte nicht zu klein und nicht zu groß sein. Ist $Q$ zu klein, ist das Dispatching zu aufwändig.
Ist $Q$ zu groß, wird Round Robin zu FIFO

Round Robis ist besser als FIFO aber schlechter als SRPT.
Round Robin ist prkatisch implementierbar und fair.

## Priority Scheduling (PS)
Jeder Prozess erhält ein Priorität. Die Abarbeitung bearbeitet Prozesse mit der Höchsten Priorität als allererstes

**Probleme**:
- Nicht fair
- Relativ schlechte Verweildauer

## Multilevel Feedback Queuing Algorithmus
Dieser Algorithmus verbindet Ideen vom Priority Scheduling und vom Round Robin.

Es gibt für jede Priorität (bis n) eine Warteschlange.

Als erstes wird der Prozess mit der höchsten Priorität bearbeitet. Wird dieser nicht innerhalb eines Zeitquantums beendet, suspendiert der Scheduler den Prozess, verringert seine Priorität und reiht ihn hinten in die Warteschlange der schwächeren Priorität ein.

Dann wird wieder ein Zeitquantum des Programms in der höchsten Prioritätenschlange verarbeitet.

Kommt ein Programm in der untersten Schlange, d.h. in der schwächsten Priorität an, wird es dort nach Round-Robin durchgearbeitet.
