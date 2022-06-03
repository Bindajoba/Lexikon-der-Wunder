TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Kohäsion und Kopplung sind zwei Wörter, um die Stärke der Abhängigkeit zweier Komponenten zu bewerten.
*Das ist wie bei einem Zug, da muss die Kopplung zwischen Wagons niedrig ist aber die Stärke/Kohäsion der Wagons selbst hoch.*

### Kopplung
Ein [[Softwaresystem]] ist in mehrere [[Softwarekomponente]] zerlegbar. Diese Komponenten kommunizieren über Schittstellen miteinander. Je häufiger auf eine Schnittstelle zugegriffen wird, desto größer ist die Abhängigkeit/**Kopplung** zwischen den Komponenten.
Je niedriger die Kopplung, desto eigenständiger ist die Komponente und desto höher ist die Wartbarkeit des Systems.
Sie ist ein qualitatives Maß für die Schnittstellen zwischen Komponenten.

Es wird zwischen unterschiedlichen Arten der Kopllung unterschieden:
- Inhaltskopplung (content coupling)
- Bereichkopplung (common-environment coupling)
- Hybridkopplung (hybrid coupling)
- Kontrollkopplung (control coupling)
- Datenkopplung (data coupling)
- Pathologische Kopplung (pathological coupling)

Q: Was ist Kopplung? ([[Softwarearchitektur]])
A: Ein Maß dafür, wie stark Module vernetzt sind.
<!--ID: 1645260973933-->


### Kohäsion
Die Köhäsion beschreibt den Grad des inneren Zusammenhangs der Komponenten, Klassen eines Systems. In einem System mit starker Kohäsion erfüllt jede Programmeinheit genau eine wohldefinierte Aufgabe.
Sie ist ein qualitatives Maß für die Kompaktheit einer Komponente.

Q: Was ist Kohäsion? ([[Softwarearchitektur]])
A: Ein Maß dafür, wie stark die Bestandteile eines Moduls vernetzt sind.
<!--ID: 1645260974065-->

# Übungen
## Übung SWT 13-2
### a)
Was verbirgt sich im Kontext der objektorientierten Programmierung hinter den Begriffen
„Kohäsion“ und „Kopplung“?

- Kohäsion: Wie unzertrennlich die Aufgabe einer Klasse ist. Hat die Klasse schlecht Kohäsion, so lässt sich sich vermutlich aufspalten
- Kopplung: Wie häufig zwei Objekte aufeinander zugreifen. Bei zu hoher Kopplung könnte es sinnvoll sein die Objekte zu vereinen.

 ### b)
 Weshalb ist es von Vorteil, wenn ein System hohe Kohäsion und geringe Kopplung aufweist?
- *Hohe Kohäsion und geringe Kopplung fördert Wartbarkeit*

Q: Weshalb ist es von Vorteil, wenn ein System hohe Kohäsion und geringe Kopplung aufweist?
A: Fördert Wartbarkeit

Q: Frage
A: Antwort

#Softwaretechnik 