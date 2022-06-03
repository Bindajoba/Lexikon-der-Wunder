# Beschreibung
Ideale wurden eingeführt, um einen Ersatz für eine eindeutige Primfaktorzerlegung in [[Faktorieller Ring|Nicht-faktoriellen Ringen]] zu finden.
Sie sind den [[Normalteiler]] der Gruppentheorie sehr ähnlich, da diese genauso für [[Faktorring|Faktorstrukturen]] genutzt werden können.

# Definition
Sei $R$ ein [[Ring]]. Ein **Ideal** in $R$ ist eine Teilmenge $I \subseteq R$ mit den Eigenschaften 
1. $0_R \in I$
2. Für alle $a, b \in I$ und $r \in R$ gilt $a + b \in I$ und $ra \in I$

# Beispiel
## Hauptideal
Siehe [[Hauptideal]]

# Rechenregeln
## Untergruppeneigenschaft
Ist $I$ ein Ideal im Ring $R$, dann ist $I$ eine [[Untergruppe]] von $(R, +)$

## Schnitt
Sei $R$ ein Ring und $(I_j)_{j\in A}$ eine Familie von Idealen in $R$. Dann ist $I = \bigcap_{j \in A} I_j$

## Summe
Seien $I, J$ Ideale in $R$. Dann ist auch die Teilmenge $I+J = \{a+b : a \in I, b \in J\}$ ein Ideal in $R$

## Produkt
Siehe [[Produktideal]]

## Teilmengen
Zu **Idealen** kann man einige Voraussetzungen und Folgerungen zu und aus Teilmengen formulieren.
1. Es gilt $(a) \subset (b)$ genau dann, wenn $b | a$
2. Ist $d \in R$ mit $(d) = (a, b)$, dann ist $d$ ein ggT von $a$ und $b$
3. Ist $e \in R$ mit $(e) = (a) \cap (b)$, dann ist ist $e$ ein kgV von $a$ und $b$

In einem [[Hauptidealring]] gelten von ii und ii auch die Umkehrungen.[^1]

## Distributivgesetz
Für Ideale gilt das [[Distributivgesetz]]
$$I(J+K) = IJ + IK$$


# Beispiele
## Triviale Ideale
In jedem [[Ring]] $R$ ist das Nullideal $(0_R) = \{0_R\}$ das kleinste und das Einheitsideal $(1_R) = R$ das bezüglich Inklusion größte Ideal.


#Zahlentheorie 

[^1]: Gerkmann - Satz 10.1