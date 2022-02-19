TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Das Testen ist eine Methode der [[Software-Validierung]]. Das Programm wird ausgeführt und so auf Fehler getestet.
Ein Test ist dann gut, wenn er mit hoher Wahrscheinlichkeit einen Fehler aufdeckt

Q: Nenne zwei Gründe, die für Qualitätssicherung durch Testing sprechen.
A: - Man kann Fehler finden
- Indentifikation von Fehlern in der Interaktion zwischen Modulen
- Geringerer Aufwand als [[Manuelle Software Prüfung]]
- Automatisierbarkeit
- In Zukunft wiederholbar
<!--ID: 1642952241987-->

Q: Warum ist Testen allein für hohe Qualitätsansprüche nicht ausreichend?
A: - Man kann nicht die Korrektheit sondern nur die Inkorrekt zeigen
- Systeme mit hoher Kombinatorik können nicht erschöpfend getestet werden.
<!--ID: 1642952242108-->


# Grundsätze
Das Testen unterliegt 8 Grundsätzen.
Diese sollen beantworten, was Testen bewirkt, was Testen erfordert, was die Grenzen sind und was es für eine Rolle in der Softwareentwicklung innehat.:
1. Testen ist eine Maßnahme der analytischen Qualitätssicherung
2. Testen kann im Allgemeinen nicht die Korrektheit eines Programms zeigen, sondern nur die Inkorrektheit
3. Systematisches Testen erfordert eine genaue Beschreibung der Anforderungen
4. Systeme mit hoher Kombinatorik können nicht erschöpfend getestet werden
5. Testen geht mit Verfahren zur Fehleridentifikation und zur Fehlerbeseitigung einher
6. Testen kann bis zu 50% des Aufwandes einer Softwareentwicklung einnehmen
7. Tests prüfen nicht nur die Implementierung sondern auch die Grundannahmen
8. Testen erfordert in der Regel die Erstellung eines Testbetts, also einer Testumgebung, was sehr aufwendig sein kann

## Prinzipien
Zu den oben genannten Grundsätzen gibt es außerdem noch 5 Prinzipien des Testens. Diese beschreiben, was und in welcher Weise getestet wird:
1. Ein Entwickler sollte nicht den eigenen Code testen
2. Es ist immer davon auszugehen, dass der Code falsch ist
3. Die Testfälle müssen gültige und ungültige Eingaben umfassen
4. Die Ergebnisse eines Tests sind gründlich zu analysieren
5. Es sind keine ad-hoc "Wegwerf(test)fälle" zu verwenden (d.h. Test sollten nachhaltig in das System integriert werden)

# Fachbegriffe
- **Testabdeckung**



Q: Was ist Testabdeckung?
A: Der Anteil aller Code Teile, die durch eine Menge von Tests getestet werden.
<!--ID: 1643668651055-->


# Testprozess
Siehe [[Testprozess]]

## Entwurfsregel F.I.R.S.T.
Siehe [[Entwurfsregel F.I.R.S.T]]


# Testformen
## White-Box-Test
Testfälle werden aus dem Inneren also aus dem Code bestimmt. Testfälle werden so gewählt, dass jede Methode einmal ausgeführt wird.

Der White-Box-Test bietet sich damit nach der Fertigstellung einer Methode an

Q: Was ist der White-Box-Test?
A: Testfälle werden aus dem Inneren also aus dem Code bestimmt. Testfälle werden so gewählt, dass jede Methode einmal ausgeführt wird.
<!--ID: 1642952242228-->


## Gray-Box-Test
Eine Mittelding zwischen dem White und Black-Box-Test. Es werden nicht mehr einzelne Funktionen und auch nicht das ganze System sondern das Zusammenspiel der Module getestet.

Der Gray-Box Test bietet sich nach Fertigstellung eines Moduls an.

## Black-Box-Test
Testfälle ergeben sich von außen, d.h. aus den Anforderungsspezifikationen und den vom Programm angebotenen Schnittstellen.

Hier werden die üblichen Methoden des Testens angewandt: Randfälle, Hohe Zugriffszahlen, große Datenmengen, etc.

Q: Was ist ein Black-Box-Test? ([[Software-Test]])
A: Testfälle ergeben sich von außen, d.h. aus den Anforderungsspezifikationen und den vom Programm angebotenen Schnittstellen. 
<!--ID: 1642952242357-->


## Unit Test
Der [[Unit Test]] ist wahrscheinlich ein White-Box-Test.

## Regressionstest
Q: Was ist ein Regressionstest?
A: Wiederholte Testfälle bei Änderungen an Komponenten, um schnell Fehler zu bemerken.
<!--ID: 1643668651157-->

## Integrationstest
Siehe [[Integration]].

# Testmethoden
Beim Testen weren unterschiedliche Tricks angewendet.

## Äquivalenzklassen
Siehe [[Äquivalenzklasse (Softwaretest)]]

# Zusammenhänge
## Softwaremetriken
Durch [[Software-Metrik]] lassen sich die benötigten Tests gut abschätzen.
Je größer die [[LOC-Metrik]], desto mehr gibt es zu Testen.
Je größer die [[McCabe-Metrik|Zyklomatische Koplexität]], desto mehr Verzweigungen gibt es.





#Softwaretechnik 