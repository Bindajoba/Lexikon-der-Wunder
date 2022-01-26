# BeschrQeibung
Die Konstruierbaren Zahlen sind alle Zahlen, die mit [[Euklidische Werkzeuge|euklidische Werkzeugen]] konstruierbar aus einer Einheitslänge konstruierbar sind.

# Erschließung
Die Konstruierbaren Zahlen enthalten nach Voraussetzung 1.
Durch Hintereinandersetzen der Länge 1 erhält man alle Natürlichen Zahlen.

Bei konstruierbaren Zahlen trifft man generell die Annahme, dass negative Zahlen Teil der Konstruierbaren Zahlen sind, wenn ihre positive [[Gegenzahl]] auch konstruierbar ist.
Damit sind die [[Ganze Zahlen]] Teil der **Konstrierbaren Zahlen**.


Durch [[Konstruktion eines Produktes]] und [[Konstrution eines Quotienten]] sind auch Quotienten von Ganzen Zahlen, d.h. [[Rationale Zahlen]] Teil der **Konstruierbare Zahlen**. 

Durch [[Konstruktion der Quadratwurzel]] können wir Quadratwurzeln von konstruierbaren Zahlen hinzufügen.

## Charakterisierung
##  Verschachtelung von Quadratwurzeln
Eine Zahl $a$ ist genau dann **konstruierbar**, wenn $a \in K_n$, wobei es für $K_n$ eine Folge von Quadratischen Erweiterungen $\mathbb{Q} = K_0 \subset K_1 \subset ... \subset K_n$, gibt. 

### Beweis (Hinreichend zum Konstruieren)
Uns fällt aus oberer Erschließung auf: Ziehen wir die Quadratwurzel einer Konstruierbaren Zahl, so ist die resultierende Zahl wieder konstruierbar.

 Können wir das irgendwie mit der Theorie der Körper verknüpfen, und dadurch hinreichende Bedingungen für Konstruierbarkeit erhalten?
 Ein Element einer [[Quadratische Erweiterung]] von $\mathbb{Q}$ hat die Form $a+b\sqrt{k}$ ($a, b \in \mathbb{Q}$) und ist konstruierbar.
**Feststellung 1**: Alle Quadratischen Erweiterungen von $\mathbb{Q}(\sqrt{k})$ bestehen aus konstruierbaren Elementen.
Verallgemeinern wir: Ist $K$ ein Körper aus konstruierbaren Elementen, dann ist $a+b{\sqrt{k}}$ auch konstruierbar. Damit ist jede Quadratische Erweiterung von $K$ konstruierbar!

Wir können also das Vorgehen vor Feststellung 1 rekursiv wiederholen und $\mathbb{Q}(\sqrt{k})$ um $\sqrt{l}$ quadratisch erweitern. Das Resultat ist wieder eine Menge aus konstruierbaren Elementen!
Wir erhalten folgende Feststellung:

**Feststellung 2:** Eine Zahl $a$ ist konstruierbar, wenn $a \in K_n$, wobei es für $K_n$ eine Folge von Quadratischen Erweiterungen $\mathbb{Q} = K_0 \subset K_1 \subset ... \subset K_n$, gibt. 

### Einzigen Konstruierbaren Zahlen
Sind die oberen Zahlen die einzigen Zahlen, die konstruierbar sind? Ja!

Der Beweis dazu ist ein wenig kompliziert, aber er lässt sich gut vereinfachen.
Eine $K$-Ebene ist die Menge aller zweidimensionalen Punkt $(x, y) \in K^2$.

Auf dieser Ebene können wir
- Eine Gerade durch zwei konstruierbare Punkte zeichnen
- Einen Kreis mit dem Mittelpunkt auf einem konstruierbaren Punkt, dessen Bogen durch einen konstruierbaren Punkt verläuft zeichnen.

Durch Herumgerechne mit Gleichungen erfährt man, dass der Schnittpunkt von
- Zwei Geraden ein Punkt in $K^2$ ist
- Zwei Kreisen ein Punkt in $K^2$ ist
- Einer Gerade und einem Kreis ein Punkt in $K(\sqrt{k}) \times K(\sqrt{l})$ ist. (Die Koordinaten sind also Quadratische Erweiterungen)

Durch m-fache Anwendung von Konstruktionen erhält man also nur Punkte mit den Koordinaten einer höchstens m-fachen Quadratischen Erweiterung.

Das Berechnen des Entfernung dieses Punktes zu einem anderen Punkt benötige nur eine Quadratwurzel und erfordert somit nur eine weitere quadratische Erweiterung.

# Eigenschaften
## Körpereigenschaft
Die man aus Konstruierbaren Zahlen die Summe, Differenenz, Produkt und Quotient konstruieren kann (und die 1 enthalten ist), bilden die **Konstruierbaren Zahlen** einen [[Körper]].



#Hadlock