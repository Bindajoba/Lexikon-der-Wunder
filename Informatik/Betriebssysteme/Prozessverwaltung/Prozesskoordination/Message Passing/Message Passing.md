TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Prozesskoordination erfordert Synchronisation und Kommunikation. Diese soll mittels Message Passing, d.h. Nachrichtentausch realisiert werden.

Für den Nachrichtenaustausch werden zwei Primitive genutzt:
- send(destination, message)
- receive(source, message)

Q: Welche zwei Primitive werden für Message Passing verwendet? ([[Message Passing]])
A: - send(destination, message)
- receive(source, message)


# Linnhoff-Visualisierung
Die Primitive kann man sich so vorstellen.
Bei send(...) schickt der Sender einen Brief mit einer Nachricht (**message**) an eine Adresse (**destination**)

receive(...) wird vom Empfänger aufgerufen. 
Bei receive() gibt es meinerseits Unklarheit:
-  Der Empfänger sieht in den Briefkasten (**source**) sieht nach, ob ein Brief (**message**) angekommen ist und nimmt in dann heraus. 
*Diese Interpretation scheint mir die sinnvollste zu sein*
-  Der Empfänger wartet auf einen Brief im Briefkasten (source), wenn einer ankommt, dann wird dieser gelesen.

Was bedeutet message bei receive(...)? Ich denke, das beschreibt die Methode, in der die Nachricht gespeichert werden soll.


# Blockierung
*Damit Nachrichten zeitlich korrekt abgestimmt sein, müssen evtl. Prozesse blockiert werden*. Dass kann auf 3 Arten geschehen:

Q: Welche 3 grundlegenden Arten gibt es Message-Passing umzusetzen?
A: - Blocking Send, Blocking Receive
- Nonblocking Send, Blocking Receive
- Nonblocking Receive-Ansätze

## Blocking Send, Blocking Receive
Sendender Prozess wird blockiert, bis die Nachricht beim Empfänger angekommen ist.
Empfangender Prozess wird nach einem receive-Aufruf blockiert, bis eine Nachricht kommt.
-> Ineffizient (Warum sollte ein Sender warten, bis ein Brief in den USA ankommt?)

## Nonblocking Send, Blocking Receive
Sendender Prozess wird ganz kurz blockiert, damit er problemlos die Nachricht abschicken kann
Empfangender Prozess wird nach einem receive-Aufruf blockiert, bis eine Nachricht kommt.

*Mein Verständnis: Der Empfänger bleibt am Briefkasten stehen, um auf die Nachricht zu warten.*

## Nonblocking Receive-Ansätze
- **Mit Puffer, Mit Blockierung**
Schlechter Ansatz behandeln wir nicht
- **Ohne Puffer, Ohne Blockierung**
Geht nicht, Nachrichten gehen verloren, man erhält [[Verklemmung]] 
- **Ohne Puffer, Mit Blockierung**
Ich denke, das heißt der Empfänger ist blockiert im Sinne dass er wartet, bis die Nachricht da ist. Wenn der Brief ankommt, wird der benutzt.
- **Mit Puffer, Ohne Blockierung**
Der Brief kann für längere Zeit im Briefkasten bleiben. So kann der Empfänger einfach reinschauen, wann er Lust hat.

Q: Welche sinnvollen Nonblocking Receive-Ansätze gibt es für das [[Message Passing]]
A: - Ohne Puffer, Mit Blockierung
- Mit Puffer, Ohne Blockierung

# Adressierung
Wie werden Adressen an bestimmte Orte/Speicher/Prozesse formuliert und wohin sollen sie gesendet werden?
Siehe dazu [[Adressierung]]



#Betriebssysteme 


