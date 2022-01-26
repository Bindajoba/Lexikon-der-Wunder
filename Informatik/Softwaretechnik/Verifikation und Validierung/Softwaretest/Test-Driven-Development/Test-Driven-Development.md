# Beschreibung
**Test-Driven-Development** (kurz **TDD**) beschreibt einen Stil in der Softwareentwicklung, bei dem [[Software-Test|Tests]] im Mittelpunkt stehen.
Die Grundidee ist, dass das eigentliche Projekt (Produktivcode genannt) durch Tests auf Spezifikation und Funktion getestet werden kann.

Daher ist es sinnvoll erst die Tests zu schreiben und dann Code, der alle Tests besteht.

Ganz so einfach ist es nicht. Produktiv und Testcoe sollen trotzdem parallel zueinander geschrieben werden.

# Ablauf
![[Test-Dirven-Development Ablauf.png]]

# Regeln
Kent Beck hat 3 Regeln formuliert:
1. Schreibe keinen Produktivcode, solange du keinen Testfall erstellt hast, der fehlschlägt
2. Schreibe nicht mehr in einen Unit Test als benötigt wird, einen Test fehlschlagen zu lassen oder einen Compiler-Fehler zu erzeugen
3. Schreibe nicht mehr Produktivcode als erforderlich ist, um den fehlgeschlagenen Test erfolgreich zu bestehen

Die Regeln wirken sehr merkwürdig. Sie wollen aber sagen, dass man schnell zwischen Test und Produktivcode wechseln soll.
Man soll ein wenig Test schreiben. Dieser Test ist nun differenziert genug, dass er Fehler im Produktivcode findet. Diese werden ausgebessert, dann verbessert man wieder die Testumgebung, usw...

Ziel dieses Vorgehens ist es die Entwicklungs- und Testzyklen zu verkürzen.

## Implikationen
Das Test-Driven-Development hat einige Aspekte, die bei der Anwendung hervorkommen

- Perspektivwechsel
Der Programmierer setzt sich mit der Schnittstelle des Codes auseinander und wird dadurch zum Nutzer des Codes
- Testbarkeit
Der Produktivcode muss Testbar programmiert werden. D.h. die Schnittstellen müssen so gestaltet sein, dass man die Testumgebung drankoppeln kann.
- Dokumentation
Die Test müssen Schnittstellen von Modulen verwenden und eignen sich daher hervorragend, diese Schnittstellen zu verstehen. Neue Programmierer kann man dann einfach auf die Testumgebung verweisen.

#Softwaretechnik 