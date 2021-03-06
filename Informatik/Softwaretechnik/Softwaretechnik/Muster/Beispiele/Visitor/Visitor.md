TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Der Besucher ist ein [[Entwurfsmuster (Softwaretechnik)]]. Der Besucher ermöglicht die Definition einer neuen Operation, ohne die Klassen der von ihr bearbeiteten Elemente zu verändern.

Q: Wozu verwendet man das [[Visitor]]-Entwurfmuster?
A: Man kann damit einer Klasse eine neue Operation hinzufügen, ohne die Klasse zu verändern.
<!--ID: 1645454018579-->

Für mehr Informationen[^1]

# Struktur
Ich gabe mein bestes, um das zu erklären:
Jedes Mal, wenn wir einer Klasse (z.B. Node) eine neue Operation hinzufügen wollen, ohne die Klasse zu verändern, erstellen wir stattdessen einen Visitor.

![[Visitorobjekt.png]]


![[Visitor Node.png]]

![[Visitor Prozess.png]]
Ein Element wird gefragt, ob es einen Visitor annehmen darf. Nimmt das Element an, dann übergibt es sich selbt dem Visitor. Dieser kann das Element nach belieben verändern.
So hat man eine Operation auf einem Element defininiert, ohne diese in das Element selbst zu schreiben.


#Softwaretechnik 


[^1]: https://refactoring.guru/design-patterns/visitor