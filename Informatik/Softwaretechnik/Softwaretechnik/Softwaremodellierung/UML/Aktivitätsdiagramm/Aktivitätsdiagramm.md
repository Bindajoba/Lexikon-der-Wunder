TARGET DECK: Universität::Informatik::SWT

# Beschreibung
**Aktivitätsdiagramme** eignen sich zu Beschreibung von Abläufen. Es handelt sich um ein [[Verhaltensdiagramm]] und ist ein Teil von [[UML]]

Q: Wofür wird ein Aktivitätsdiagramm verwendet
A: Zur Beschreibung von Aktivitäten
<!--ID: 1641388713911-->


# Syntax
In einem Aktivitätsdiagramm werden die Aktionen in abgerundete Rechtecke geschrieben und durch Pfeile verbunden.

## Start- und Endknoten
Startknoten werden wie in einem [[Zustandsdiagramm]] durch einen ausgefüllten Kreis dargestellt.
Ein Endknoten mündet in ein Spiegelei.

Q: Wie wird ein Startknoten in einem [[Aktivitätsdiagramm]] dargestellt?
A: Ein ausgefüllter Kreis, aus dem ein Pfeil kommt
<!--ID: 1645543049116-->


Q: WIe wird ein Endknoten in einem [[Aktivitätsdiagramm]] dargestellt?
A: Ein Spiegelei
<!--ID: 1645543049231-->



## Bedingungen
Bedingungen werden in Eckigen Klammern über die Kanten geschrieben.
![[Aktivitätsdiagramm Bedingung.png]]
Will man Bedingungen schachteln, kann man "Entscheidungsknoten" in Form einer Raute hinzufügen:
![[Aktivitätsdiagramm Bedingung II.png]]

Q: Wie wird ein Entscheidungsknoten in einem [[Aktivitätsdiagramm]] dargestellt
A: Durch eine Raute 
(Entscheidungen in eckigen Klammern)
<!--ID: 1645543049357-->



## Nicht-disjunkte Bedingungen
Sind die Bedingungen nicht disjunkt, das heißt, es können mehrere Bedingungen gleichzeitig auftreten, dann wird das mit einem Synchronisationsbalken verdeutlicht. 
Ein Synchronisationsbalken erzeugt parallele Abläufe oder synchronisiert die Eingänge, in dem er darauf wartet, dass alle Eingänge bei ihm ankommen, bevor die Aktivität fortgeführt wird.
![[Aktivitätsdiagramm Synchronisation.png]]
*Ich verstehe nicht, was in dem Beispiel synchronisiert wird aber so sehen die Balken aus.*

## Verantwortungsbereiche
Eine Aktivität kann zwischen Objekten hin und her springen. Um darzustellen, wer gerade für die Ausführung der Aktivität verantwortlich ist, kann man **Verantwortungsbereiche** nutzen.
![[Aktivitätsdiagramm Verantwortungsbereich.png]]

## Weiterleiten von Objekten
Eine Kante kann Objekte weiterleiten. *Zum Beispiel wird vooberen Entscheidungsknoten Geld an Straße aushändigen weitergegeben.*
Die mitgegebenen Objekte werden durch Rechtecke dargestellt.

![[Aktivitätsdiagramm Weiterleiten von bjekte.png]]

## Geschachtelte Aktivitäten
Jede Aktion (also jeder Knoten) kann sich wieder als Aktivität beschreiben lassen. Wir können also in einen Knoten einen neuen [[Graph|Graphen]] zeichnen. Wir benutzen ein Gabelsymbol, um das zu verdeutlichen.

![[Aktivitätsdiagramm Verschachtelung.png]]

#Softwaretechnik 


