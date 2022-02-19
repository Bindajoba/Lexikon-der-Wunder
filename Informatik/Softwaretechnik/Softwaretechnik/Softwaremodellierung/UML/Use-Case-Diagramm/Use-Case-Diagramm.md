TARGET DECK: Universität::Informatik::SWT

# Beschreibung
**Use-Case-Diagramme** erfassen die Anforderungen und spezifiziern damit die Funktionalität, die die Software erfüllen soll.

Konkret beschreibt es, welche Benutzer ein System hatund welche Interaktionen (**Anwendungsfall** genannt) diese mit dem System haben können.[^1]
Das Use-Case soll nur einen groben Überblick geben. Die Interaktionen selbst werden durch andere Diagramme, wie dem [[Aktivitätsdiagramm]] spezifiziert.

*Es ist ein [[Verhaltensdiagramm]] und Teil der [[UML]].*

Q: Was beschreibt ein Anwendungsfall?
A: Ein Anwendungsfall beschreibt eine typische Interaktion, die ein Akteur mit dem System hat
<!--ID: 1641730455361-->


Q: Welche Rolle spielen die [[Verhaltensdiagramm|Verhaltensdiagramme]] beim Verfeinern von Anwendungsfällen
A: Mit Verhaltensdiagrammen lassen sich Anwendungsfälle in kleine Schritte aufteilen. Dadurch soll die Implementierung klarer und es sollen zu verwendende Klassen erkannt werden.
<!--ID: 1641730455457-->



# Syntax
## Grundlagen
- Akteure werden durch Strichmännchen gekennzeichnet.
- Use-Cases/Anwendungsfälle werden durch Kreise gekennzeichnet.
- Assoziationen sind Linien zwischen Akteuren und Use-Cases
- User Generalisierungen werden durch Vererbungspfeile symbolisiert (wie im [[Klassendiagramm]])
![[Use-Case-Diagram Beispiel.png]]

## Multiplizität
Mit Multiplizität kann man angeben, wie viele Akteure an einem Anwendungsfall beteiligt sind.
![[Use-Case-Diagramm Multiplizität.png]]
*z.B.: Zwei Leute sind beim Zahlen einer Mite beteiligt.*

## Use-Case-Generalisierung
Use Cases können auch Vererbungsstrukturen haben. Ein Spielzug kann mehrere speziellere Formen annehmen.: Entweder man zahlt eine Miete oder kauft eine Straße.

![[Use-Case-Diagramm Generalisierung.png]]

## Use-Case-Abhängigkeiten (extends)
Use-Cases können um andere Use-Cases erweitert werden. Dies wird durch eine extends-Beziehung ausgedrückt. Dabei wird ein gestrichelter Pfeil verwendet.

![[Use-Case-Digramme.png]]
*Wenn man eine Straße kauft, kann man die Aktion durch das Aufnahmen einer Hypothek erweitern.*

## Use-Case-Abhängigkeiten (include)
Ruft ein Use-Case einen anderen immer auf, dan wird das durch eine include-Beziehung gekennzeichnet.
![[Use-Case-Diagramm includes.png]]
*Ein Spielzug beihnaltet immer ein Würfeln.*


[^1]: https://en.wikipedia.org/wiki/Use_case_diagram

#Softwaretechnik 





