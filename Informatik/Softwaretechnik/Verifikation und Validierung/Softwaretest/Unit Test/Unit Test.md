TARGET DECK: Universität::Informatik::SWT

 # Beschreibung
Ein **Unit Test** beschreibt einen (meist automatisierten) [[Software-Test|Test]], mit dem kleine Mengen Quellcode so früh und so oft wie möglich getestet werden.
Sie werden idealerweise während der Entwicklung entworfen.

Unit-Tests sind üblicherweise in einer eigenen Klasse ansässig.
Am Besten man spiegelt die Ordnerstruktur des Projekts für ein ProjektTest.
Die Klassen in dem ProjektTest haben den gleichen Namen, wie beim Projekt, nur das Test hinten angehängt wird.

Q: Was ist ein Unit-Test?
A: Ein **Unit Test** beschreibt einen (meist automatisierten) [[Software-Test|Test]], mit dem kleine Mengen Quellcode so früh und so oft wie möglich getestet werden.
<!--ID: 1642952241736-->


Q: Birgt es Gefahren, wenn eine Test-Suite ausschlißlich Unit-Test enthält.
A: Man testet damit die einzelnen Modulen, jedoch nicht ihre Interaktionen.
<!--ID: 1642952241889-->


# Entwicklung von Uni Tests
## Anwendung der F.I.R.S.T-Regeln
Siehe [[Entwurfsregel F.I.R.S.T]]

## Entwufskriterien nach Martin
Martin ist der Autor des Buches mit dem [[Sauberer Code]]. Er schlägt folgende Entwurfskriterien vor:
- One Assert per Test
Pro Test soll es nur ein Assert-Statement geben
- Single Concept per Test
Bei einem Test soll immer nur eine Sache gleichzeitig getestet werden. Das deckt sich gut mit dem [[Single-Responsibility-Prinzip]]

# Beispiel
## Test Kreisfläche
![[Unit Test Beispiel 1.1.png]]
![[Unit Test Beispiel 1.2.png]]

#Softwaretechnik 