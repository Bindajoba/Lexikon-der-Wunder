TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Model-View-Controller ist ein Interaktion-[[Architekturmuster]].

# Struktur
Das System wird in drei Komponenten aufgeteilt: 
- Datenmodell (Model)
- Präsentation (View)
- Steuerung (Controller)

![[MVC Struktur I.png]]
![[MVC Struktur II.png]]
Dieses MVC ist etwas anders, als ich es aus dem SEP kenne. Diese View kann nämlich Daten aus dem Controller anfragen.


# Übungen
## Übung SWT 13-3
Wie verhalten sich die Maße Kohäsion und Kopplung für eine monolithische Applikation
(d. h. ohne Aufteilung nach Verantwortlichkeit) und eine Applikation nach Model-View-
Controller-Architekturmuster?

In einer monolythischen Applikation ist die Kohäsion niedrig, da vermutlich viele verschiedene Aufgaben erledigt werden.
Eine Applikation nach Modell-View-Controller hat eine hohe Kohäsion, da jedes Modul das tut, wofür es geschaffen wurde und niedrige Kopplung, da nur dann auf andere Modeule (Controller/Viewer/Model) zugegriffen wird, wenn es wirklich nötig ist.

Skizzieren Sie die Struktur des MVC-Architekturmusters. Geben Sie den zeitlichen Ablauf
der Kommunikation zwischen den Komponenten an. Als Startpunkt können Sie von einer
Interaktion des Benutzers mit der Benutzeroberfläche ausgehen.

Welche Vorteile ergeben sich durch die Verwendung von MVC?
- Die Verarbeiteung der Daten, die Kontrolle und die Darstellung sind voneinander getrennt.

#Softwaretechnik 