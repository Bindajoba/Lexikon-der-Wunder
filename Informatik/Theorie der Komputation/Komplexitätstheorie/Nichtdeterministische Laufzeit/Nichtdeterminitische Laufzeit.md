## Beschreibung
Die **Nichtdeterministische Laufzeit** ist die Zeit, die eine stets anhaltende nichtdeterminisitsche Turingmaschine braucht, um auf allen Wegen ein Wort zu akzeptieren oder abzulehnen. 
Es ist ein Spezialisierung der allgemeinen [[Komplexität eines Algorithmus]]

## Definition
Sei $M$ eine stets anhaltende [[Turingmaschine|NTM]] mit Startzustand $z_0$.

Für Eingabe $w$ definieren wir 
$$ntime_M(w) := \max\{i : z_0w \vdash^i_M uzw \text{ und } uzw ...\}$$

