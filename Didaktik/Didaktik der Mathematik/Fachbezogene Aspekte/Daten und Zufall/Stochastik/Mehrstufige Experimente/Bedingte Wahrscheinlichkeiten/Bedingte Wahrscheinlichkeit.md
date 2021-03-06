TARGET DECK: Universität::Informatik::SWT

# Beschreibung

# Definition
Die Wahrscheinlichkeit für das Eintreten eines Ereignisses A unter der Bedingung B (d.h. wenn man schon weiß, dass B eingetreten ist) heißt bedingte Wahrscheinlichkeit von A unter B.

Formal wird die bedingte Wahrscheinlichkeit definiert als 
$$P_B(A) = \frac{P(A \cap B)}{P(B)}$$
*Warum ist $P(B) \neq 0$?*


# Fehler
## Vernachlässigung von Basisraten
(Oder Vertauschen der Bedingten Wahrsch. und Bedingung)
9 von 10 Leuten der tödlich verunglückten Autofahrern trugen einen Sicherheitsgurt. 
Sicherheitsgurte sind lebensgefährlich!!!

Problem:
Man sollte berechnen wie hoch die Wahrscheinlichkeit zu sterben ist, unter der Bedingung, dass man einen Gurt trägt, nicht
Die Wahrscheinlichkeit, dass man einen Gurt trägt, unter der Bedingung dass man stirbt.
$$P_A(B) \neq P_B(A)$$
Die richtige Wahrscheinlichkeit erhält man wie folgt:
![[Bedingte Wahrscheinlichkeit Vertauschen.png]]

Oder man benutzt die [[Formel von Bayes]], welche aus dem oberen Diagram folgt:
$$P_B(A) = \frac{P_A(B)\cdot P(A)}{P_{\bar A}(B) \cdot P(\bar A) + P_A(B) \cdot P(A)}$$



# Beispiele
## Impfung
![[Bedingte Wahrscheinlichkent Grippeimpfung.png]]

## Rückwärtsaufgabe
![[Bedingte Wahrscheinlichkeit.png]]
Die Aufgabe könnte man mit einer Tabelle mit Natürlichen Häufigkeiten lösen.

## Laplace Methoden
![[Bedingte Wahrschelinlichkeit Laplace.png]]

## Randomized Repsonse Methods
![[Bedingte Wahrscheinlichkeit Randomized Response Maethods.png]]

## Notwendigkeit von Mathematischer Analyse
![[Bedingte Wahrscheinlichkeit Weiißer Chip.png]]

# Übungen
## Klausur 2020 Aufgabe 11
![[Klausur 2020 Aufgabe 11.png]]
Martin Schulz hat Basisraten vernachlässigt. Statt die Wahrscheinlichkeit anzugeben, dass eine Person mit der Bedingung zwischen 25 und 35 Jahre einen befristeten Arbeitsvertrag hat, hat er die Wahrscheinlichkeit angegeben, dass jemand mit einem befristeten Arbeitsvertrag zwischen 25 und 35 Jahren alt ist.

Sei $B:$ Befristeter Arbeitsvertrag, $A:$ Zwischen 25 und 35 Jahren als.
Dann gilt $P_B(A) = 40\%$ aber $P_A(B) = 18\%$




#Mathe-Didaktik-III 


