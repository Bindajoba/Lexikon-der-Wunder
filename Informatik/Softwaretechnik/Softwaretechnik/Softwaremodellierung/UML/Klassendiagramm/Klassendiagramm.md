TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Ein Klassendiagramme ist ein [[Strukturdiagramm]] und der wichtigste Bestandteil der [[UML]].
lassendiagramme visualisieren eine Menge von Klassen und ihre Zusammenhänge. In den einzelnen Klassen werden Attribute und Operatoren gespeichert. Aber das ganze weiß ich schon aus der 5. Klasse.

Klassendiagramme dienen erst der groben Übersicht, sollten dann aber iterativ verfeinert werden, bis sich die Klassen automatisiert aus dem Diagramm generieren lässt (Dazu gibt es [[Software-Tool]], Mit solchen Tools kann man auch Code zu Klassendiagrammen machen).

# Varianten
Je nach Details und Programmierstand kann man zwischen verschiedenen Varianten eines Klassendiagramms unterscheiden:
- **Analyse-Klassendiagramm**, enthält
Klassenname
Verantwortlichkeiten der Klasse in Fließtext. (*Das erinnert mich sehr an die [[CRC-Karte]]*)
- **Entwurf-Klassendiagramm**, enthält
Klassenname, Attribute, Operationen
- **Implementierungs-Klassendiagramm**
Klassenname, Attribute, Operationen in vollstem Detail (Sichtbarkeit, Datentypen, ...)

Q: Was sind die Genauigkeitsstadien eines Klassendiagramms?
A: - Analyse-Klassendiagramm
- Entwurf-Klassendiagramm
- Implentierungs-Klassendiagramm
<!--ID: 1641730455600-->


# Syntax
![[Klassendiagramm Beispiel.png]]

## Grundlegendes
Ich weiß schon eine Menge zu Klassendiagrammen, daher notiere ich bloß die wichtigsten Sachen:
- Durch unterstreichen zeigt man an, dass ein Attribut statisch ist.

Q: Wie stellt man statische Attribute einer Klasse dar?
A: Durch Unterstreichen
<!--ID: 1641305255720-->

Q: Was ist die Syntax eines Attributs?
A: Name : String = "Alice"
<!--ID: 1641305981288-->


Q: Was ist die Syntax einer in-Methode?
A: methodeName(in eingabeName : eingabeTyp) : ausgabeTyp
<!--ID: 1641305981304-->


Q: Was bedeutet inout in einer Methode eines Klassendiagramms?
A: Die Eingabe wird bearbeitet.
<!--ID: 1641305981328-->


## Sichtbarkeit
- public wird mit - dargestellt
- protected wird mit # dargestellt
- private wird mit + dargestellt

Q: UML-Klassendiagrammsymbol für private?
A: -
<!--ID: 1641305981354-->


Q: UML-Klassendiagrammsymbol für protected?
A: #
<!--ID: 1641305981377-->


Q: UML-Klassendiagrammsymbol für public?
A: +
<!--ID: 1641305981393-->

## Assoziationen
Können [[Objektdiagramm|Objekte]] einer Klasse miteinander kommunizieren, so sind die Klassen miteinander assoziiert. Klassen können auch mehrfach assoziiert sein, was dann berücksichtigt werden sollte.
![[Klassendiagrammm Beispiel II.png]]

## Rolle
Bei einer Assoziation nehmen beide Klassen bestimmte **Rollen** an. Diese können so beschrieben werden:
![[Klassendiagramm Rolle.png]]
Die Rollen treten später als Attributnamen in einer Klasse auf und sind daher interessant.

# Richtungen
Assoziationen zwischen Klassen können je nach Anforderung Uni- oder Bidiraktional stattfinden.
![[Klassendiagramm Bidirektional.png]]
*Dies zeigt ein Beispiel aus Monopoly. Jeder Spieler weiß, welche Straßen er besitzt. Damit man aber weiß, an wen man die Miete bezahlen muss, weiß auch jede Straße, wer ihr Besitzer ist.*

![[Klassendiagramm Unidirektional.png]]
*Wieder ein Beispiel aus Monopoly. Die Straße muss nicht wissen, wer auf ihr steht, und so muss sie nie auf den Spieler zugreifen. Das spiegelt sich im Klassendiagramm.*

Sind keine Pfeile vorhanden, dann ist die Richtung nicht festgelegt.

## Komposition
Komposition Modelliert eine "besitzt"/"besteht aus"-Beziehung. Es wird durch eine schwarze Raute dargestellt. Die Objekte sind miteinander verknüpft und sollten die gleiche Lebensdauer haben (gleichzeitig entstehen und gelöscht werden)
Daher empfielt es sich die Objektreferenz im Konstruktur der Oberklasse zu erzeugen.
![[Klassendiagramm Komposition.png]]

## Aggregation
Aggregation ist eine Verallgemeinerung der Komposition. Ein Objekt kann ein oder mehrere Aggregate besitzen, von denen es ein Teilobjekt ist.
Der Unterschied zur Komposition ist, dass ein Objekt Teil mehrere Aggegate sein kann. Bei der Komposition hingegen kann das Objekt nur Teil einer Sache sein.
![[Klassendiagramm Aggregat.png]]

## Multiplizität
Wie viele Objekte in einer Beziehung stehen, wird durch eine Zahl über den Enden der Assoziation dargestellt. (vgl. [[Multiplizität]])
![[Klassendiagramm Multiplizität.png]]
*Der Stern steht für beliebig viele Objekte (0 eingeschlossen).*

## Assoziationsklasse
An einem Monopolyspiel können bis zu 6 Spieler teilnehmen. Ein Spieler kann beliebig viele Monopolyspiele gleichzeitig spielen.
Ein Spieler hat aber in jedem Spiel einen unterschiedlichen Kontostand, unterschiedliche Straße, unterschiedliche Position, etc. 
Daher wird der Verknüpfung selbst eine Klasse zugeordnet. Diese Klasse kann selbst in Beziehung zu anderen Klassen stehen.

![[Klassendiagramm Assoziationsklasse.png]]

## Ternäre Operationen
Sind in einer Assoziation mehr als zwei Objekte beteiligt, dann kann man diese durch eine Raute verbinden. Das hat aber in Objektorientierten Programmen schwer umzusetzen und sollte daher nur zur Modellierung von Datenbeständen verwendet werden. 

## Vererbung und Abstrakte Klasse
![[Klassendiagramm Vererbung.png]]
Vererbung werden durch einen solchen Pfeil dargestellt. Abstrakte Klassen und die abstrakten Methoden werden Kursiv geschrieben.

## Interfaces
Interfaces sind abstrakte Klassen ohne Attribute und nur mit abstrakten Operationen.
Es gibt zwei Möglichkeiten sie darzustellen:
![[Klassendiagramm Interface.png]] ![[Klassendiagramm Interface II.png]]

# Umsetzung und Java
## Attribute
Attribute einer Klassenkarte werden als Variablen der Klasse implementiert. Die Variable erhält die Sichtbarkeit, den Datentyp und den Initialisierungswert des Attributs.

## Operationen
Operationen einer Klassenkarte werden als Methoden der Klasse implementiert. Die Methode erhält Eingabeparameter und Rückgaben der Operation.

## Interfaces
Für ein Interface im Klassendiagramm wird eine Interface-Klasse mit dem selben Namen erstellt. Operationen in der Karte des Interfaces werden als abstrakte Methoden in der Interface-Klasse implementiert.

## Generalisierungen
Eine Generalisierung einer Klasse wird in Java durch extends umgesetzt.

## Assoziationen
Die Implementation von Assoziationen zwischen einer Klasse A und einer Klasse B ist je nach  Multiplizität etwas anders:
- 1:1: Ein Objekt aus Klasse A referenziert ein Objekt aus Klasse B (oder umgekehrt, das ist von der Direktionalität abhängig. Bei Bidirektionalität referenzieren sich die Klassen gegenseitig)
- 1:n: Ein Objekt aus Klasse hat eine Containerobjekt (wie Array), mit der n-Objekte aus B referenziert werden können
- n:m: Eine Umsetzungsmöglichkeit ist dass A und B ein Containerobjekt haben.
Alternativ kann man (wie in Datenbanken üblich) eine Verknüpfungsklasse erzeugen, die eine Menge alle 1:1-Beziehungen ist, die durch die ursprüngliche n:m-Beziehung erzeugt werden.
A und B referenzieren dann diese Verknüpfungsklasse.
Jede dieser 1:1-Verknüpfungen kann als ein Objekt einer Verknüpfungsklasse modelliert werden. So erhält man die Implementation einer Verknüpfungsklasse.

## Aggregationen
Ich denke, Aggrationen sind nicht wirklich mit Java implementierbar. 
Vielleicht ist aber eine einfache Referenz in Sinne einer Objekt A hat Objekt B schon ausreichend.

## Komposition
Eine Komposition lässt sich als Referenz eines Objekts a:A auf ein Objekt b:B implementieren.
Da bei einer Komposition b:B ein fester Bestandteil von a:A sein soll, sollen sie die gleiche Lebenszeit haben.
Dies wird bewirkt, indem b:B im Konstruktor von a:A erstellt wird.



#Softwaretechnik 


