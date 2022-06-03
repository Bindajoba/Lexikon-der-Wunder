TARGET DECK: Universität::MaDid III

# Beschreibung
Experimente, die als Kombination mehrerer (einfacher) Zufallsexperimente modelliert werden können.

Der Ergebnisraum ist eine Teilmenge des kartesischen Produkts der Ergebnisräume der Teilexperimente


# Darstellung des Wahrscheinlichkeitsraums
- Tabelle (z.B. Würfeln mit zwei Würfeln)
- Baumdiagramm (man kann Pfadregen anwenden, Mehrstufigkeit wird sichtbar)

Q: Wie kann mna den Wahrscheinlichkeitsraum eines mehrstufigen Experiments darstellen? ([[Mehrstufige Experimente]])
A: - Tabelle
- Baumdiagramm
<!--ID: 1645282095106-->


# Pfadregeln
## 1. Pfadregel
Die Wahrscheinlichkeit eines Pfades ist gleich dem Produkt der Wahrscheinlichkeiten entlang dieses Pfades.
Folgt in der Hochschule aus den bedingten Wahrscheinlichkeiten (in der Schule andersherum).

Q: Was ist die 1.Pfadregel ([[Mehrstufige Experimente]])
A: Die Wahrscheinlichkeit eines Pfades ist gleich dem Produkt der Wahrscheinlichkeiten entlang dieses Pfades.
<!--ID: 1645282095211-->


In der Schule kann man diesen wie folgt zeigen:
Q: Mit welchen Methoden kann man die Erste Pfadregel belegen? ([[Mehrstufige Experimente]]).
A: - Laplace Aspekt
- Chancenaspekt
- Frequentistisch/Natürliche Wahrscheinlichkeiten
<!--ID: 1645282095314-->


### Laplace Aspekt
Man zeichnet den Baum auf aber statt der Wahrscheinlicheit trägt man die Möglichkeitszahl auf, mit der ein Ergebnis auftreten kann. (z.B. drei rote kugeln in der Urne, wie viele Möglichkeiten gibt es, zwei zu ziehen? Für die erste rote 3, für die zweite 2, also insgesamt 6. Ebenso kann man die Möglichkeiten insgesamt multiplizieren)
![[Mehrstufige Experimente Pfadregel.png]]
*Laplace-Argumentation ist fachlich etwas schwach, das Bruchrechnen ergibt nicht ganz so viel sinn. Es ist auch bei macnchen Aufgaben gefährlich, zum Beispiel wenn die Wahrscheinlichkeiten in zweiten Baum unterschiedlich sind, weil sie vom ersten Ergebnis abhängen.*

Siehe auch [[Wahrscheinlichkeitsbegriff (Didaktik)#Zugänge zum Wahrscheinlichkeitsbegriff|Laplace Aspekt]].

### Chancenbetrachtung
Die Gesamtwahrscheinlihckeit 100% wird verteilt. 2/5 ist die Wahrscheinlichkeit, dass zuerst ein "r" gezogen wird. Von diesen 2/5 Chancen entfallen "3/4" auf den Fall, dass als zweites ein "e" gezogen wird
3/4 von 2/5 sind $\frac{3}{4} \cdot \frac{2}{5}$ (Setzt den von-Ansatz voraus)
*Kaum an konrete Situationsvorstellungen anzubinden*

### Frequentistisch/Natürliche Wahrscheinlichkeiten
Wir probieren das Experiment 10000 mal
Ein etwa 2/5 Versuche, d.h. 4000 werden wir zuerst ein r ziehen
Von diesen werden bei 4/5 ein e ziehen (das sind 3000)
Insgesamt werden wir bei $3/4*2/5*10000$ re ziehen, das sind $6/20$ der Fälle
*Fördert vielleicht die Fehlvorstellung des Outcome-Approuch oder des [[Empirisches Gesetz der Großen Zahlen]], es werden genau 4000 re herauskommen.*


## 2. Pfadregel
Die Wahrscheinlichkeit eines Ereignisses ist gleich der Summe der Wahrscheinlichkeiten der für dieses Ereignis günstigen Pfade.

Q: Was ist die 2. Pfadregel ([[Mehrstufige Experimente]])
A: Die Wahrscheinlichkeit eines Ereignisses ist gleich der Summe der Wahrscheinlichkeiten der für dieses Ereignis günstigen Pfade.
<!--ID: 1645282095420-->


# Beispiele
## Einführungsbeispiel
![[Mehrstufige Experiemente Einführung.png]]
Dieses Beispiel behandelt zwei verschiedene Experimente hintereinander (Würfel ziehen, Würfel werfen) und macht damit transparent, dass ein Konzept benötigt wird, mit dem man Wahrscheinlichkeiten von mehrstufigen Experimenten berechnen kann.

Des Weiteren ist die Aufgabe nicht ohne Weiteres nur mit vorherigen Konzepten lösbar.
Es erfüllt also die zwei wichtigen Bedingungen eines [[Einführungsbeispiel]]

## Beispiel 1
Zwei mal ziehen aus einem Beutel ohne Zurücklegen

## Wegenetz
![[Mehrstufige Experimente Wegenetz.png]]
# Übungen
## Klausur 2020 Aufgabe 10
![[Klausur 2020 Aufgabe 10.png]]
Korrekt sind i, ii.

*Wie lustig ist denn diese Aufgabe! Man kann sagen, ich gewinne, wenn ich zwei mal die gleiche Farbe ziehe (also die Wahrscheinlichkeit verdopple) und würde trotzdem verlieren!*
  


#Mathe-Didaktik-III 


