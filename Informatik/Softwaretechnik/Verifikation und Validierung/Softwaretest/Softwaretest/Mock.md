# Beschreibung
Will man einen Programmteil [[Software-Test|testen]], der Daten von komplizierten und ungetesteten Klassen empfängt, ist es sinnvoll die anderen Klassen durch einen **Mock** (engl. für Atrappe) zu erstzen.

Der Mock ist ein Platzhalter, der (üblicherweise) default-Werte ausgibt. So können sich Bugs der vorherigen Klasse nicht auf die getestete Klasse auswirken.

# Software Tools
Es gibt [[Software-Tool|Software-Tools]], die das Erstellen von Mocks automatisieren. Dazu gehören:
- Mockito
- JMock
- EasyMock


#Softwaretechnik 