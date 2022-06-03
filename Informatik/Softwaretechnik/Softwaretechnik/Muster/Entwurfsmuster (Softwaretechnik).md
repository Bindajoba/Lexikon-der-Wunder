TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Muster (auch Design Pattern) sind Lösungen auf variable Probleme der Softwaretechnik.

Q: Was ist ein Pattern?
A: Ein Pattern ist eine standardisierte Lösung auf ähnliche, wiederkehrende Probleme der Softwareerstellung.
<!--ID: 1642761437403-->

# Bestandteile
Design Patters umfassen vier Maßgebliche Elemente:
1. **Name**
2. **Problemstellung**
Die Situation, in der das Pattern anzuwenden ist.
3. **Lösung**
Die Beschreibung des Patterns
4. **Konsequenzen**
Die Auswirkungen und Kompromisse, die man berücksichtigen muss

Q: Durch welche 4 Elemente können Entwurfsmuster beschreiben werden?
A: 1. Name
2. Problemstellung
3. Lösung
4. Konsequenzen
<!--ID: 1645260971863-->


# Vorteile
1. Entwurfmuster haben sich als Lösung auf Probleme bewährt.
2. Entwurfsmuster sind vielseitig anwendbar
3. Entwurfmuster bilden Bausteine höherer Abstraktion, über die man reden kann
4. Entwurfsmuster sind vermutlich anerkannte Lösungen auf Probleme

# Anwendung
Will man Entwurfsmuster anwenden kann man sich an diese Schritte halten, die von der "Gang of Four" definiert wurden.
1. Passende Objekte finden
2. Objektgranularität bestimmen
3. Objektschnittstellen spezifizieren
4. Objektimplementierung spezifizieren
5. Wiederverwendungsmechanismen einsetzen
6. Strukturen der Laufzeit beim Kompilieren abstimmen
7. Designänderung berücksichtigen

*Puh, das ist, um es englisch auszudrücken eine Mundvoll. Ich verstehe das nicht ganz. Ich denke, ich lerne nur die Pattern selbst. Das wird schon passen.*

# Klassifikation
## Zweck
Entwurfsmuster lassen sich in drei Bereiche unterteilen.

Q: In welche drei Zweckarten von Mustern lassen sich Entwurtfmuster klassifizieren?
A: - Erzeugungsmuster
- Strukturmuster
- Verhaltensmuster
<!--ID: 1645260972042-->

- **Erzeugungsmuster**
Beziehen sich auf der Erstellungsprozess von Objekten
- **Strukturmuster**
Wirken sich auf die Zusammensetzung von Klassen und Objekten aus
- **Verhaltensmuster**
Charakterisieren die Art und Weise der Interaktion von Klassen und Objekten sowie die Verteilung der Zuständigkeiten.

## Gültigkeitsbereich
Entwurfsmuster lassen sich weiter dadurch klassifizieren, ob sie primär auf Klassen oder auf Objekten angewendet werden.
- **Klassenbasierte Entwurfsmuster**
Werden durch Unterklassen an die Situation angepasst und sind vor dem Kompilieren fest
- **Objektsbasierte Entwurfmuster**
Werden durch das Instanziieren von Objekten angepasst und sind auch noch nach dem Kompilieren veränderbar

## Klassifikationstabelle
| Gültigkeit/Zweck   | Erzeugungsmuster     | Strukturmuster | Verhaltensmuster           |
| ------------------ | -------------------- | -------------- | -------------------------- |
| **Klassenbasiert** | [[Factory Method]]   | [[Adapter]]+    | [[Template Method]]        |
| **Objektbasiert**  | [[Abstract Factory]] | [[Kompositum]]+ | [[Iterator]]               |
|                    | [[Singleton]]+        | [[Proxy]]+      | [[Observer]]+               |
|                    |                      |                | [[State (Entwurfsmuster)]] |
|                    |                      |                | [[Visitor]]                           |

Mit + sind die Patterns benennt, die man Detailliert kennen soll.

Q: Nenne ein Erzeugungsmuster ([[Entwurfsmuster (Softwaretechnik)]]) 
A: - Factory Method
- Abstract Factory
- Singleton
<!--ID: 1645454018180-->


Q: Nenne ein Strukturmuster ([[Entwurfsmuster (Softwaretechnik)]])
A: - Adapter
- Kompositum
- Proxy
<!--ID: 1645454018311-->


Q: Nenne ein Verhaltensmuster ([[Entwurfsmuster (Softwaretechnik)]])
A: - Template Method
- Iterator
- Observer
- State
- Visitor
<!--ID: 1645454018440-->


# Übungen
## Übung SWT 10-1
Beantworten Sie kurz und bündig folgende Fragen!
- Welche Vorteil ergeben sich durch den Einsatz eines Design-Pattern?
Design Patterns sind erprobte Lösungen auf häufig wiederkehrende Probleme. Mit ihnen kann man Zeit und Fehler ersparen
- Design-Pattern werden in drei Kategorien unterteilt. Nennen Sie die Kategorien sowie
jeweils ein passendes Design-Pattern.
Erzeugungsmuster (Abstract Factory), Strukturmuster (Adapter), Verhaltensmuster (Iterator)
- Manche Design-Pattern werden oftmals miteinander kombiniert und arbeiten zusammen.
Geben Sie hierfür zwei Beispiele an und erklären diese kurz.
Die View eines Model-View-Controller nutzt häufig eine Struktur eines Kompositums, um seine Elemente zu organisieren.
*Visitor+Kompositum, Iterator+Kompositum*

## Übung SWZ 10-2
Modellieren Sie folgenden Sachverhalt als UML-Klassendiagramm. Gehen Sie dabei davon aus, dass für die Implementierung Java zu benutzen wäre. Sie müssen jedoch keine Implementierung erstellen, sondern nur das UML-Klassendiagramm. Sie werden feststellen, dass ein naiver Ansatz problematisch ist. Besser ist es, auf ein passendes Design-Pattern zurückzugreifen.Welches Design-Pattern wäre hierfür geeignet?
Eine Grafikbibliothek soll die Verwendung folgender Fenstertypen erlauben:
- einfache Fenster ohne Zusatzfunktionalität
- Fenster, die eine Titelleiste haben
- Fenster, die eine Statusleiste haben
- Fenster, die horizontal und vertikal „scrollbar“sind
- alle daraus konstruierbaren „Featurekombinationen“, wie z.B. ein Fenster mit Titelleiste
das horizontal und vertikal „scrollbar“ist

Sinnvoll wäre eine Factory, das heißt eine Factory Method, mit der man spezielle Fenster erstellen kann.
*Sinnvoll wäre ein Decorator, ein Entwurfsmuster, mit dem man Features dazustapeln kann.*

## Übung SWT 10-3
Wir betrachten in dieser Aufgabe Terme über die Rechenarten $op \in \{+, -, \cdot, /\}$ die rekursiv definiert sind:
- jedes Literal ist ein Term, z.B. „4“.
- ist t ein Term, so ist „(t)“ ein (geklammerter) Term.
- sind t1, t2 Terme, so ist „t1 op t2“ ebenso ein Term.
Beispiele für gültige Terme sind also „4 + 8“, „4  8“ oder „4 + (4  8)“.

### a)
Modellieren Sie eine Klassenstruktur in UML, mit Hilfe derer eine rekursive Struktur von Termen erstellt werden kann. Sehen Sie mindestens einzelne Klassen für die Addition und Multiplikation vor, sowie weitere Klassen für geklammerte Terme und Literale, welche ganze Zahlen repräsentieren. Welches Design-Pattern eignet sich hier am Besten?
(Hinweis: es ist nicht das Visitor-Pattern :-) )

Das [[Kompositum]]


### b)
Die Klassenstruktur soll das Visitor-Pattern unterstützen, damit das Auswerten von Termen bzw. das Ausgeben in einer leserlichen Form in zwei Visitor-Klassen TermEvaluator bzw. TermPrinter erfolgen kann.
Gehen Sie bei der Modellierung der Klassenstruktur davon aus, dass für die Implementierung Java zu benutzen wäre.

### c)
Fertigen Sie eine Implementierung für diese Klassenstruktur an, welche die oben genannten Terme anlegt und über die Visitor-Klassen ausgibt bzw. denWert berechnet.

#Softwaretechnik 


