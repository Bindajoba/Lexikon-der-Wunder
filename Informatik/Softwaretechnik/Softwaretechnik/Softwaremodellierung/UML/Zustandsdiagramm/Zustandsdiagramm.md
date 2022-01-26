TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Ein Zustandsautomat ist ein [[Automat]], welcher die Zustände und Zustandsübergänge eines [[Objektdiagramm|Objekts]] beschreibt. Sie sind ein Teil der [[UML]]

Q: Wofür wird ein Zustandsdiagramm verwendet?
A: Zur Beschreibung der Zustände und Zustandsänderungen eines Objekts
<!--ID: 1641730455244-->


# Syntax
## Transition
Eine Transition (d.h. Zustandsübergang) wird durch einen Pfeil dargstellt. Der Pfeil ist mit einem **Trigger** beschriftet. Durch auslösen des **Triggers**, wird die Transition ausgelöst.
Die Trigger werden üblicherweise in der Syntax **Ereignis(Parameterliste)[Bedingung]** beschrieben.

![[Zustandsdiagramm Transition.png]]

## Verzweigung
Verzweigungen werden üblicherweise durch Angabe einer Bedingung in der eckigen Klammer realisiert. 
Man kann Verzweigungen statisch oder dynamisch implementieren.
- **Statische Verzweigungen** werden durch einen ausgefüllten Üunkt dargestellt. Hier wird davon ausgegangen, dass die Bedingung vor Ausführung der Transition bereits berechnet vorliegt.
- **Dynamische Verzweigungen** werden durch einen unausgefüllten Kreis dargestellt. Hier wird nicht davon ausgegangen, dass Bedingung berets berechnet vorliegt. Sie wird berechnet, wenn die Transition eintritt. 
*Der leere Kreis symbolisiert wohl, dass man kurz auf der Transition stehen bleibt.*


![[Zustandsdiagramm Verzeung.png]]![[Zustandsdiagramm Verzweigung II.png]]

## Atomare Aktivitäten
Mit jeder Transition oder in jeden Zustand können atomare Aktivitäten ausgeführt werden.
Diese werden mit einem Schrägstrich an das Ereignis angehängt.
Es wird angenommen, dass Atomare Transitionen keine Zeit in Anspruch nehmen und nicht unterbrechbar sind.

Man kann Schlüsselwörter verwenden um zu spezifizieren, wann Aktivitäten in einem Zustand ausgeführt werden.
- do / : Im Widerspruch zum vorher gesagten, braucht diese Aktivität Zeit in Anspruch, kann aber nicht unterbrochen werden.
- entry / : Wird ausgeführt, wenn der Automat in den Zustand kommt
- exit / : Wird ausgeführt, wenn der Automat den Zustand verlässt

![[Zustandsdiagramm Aktivität.png]]   

## Hierarchische Zustände
Jeder Zustand kann eine beliebige Zahl von Unterzuständen haben.
Wechselt ein Zustand in den Oberzustand, dann ist der nächste Zustand der Teilzustand im Oberzustand, der durch einen Start bezeichnet ist.
Wird die Transition ausgelöst, die aus dem Oberzustand herausführt, dann wird das getan, egal in welchem Teilzustand das Objekt sich gerade befindet.
Gelangt der Unterautomat in einen Endzustand, dann wird die automatische Transition des Oberzustands ausgeführt.

![[Zustandsdiagramm Unterzustände.png]]

## Stümpfe
Will man nicht den ganzen Unterautomaten zeichnen, obwohl es Transitionen gibt, die zu speziellen Unterzuständen wechseln, kann man dies durch Stümpfe symbolisieren:
![[Zustandsdiagramm Stumpf.png]]

## History-Zustand
Manchmal muss die Aktuelle Aktivität unterbrochen werden und durch eine wichtigere Aktivität ersetzt werden.
Man soll dann da in die vorherige Aktivität zurückkehren, wo man aufgehört hat.
Dazu wird ein Histrory-Zustand verwendet. Verlässt man einen gebündelten Zustand, und tritt dann wieder in ihn ein, dann merkt sich (bei Anwesenheit des History-Zustands) der gebündelte Zustand, wo er herausgesprungen ist.

![[Zustandsdiagramm Historyzustand.png]]

## Nebenläufigkeit
Manchmal kann ein Objekt durch zwei [[Nebenläufigkeit|nebenläufige]] Automaten beschrieben werden. In UML wird das so dargestellt:
![[Zustandsdiagramm Nebenläufigkeit.png]]

#Softwaretechnik 


