## Definition
Eine [[Natürliche Zahlen|Natürliche Zahl]] heißt Primzahl, wenn sie nur durch 1 oder sich selbst teilbar ist.

## Eigenschaften
### Euklids erster Satz
Ist $p$ prim und sind $a, b \in \mathbb{Z}$ mit $p|ab$, dann gilt $p|a$ oder $p|b$

D.h.: Ist $ab$ durch eine Primzahl [[Teilbarkeit|teilbar]], so ist entweder $a$ oder $b$ durch eine Primzahl teilbar. 


### Euklids zweiter Satz
Es gibt unendlich viele Primzahlen

**Beweis:**
Angenommen es gibt eine endliche Menge $M = \{p_1, ..., p_n\}$ aller Primzahlen.
Dann ist das Produkt $p_1 \cdot ... \cdot p_n$ aller dieser Zahlen eine ganze Zahl und offensichtlich durch jede Primzahl $p_i$ teilbar.

Betrachte aber nun $p_1 \cdot ... \cdot p_n + 1$!
$p_1 \cdot ... \cdot p_n + 1$ ist durch keine Primzahl $p_i$ teilbar, da erst $p_1 \cdot ... \cdot p_n + p_i$ die nächste durch $p_i$ teilbare Zahl ist. 
Also muss $p_1 \cdot ... \cdot p_n + 1$ entweder eine neue Primzahl sein oder unentdeckte Primzahlen enthalten. Dadurch erhalten wir aber einen Widerspruch, da $M$ somit nicht die Menge aller Prizahlen war. 

### Primzahlsatz
Der Primzahlsatz beschreibt, wie häufig Primzahlen vorkommen.
Sei $$\pi(n) = |\{p \leq n | p \in \mathbb{N} \text{ ist prim}\}|$$
Dann gilt
$$\underset{n \to \infty}{\lim} \frac{\pi(n)}{\frac{n}{\ln(n)}}$$

#Böhm 

