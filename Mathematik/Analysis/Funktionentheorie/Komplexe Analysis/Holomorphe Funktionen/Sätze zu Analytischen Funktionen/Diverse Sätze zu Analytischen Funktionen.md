## Beschreibung
[[Analytische Funktion|Analytische Funktionen]] sind sehr merkwürdig.
Deshalb gibt es viele Sätze die Zusammenhänge zu den unterschiedlichsten Sachen.

Ich wusste nicht, wo ich das ganze hintun soll, also steht es hier drin.

## Ausreichende Kriterien für Konstanz
### Kriterium $Re f(z) = 0$
Da $f$ analytisch (und damit lokal eine Drehsteckung) ist, muss es eine Richtung geben, in der man einen Punkt $z$ bewegen kann, sodass $f(z)$ sich parallel zur Re-Achse bewegt.
Da $Re f(z) = 0$, ist das aber nur möglich, wenn der Betrag der Bewegung $0$ ist.

Somit ist der Streckungsfaktor der Drehstreckung für alle $z$ $0$ und $f(z)$ ist konstant.[^9]

### Kriterium $|f(z)| = const$
Da $f$ analytisch (und damit lokal eine Drehsteckung) ist, muss es eine Richtung geben, in der man einen Punkt $z$ bewegen kann, sodass $f(z)$ sich senkrecht zum Kreis um $0$ mit Radius $const$ bewegt.
Da $|f(z)| = const$, ist das aber nur möglich, wenn der Betrag der Bewegung $0$ ist.

Somit ist der Streckungsfaktor der Drehstreckung für alle $z$ $0$ und $f(z)$ ist konstant.[^10]

### Kriterium $f(z)$ und $\overline{f(z)}$ analytisch
Da $f$ analytisch (und damit lokal eine Drehsteckung) ist, muss es eine Richtung geben, in der man einen Punkt $z$ bewegen kann, sodass $f(z)$ sich parallel und positiv zur Re-Achse $const$ bewegt.
Bewegt man nun $z$ (gegen Uhrzeigersinn) senkrecht, so bewegt sich $f(z)$ und $\overline{f(z))}$ nach oben.
Das widerspricht aber der Tatsache, dass $f(z)$ und $\overline{f(z)}$ achsensymmetrisch zur Re-Achse sein sollten.
Der Betrag der Bewegung musste also $0$ sein.

Somit ist der Streckungsfaktor der Drehstreckung für alle $z$ $0$ und $f(z)$ ist konstant.[^11]

## Argumentprinzip
Siehe [[Argumentprinzip]]

## Existenz von Nullstellen
Seien
- $\emptyset \neq U \subseteq \mathbb{C}$ ein [[Gebiet]] der Definitionsbereich von $f$
- $f:U \to \mathbb{C}$ eine [[Analytische Funktion]]
- $\overline{K}(a, r) \subseteq U$ eine [[Abgeschlosse Menge|abgeschlossene]] Kreisscheibe

Gilt:
$$\min\{|f(z)|:|z-a|=|r|\} > |f(a)|$$ so hat f eine Nullstelle in $K(a,r)$[^1]

## Satz der Gebietstreue
[[Satz der Gebietstreue]]


## Maximumsprinzip
[[Maximumsprinzip]]


## Minimumsprinzip
Seien
- $\emptyset \neq U \subseteq \mathbb{C}$ ein [[Gebiet]] 
$U$ ist der Definitionsbereich von $f$
- $f:U \to \mathbb{C}$ eine [[Analytische Funktion]]

Hat $|f|$ in $a\in U$ ein lokales Minimum, dann gilt $f(a)=0$ oder $f$ ist konstant auf $U$[^4]

**Beweis:**
Man stelle sich ein Gebiet $U$ vor. Dieses Gebiet wird durch die analytische Funktion auf ein neues verzerrtes Gebiet $f(U)$ abgebildet.
Misst man jetzt den Abstand von jedem Punkt des neuen Gebiets zum Ursprung ist es offensichtlich, dass entweder ein Randpunkt der 0 am nähesten ist oder dass die 0 selbst im Inneren liegt.

## Maximums- Minimumsprinzip für beschränkte Mengen
Seien
- $\emptyset \neq U \subseteq \mathbb{C}$ ein [[Beschränktheit|beschränktes]] [[Gebiet]] 
- $\overline{U}$ ist der [[Abschluss]] von $U$
- $f:\overline{U} \to \mathbb{C}$ eine [[Stetigkeit|stetige]] Funktion

Ist die Einschränkung $f|_U \to \mathbb{C}$ eine [[Analytische Funktion]], dann gilt:
1. $|f|$ nimmt auf dem [[Rand]] $\partial U = \overline{U}\backslash U$ ein Maximum an
D.h. Es gibt ein $a \in \partial U$ mit $|f(a)|=\max\{|f(z)|:z\in \overline{U}\}$
2. $f$ hat in $U$ eine Nullstelle oder $|f|$ nimmt auf $\partial U$ ein Minimum an. [^5]

## Maximums- Minimumsprinzip für Real- und Imaginärteil
Seien
- $\emptyset \neq U \subseteq \mathbb{C}$ ein [[Gebiet]] 
$U$ ist der Definitionsbereich von $f$
- $f:U \to \mathbb{C}$ eine [[Analytische Funktion]]

1. Hat $Re(f)$ in $a\in U$ ein lokales Maximum, dann ist $f$ konstant auf $U$
1. Hat $Im(f)$ in $a\in U$ ein lokales Maximum, dann ist $f$ konstant auf $U$
1. Hat $Re(f)$ in $a\in U$ ein lokales Minimum, dann ist $f$ konstant auf $U$
1. Hat $Im(f)$ in $a\in U$ ein lokales Minimum, dann ist $f$ konstant auf $U$[^6]

## Maximums- Minimumsprinzip für beschränkte Mengen und Real- Imaginärteil
Seien
- $\emptyset \neq U \subseteq \mathbb{C}$ ein [[Beschränktheit|beschränktes]] [[Gebiet]] 
- $\overline{U}$ ist der [[Abschluss]] von $U$
- $f:\overline{U} \to \mathbb{C}$ eine [[Stetigkeit|stetige]] Funktion

Ist die Einschränkung $f|_U \to \mathbb{C}$ eine [[Analytische Funktion]], dann gilt:
1. $Im(f)$ und $Re(f)$ nimmt auf dem [[Rand]] $\partial U = \overline{U}\backslash U$ ein Maximum an
D.h. Es gibt ein $a \in \partial U$ mit $|f(a)|=\max\{|f(z)|:z\in \overline{U}\}$
2. $Im(f)$ und $Re(f)$ nimmt ein Minimum an. [^7]

## Satz von Liouville
([[Satz von Liouville]])

## Residuensatz
Siehe ([[Residuensatz]])

## Zählen von Nullstellen
Siehe ([[Residuensatz|Zählen von Nullstellen]])

## Satz von der lokalen Umkehrfunktion
Es sei 
- $\emptyset \neq U \subseteq \mathbb{C}$ [[Offene Menge|offen]]
- $f: U \to \mathbb{C}$ analytisch
- $a\in U$ mit $f'(a) \neq 0$

Dan ist $f$ lokal biholomorph um $a$, d.h. es gibt eine offene Umgebung $V$ von $a$ und eine offene Umgebung $W$ von $f(a)$, sodass $g:V \to W, z \mapsto f(z)$ [[Biholomorphe Funktion|biholomorph]] ist.[^8]

## Schwarzsches Lemma
Siehe [[Schwarzsches Lemma]]


#Mathe-IV 
#Needham 

[^1]: Zenk - Lemma 22.5.1
[^2]: Zenk - Satz 22.5.4
[^4]: Zenk - Korollar 22.5.6
[^5]: Zenk - Korollar 22.5.7
[^6]: Zenk - Satz 22.5.8
[^7]: Zenk - Korallar 22.5.9
[^8]: Zenk - Satz 25.1.6
[^9]: Needham - Aufgabe Kap. 3-7-i
[^10]: Needham - Aufgabe Kap. 3-7-ii
[^11]: Needham - Aufgabe Kap. 3-7-iii