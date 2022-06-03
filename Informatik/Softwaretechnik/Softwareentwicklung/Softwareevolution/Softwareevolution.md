TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Software wird meistens nicht von null an begonnen. Oft wird ein altes Projekt verwendet, verbessert oder angepasst.
In dem Fall müssen andere Methoden als bei der Softwareerstellung verwendet werden.
Es gibt wahrscheinlich feine Unterschiede zur [[Softwarewartung]]. Ich kenne sie aber nicht.
Softwareevolution umfasst [[Softwarewartung]], Pflege und Weiterentwicklung.

# Definition
Softwareevolution umfasst alle Aktivitäten in der Erstentwicklung und Weiterentwicklung eines Softwaresystems im Rahmen der Wartung und Pflege über lange Zeiträume.

*Wahrscheinlich findet Softwareevolution nach der [[Projektabnahme]] und vor dem [[Projektabschluss]] statt.*

Q: Wie ist Softwareevolution definiert? ([[Softwareevolution]])
A: Softwareevolution umfasst alle Aktivitäten in der Erstentwicklung und Weiterentwicklung eines Softwaresystems im Rahmen der Wartung und Pflege über lange Zeiträume.
<!--ID: 1645543053258-->


# Lehmans Gesetze
Die daaligen IBM-Mitarbeiter haben einige Gesetzmäßigkeiten der Softwareevolution zusammengestellt:
- **Anhaltender Wandel** (Continuing Change)
Ein System, das über einen längeren Zeitraum verwendet wird, unterliegt kontinuierlichen Veränderungen oder verliert an Effektivität, weshalb eine kontinuierliche Anpassung und Weiterentwicklung unverzichtbar ist.
- **Zunehmende Komplexität** (Increasing Complexity)
Ein Softwaresystem, das ständig geändert wird, verliert langsam an Struktur
- **Selbstregulierung** (Self Regulation)
Übergreifende Prozesse der Evolution von Softwaresystemen sind übglicher weise selbstreguierend (?)
- **Konservierung der organisatorischen Stabilität** (Conservation of Organizational Stablity)
Obwohl entsprechende Feedback-Mechanismen implementiert und an den Erfordernissen ausgerichtet sind, neigt die durchschnittliche effektive Tätigkeit hinsichtlich derWartung und Pflege im Evolutionsprozess über den gesamten Lebenszyklus hin konstant gering zu sein
- **Konservierung der Benutzbarkeit**
Während der Evolution müssen alle Stakeholder weiterhin in der Lage sein, das System effizient und effektiv zu nutzen. 
- **Kontinuierliches Wachstum**
Der funktionale Umfang einer Software muss erweitert werden, um die Zufriedenheit ders Nutzers zu gewährleisten
- **Schwindende Qualität**
Qualität sinkt tendentiell
- **Feedback**
Alle Prozesse, die im Rahmen derWartung und Pflege eines Softwaresystems implementiert werden, sind als Multi-Level, Multi-Loop und Multi-Agent Feedback-System zu verstehen.

# Techniken der Evolution
## Architecture Governance
Kapier ich nicht

## Reengineerung
Anpassung eines Softwaresystems mit dem primären Ziel der Qualitätsverbesserung. (Wie eine Renovierung)

Q: Was ist Reengineering? ([[Softwareevolution]])
A: Renovierung eines Softwaresystems mit dem Ziel einer Qualitätsverbesserung
<!--ID: 1645543053385-->



### Forward Engineering
Reverse Engineering beschreibt den Prozess von hoher zu niedriger Abstraktionsstufe arbeiten.

## Reverse Engineerung
Die Analyse eines Systems, indem man sein Verhalten untersucht.
Q: Was ist Reverse Engineering? ([[Softwareevolution]])
A: Man versucht auf die Struktur eines Programms zu schließen, indem man sein Verhalten untersucht.
<!--ID: 1645543053529-->


## Refactoring
Siehe [[Refactoring]].

## Program Comprehension
Q: Was ist Program Comprehension ([[Softwareevolution]])
A: Program Comprehension beschreibt den Prozess, den Code zu verstehen.
<!--ID: 1645543053664-->


## Clone Detection
Q: Was ist Clone Detection? ([[Softwareevolution]])
A: Die Erkennung von ähnlichen Code-Passagen.
<!--ID: 1645543053811-->


*Hierfür kann man automatisierte Werkzeuge nutzen.*






#Softwaretechnik 