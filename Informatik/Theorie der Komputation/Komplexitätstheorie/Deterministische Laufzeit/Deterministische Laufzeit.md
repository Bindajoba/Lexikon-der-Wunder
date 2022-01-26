## Beschreibung
Die **Deterministische Laufzeit** ist die Zeit, die eine stets anhaltende Turingmaschine braucht, um ein Wort zu akzeptieren oder abzulehnen. 
Es ist ein spezialisierung der allgemeinen [[Komplexität eines Algorithmus]]

## Definition
Sei $M$ eine stets anhaltende [[Turingmaschine|DTM]] mit Startzustand $z_0$.

Für Eingabe $w$ definieren wir $time_M(w) := i$, wenn $z_0w \vdash^i_M uzw$ und $z$ ist Endzustand oder Verwerfe Zustand.
