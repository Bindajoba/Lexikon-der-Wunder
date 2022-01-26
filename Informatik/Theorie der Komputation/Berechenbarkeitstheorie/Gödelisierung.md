## Beschreibung
Die Gödelisierung ist ein Verfahren, mit dem man durch eine [[Injektive Abbildung]] einem [[Wort]] einer [[Formale Sprache|Formalen Sprache]] oder einem Tupel eine eindeutige Nummer zuweisen kann.

Es wurde benannt nach dem Mathematiker [[Kurt Gödel]]

## Definition
Sei $M$ eine abzählbare Menge von [[Wort|Wörtern]] (also endlich lange Tupel). Eine Funktion
$$g:M\to \mathbb{N}$$ wird **Gödelisierung** gennant, wenn
- $g$ [[Injektivität|injektiv]] und [[Berechenbarkeit|berechenbar]],
- die [[Bildmenge]] $g(M)$ [[Entscheidbarkeit|entscheidbar]]
- die auf $g(M)$ definierte Umkehrfunktion von $g$ berechenbar ist.
$g(m)$ nennt man dann die **Gödelnummer**

## Spezialfälle & Anwendungen
- [[Gödelisierung (Turingmaschine)|Gödelisierung von Turingmaschinen]]

## Beispiel
Die folgende Gödelisierung funktioniert so:

Jedem Zeichen eines [[Alphabet|Alphabets]] wird eine Zahl zugewiesen. 
Jeder Position in einem Wort wird eine [[Primzahl]] zugeordnet.

Zu jeder Position wird die zugeordnete Primzahl mit der Zahl des da stehenden Zeichens potenziert. Dann werden die potenzierten Primzahlen miteinander multipliziert.

Das Wort $abccba$ konstruiert sich so:
- Das $a$ an erster Stelle hat den Wert $2^1=2$
- Das $b$ an zweiter Stelle hat den Wert $3^2 = 9$
- ...
- Das $a$ an sechster Stelle hat den Wert $13^1=13$

Multipliziert man alle Werte zusammen, erhält man die Gödelnummer.
Durch [[Primfaktorenzerlegung]] kann man dann das Wort zurückkonstruieren.


#FSK 