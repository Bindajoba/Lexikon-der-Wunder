## Beschreibung
Die Modellmaschine MI ist ein Modell eines Rechners mit einem [[Betriebssystem]], welcher Konzepte der Vorlesung illustrieren soll.

## Eigenschaften
### Register
MI verfügt über die Register 
- **PC** (Programmzähler)
- **SP** (Stack-Pointer, siehe [[Stack von MI]])
- **R0 bis R14**

Wobei **R12** und **R13** nicht frei genutzt werden dürfen, sondern spezielle Bedeutungen haben:
- R12 enthält die Ablageadresse des ersten Aufrufparameters/Arguments (p1).
- R13 enthält die Basisadresse des lokalen Datenraums des Unterprogramms

Die Register und Speicherzellen sind 4 Bytes breit. Daher schreitet der Befehlszähler nach jeden Befehl 4 Schritte nach vorne. 

### Sicherheit
Die Register der MI sind [[Callee-saved]], d.h. das aufgerufene Unterprogramm trägt die
Verantwortung dafür, dass der Kontext des Aufrufers (Caller) nach dem Rücksprung unverändert
dem Kontext vor dem Unterprogrammaufruf entspricht.

### Befehle
Siehe [[Befehle von MI]]

#Betriebssysteme 