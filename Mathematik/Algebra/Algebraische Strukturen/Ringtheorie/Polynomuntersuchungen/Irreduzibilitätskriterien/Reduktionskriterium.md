\braTARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Das Reduktionskriterium gibt im engsten Sinne eine Möglichkeit, zu prüfen, ob eine Funktion irreduzibel ist. Im Allgemeineren hat dieses aber noch einen weiteren Anwendungsbereich.

# Definition
Sei $R$ ein [[Faktorieller Ring]], $p \in R$ ein [[Primelement]] und $\bar R = R \backslash (p)$.
Es sei $f$ ein [[Primitives Polynom]], dessen [[Polynom (Ring, Körper)|Leitterm]] $a_n \notin (p)$ und $\bar f$ das Bild von $f$ in $\bar R[x]$.  Ist $\bar f$ in $\bar R[x]$ irreduzibel, dann auch das Polynom $f$ in $R[x]$.

*Obacht, die Umkehrung gilt nicht!!!!!!!!*


# Beispiel
Zu zeigen: $f = x^4+x+1$ ist irreduzibel  in $\Z[x]$ und $\Q[x]$.
Nach dem Reduktionskriterium genügt es zu zeigen, dass $f$ in $\F_2[x]$ reduzibel ist. Dann folgt die Reduzibilität über $\Z$ und nach [[Lemma von Gauß|Gauß'schen Lemma]] auch über $\mathbb{Q}$.
$f(\bar 0) = \bar 1$, $f(\bar 1) = \bar 1$
Ist $\bar f$ dennoch reduzibel, dann muss es eine Zerlegung in zwei irreduzible Polynome von Grad $2$ geben.
$x^2+x+1$ ist das einzige irreduzible Polynom von Grad $2$ in $\F_2[x]$. Dieses multipliziert sich aber nicht zu $f$! 

#Zahlentheorie 


