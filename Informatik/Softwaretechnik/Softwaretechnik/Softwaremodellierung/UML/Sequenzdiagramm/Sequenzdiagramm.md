TARGET DECK: Universität::Informatik::SWT

# Beschreibung
**Sequenzdiagramme** dienen der Beschreibung des Nachrichtenaustausches zwischen mehreren Objekten.

Q: Wofür benötigt man Seqenzdiagramme?
A: Zur Beschreibung des Nachrichtenaustausches zwischen mehreren Objekten
<!--ID: 1642761437289-->


# Zusammenhang zu Klassendiagrammen
Sind zwei Klassen eines [[Klassendiagramm]] mit einer Linie verbunden, so sind diese assoziiert, d.h. sie kommunizieren irgendwie miteinander. Jede dieser Kommunikationen lässt sich durch ein **Sequenzdiagramm** beschreiben.

# Syntax
Die Objekte werden mit ihrer Klassenbezeichnung in Rechtecken an die Spitze des Diagramms eingetragen. Im Gegensatz zu einem [[Objektdiagramm]] wird der Objektname nicht Unterstrichen.
Das ist wohl der Tatsache zuzuschreiben, dass die Objekte eher exemplarisch für das Verhalten einer Klasse sind.

Von den Rechtecken abwärts zieht man eine gerade, gestrichelte Linie. Diese Linie steht für den Lebenslinie des Objekts. Je weiter unten etwas steht, desto später passiert es.

Sequenzdiagrame werden mit benannt nd mit einem sd betitelt.

![[Sequenzdiagramm Beispiel.png]] 
Wie man erkennen kann, werden Anfragepfeile Schwarz und Antwortpfeile gestrichelt gezeichnet.

Q: Wie werden Objekte in Sequenzdiagrammen übertragen?
A: Durch die Form häuserBauen(Anzahl)
<!--ID: 1645260971659-->

Q: Wie wir eine Synchrone Nachricht in einem [[Sequenzdiagramm]] dargestellt?
A: Durchgezogener Pfeil mit ausgefülllter dreieckiger Pfeilspitze
<!--ID: 1645543047851-->


Q: Wie wird die Antwort eine synchronen Nachricht in einem [[Sequenzdiagramm]] dargestellt?
A: Gestrichelter Pfeil mit normaler Pfeilspitze
<!--ID: 1645543047972-->




## Aktivitätszonen
Aktivitätszonen werden durch schmale Rechtecke markiert. Sie verdeutlichen, die Zeit in der ein Objekt etwas tut.
Hat ein Objekt mehrere Aktivitätszonen gleichzeitig, dann kann das entweder heißen, dass zwei Aktivitäten gleichzeitig verlaufen oder dass die zweite Aktivität auf die Fertigstellung der ersten wartet.

![[Sequenzdiagramm Aktivitätszonen.png]]

Q: Was ist eine Aktivitätszone ([[Sequenzdiagramm]])
A: Die visualisierung der Zeit, in der ein Objekt etwas tut.
<!--ID: 1645543048118-->


Während ein Objekt auf eine Antwort wartet, wird dieses selbst lahmgelegt.

![[Sequenzdiagramm Assynchr.png]]
*Falls ich das richtig verstanden habe, werden die Rechtecke übereinander gezeichnet, um zu zeigen, dass der Thread, der das Gemeinschaftfeld betreten hat der gleiche ist wie der, der nun 200 Gutschreibt.*

## Asynchrone Nachrichten
Asynchrone Nachrichten werden durch offene Pfeilspitzen dargestellt.
Es scheint so, als ob bei asynchronen Nachrichten die Objekte nicht auf Antworten warten und deshalb sofort in Bereitschaft gehen.

![[Sequenzdiagramm Assynchrone Nachricht.png]]

Q: Wie sieht eine asynchrone Nachricht in einem [[Sequenzdiagramm]] aus.
A: Durchgezogener Pfeil mit normaler Pfeilspitze.
<!--ID: 1645543048250-->



## Erzeugung und Zerstörung von Objekten
Zeinet man gestrichelte Pfeile mit den Schlüsselwörtern new/create kann man ein Objekt erzeugen.
Durch das Schlüsselwort destroy und einem Kreuz bei der Lebenslinie kann man Objekte zerstören. Ich verstehe nur nicht warum der Pfeil beim Erstellen gestrichelt ist.

![[Sequenzdiagramm Erzeugung.png]]

Q: Wie wird in einem [[Sequenzdiagramm]] ein Objekt erzeugt?
A: Ein gestrichelter Pfeil mit create zeigt auf ein Rechteck mit dem Namen des neuen Objektes.
<!--ID: 1645543048369-->


Q: Wie wird in einem [[Sequenzdiagramm]] ein Objekt zerstört?
A: Ein durchgezogener Pfeil zu einem Kreuz.
<!--ID: 1645543048487-->


Q: Nenne 3 von 5 Regler/Fragmente, um [[Sequenzdiagramm]] zu kontrollieren.
A: - opt
- alt
- loop/break
- par
- neg
<!--ID: 1645543048606-->


## Bedingungen
Manchmal ist eine Interaktion optional oder von Bedingungen abhängig.
z.B. man kauft sich eine Straße, wenn sie frei ist und Geld vorhanden ist.

![[Sequenzdiagramme.png]]
Man nennt das Eingebettete Sequenzdiagramm opt wenn die Operation optional ist oder alt, wenn es mehrere Alternativen gibt.

Q: Wie stellt man in einem [[Sequenzdiagramm]] optionale Nachrichten dar?
A: Durch einen Kasten mit dem Namen opt.
<!--ID: 1645543048730-->



## Wiederholung
Will man Unterdiagramme wiederholen, so macht man das mit loop (1, n).
Schleifen kann man mit einem break verlassen.
![[Sequenzdiagramm Wiederholung.png]]

## par, seq, strict
par, seq, strict sind Operatoren, die die Reihenfolge festlegen, in der Aktionen ausgeführt werden könnnen/sollen.
- par: Die Interaktionen können in beliebiger Reihenfolge und sogar gleichzeitig passieren
- seq: Die Interaktionen können in beliebiger Reihenfolge stattfinden, dürfen aber nicht gleichzeitig passieren.
- strict: Die Reihenfolge, die durch die Achse festgelegt ist

![[Sequenzdiagramm par.png]]

## Sonstiges
- **critical**: Atomare Nachfolgen, die nicht unterbrochen werden dürfen sind in einem [[Kritischer Abschnitt|Kritischen Bereich]] 
- **ref**: Teile des Digramms können in seperate Diagramme verkapselt werden

![[Sequenzdiagramm Kapselung.png]]

## Zeitbedingungen
Nicht ganz verstanden. Hoffentlich ist das nicht relevant.






#Softwaretechnik 


