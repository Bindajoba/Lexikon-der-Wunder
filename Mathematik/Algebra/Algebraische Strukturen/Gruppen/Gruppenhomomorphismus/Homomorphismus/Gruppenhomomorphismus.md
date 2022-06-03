# Beschreibung
Ein Gruppenhomomorphismus ist ein [[Homomorphismus]], der die Struktur einer [[Gruppe]] erhält.

Er ahmt die Struktur seiner Definitionsmenge nach.


# Intuition
Homomorphismen tauchen in genau zwei Situationen auf:
1. Bei [[Untergruppe|Untergruppen]]
2. Bei [[Faktorgruppe|Faktorgruppen]]

## Untergruppe
Siehe [[Einbettung (Gruppe)]]

## Faktorgruppe
Siehe [[Quotientenkarte]]

# Definition
Seien $(G, \cdot), (H, *)$ Gruppen.
Ein **Gruppenhomomorphismus** $\phi$ erfüllt die Bedingung
$$\phi(g_1 \cdot g_2) = \phi(g_1) * \phi(g_2)$$

*Beobachte, dass die Bedingung $\phi(e_G) = e_H$ und $\phi(g^{-1}) = \phi(g)^{-1}$ nicht erfüllt werden muss.
Diese Bedingungen sind natürlich für die Gruppenstruktur notwendig, folgen aber aus der Tatsache, dass $G$ und $H$ Gruppen sind.*

# Charakterisierungen
## Cayley-Diagramm
Wenn ein Pfeil $b$ im [[Cayley-Diagramm]] der Urbildmenge von $a$ nach $c$ geht, dann muss der Pfeil $\phi(b)$ in der Gruppe der Bildmenge von $\phi(a)$ nach $\phi(c)$ gehen.


# Eigenschaften
## Injektivität
Die Abbildung $\phi$ ist genau dann injektiv, wenn $ker(\phi) = \{e_G\}$ gilt.

Siehe [[Kern]].

## Untergruppen
Sei $\phi: G \to H$ ein [[Gruppenhomomorphismus]], außerdem $U$ eine [[Untergruppe]] von $G$ und $V$ eine Untergruppe von $H$. Dann gilt:
	- Die Bildmenge $\phi(U)$ ist eine Untergruppe von $H$
	- Die Urbildmenge $\phi^{-1}(V)$ ist eine Untergruppe von $G$[^2]

## Homomorphismen und Erzeugendensysteme
Seien $G, H$ Gruppen und $S \subseteq G$ ein [[Erzeugendensystem]] von $G$. Sind $\phi, \phi': G \to H$ Gruppenhomomorphismen mit $\phi(s) = \phi'(s)$ für alle $s \in S$, dann folgt $\phi = \phi'$ auf der ganz $G$

*Ein Gruppenhomomorphismus ist also durch Angabe des Erzeugendensystems eindeutig definiert!*


# Ordnung unter Homomorphismen
Sei $\phi: G \to H$ ein Gruppenhomomorphismus.
Ist $g \in G$ ein Element von endlicher [[Ordnung (Gruppe)]] $n$, dann ist auch $ord(\phi(g))$ endlich und ein [[Division mit Rest|Teiler]] von $n$.

## Induzierter Homomorphismus
Siehe [[Induzierter Homomorphismus]]


## Homomorphiesatz für Gruppen
Siehe [[Homomorphiesatz für Gruppen]]

# Übungen
## Klausur 2016 Aufgabe 1
![[Klausur 2016 Aufgabe 1.png]]
### b)
- Neutrales Element
$\phi(e) = \psi(e) = e \implies e \in U$
- Abgeschlossen
Für $\phi(a) = \psi(a)$ und $\phi(b) = \psi(b)$
Dann auch $\phi(a + b) = \phi(a)+\phi(b) = \psi(a)+\psi(b) * \psi(a+b)$ also $a+b \in U$
- Inverses
Für $a \in U$
$\phi(-a) = -\phi(a) = -\psi(a) = \psi(-a)$
- Untermenge
Offensichtlich


#Algebra #Carter 