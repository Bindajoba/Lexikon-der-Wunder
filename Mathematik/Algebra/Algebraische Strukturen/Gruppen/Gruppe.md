## Beschreibung
Eine Gruppe ist eine [[Menge]] von Operationen, die spezielle Eigenschaften haben.
- In einer Gruppe ist die Verkettung von zwei Operationen wieder in der Menge enthalten.
- Die Umkehroperation einer Gruppe ist wieder in einer Menge enthalten

## Definition
### Definition (Zenk)
*Die Definition stammt aus meinem Gedächtnis und muss nicht komplett korrekt sein.*
Eine Gruppe ist eine Menge $M$ und eine Operation $+$ und wird geschrieben als $(M, +)$, wenn
- die Gruppe hat ein **neutrales Element** $e$ 
- für jedes Element $x \in M$ existiert ein **Inverses** $x^{1-} \in M$, sodass $x+x^{-1}$ 
- für zwei Elemente $x, y \in M$ ist auch $x+y\in M$
- Die Operation ist [[Assoziativität|assoziativ]]

### Definition (Arnold)
Es sei $A$ eine [[Transformationsgruppe]] auf einer Menge X (d.h. eine Menge von Transformationen)
Ignoriere die Menge $X$ einfach und nenne $A$ eine **Gruppe**.

Die Definition ist zu der oberen äquivalent, Arnold benutzt aber die Tupelschreibweise nicht.

### Definition Generator (Carter)
Carter benutze beim Erstellen von Gruppen den Begriff des Generators.

Ein Generator ist eine Menge von Aktionen, deren Hintereinanderausführung Aktionen aus dem gleichen Pool ergeben

Dabei muss:
- jedes Aktion eine Umkehraktion haben
- jede Aktion immer anwendbar sein
- jede Aktion hat ein determiniertes Ergebnis

**Obacht:**
Diese Definition erlaubt das Erstellen von [[Cayley-Diagramm|Cayley-Diagramme]] welche aber keine Gruppen nach den anderen Definitionen sind. Carter sagte, dass diese Definition daher unvollständig ist.
In späteren Kapiteln erklärt er, dass ein Cayley-Diagram zusätzlich [[Reguläres Diagramm|regulär]] sein muss, das heißt, sich an jedem Knoten gleich verhalten muss. (Jede Folge von Aktionen generiert ein Diagramm, welches bis auf Name genau gleich aussieht) 

### Gruppenhomomorphismus
Siehe [[Gruppenhomomorphismus]]

## Eigenschaften
### Eigenschaften bei Inversen
- Jedes Element $g\in G$ besitzt höchstens ein Inverses und wird mit $g^{-1}$ bezeichnet
- Seien $g, h \in G$ invertierbare Elemente. Dann sind auch $g *h$ invertierbar und es gilt $(g*h)^{-1} = h^{-1} * g^{-1}$ und $(g^{-1})^{-1} = g$
- Seien $g_1, ..., g_r \in G$ invertierbare Elemente. Dann sind auch $g_1 * ... * g_r*$ invertierbar und es gilt $(g*...*g_r*)^{-1} = g_r^{-1} * ... * g_1^{-1}$ und $(g^{-1})^{-1} = g$ 
(Beweis durch Induktion der vorherigen Regel)
- Das Neutralelement $e_G$ von $(G, *)$ ist invertierbar und es gilt $e_G^{-1} = e_G$[^2]

### Eigenschaften bei Potenzen
Sei $\phi:G \to H$ ein Gruppenhomomorphismus und $g \in G$
Dann gilt: $\phi(g^n) = \phi(g)^n$ für alle $n \in \mathbb{Z}$

*Den Beweis erhält man durhc Fallunterscheidung und Induktion der oberen Eigenschaften.*

### Endomorphismen zu Automorphismen
Sei $G$ eine Gruppe $\rho \in End(G)$ ein invertierbarer [[Endomorphismus]].
Dann ist $\rho$ ein [[Automorphismus]][^3]

Man nennt die resultierende Gruppe dann die [[Automorphismengruppe]].



## Beispiele
### Transformationsgruppe
Die [[Transformationsgruppe]] ist eine **Gruppe** von Transformationen

### Ganze Zahlen
Sei $A$ die Transformationsgruppe auf der Menge $\mathbb{Z}$, die die ganzen Zahlen hin und her bewegt.
Dann kann jede Transformation durch die Operation $+n$ mit $n\in\mathbb{Z}$ dargestellt werden.

Die Menge aller $+n$ bezeichnen wir als die **Gruppe** $(+, \mathbb{Z})$
*Ich denke, man schreibt $+n$, weil nur $n$ zu sehr wie eine Zahl aussieht, aber nur $+$ nicht alle Transformationen repräsentiert.*



### Permutationsgruppe
Die Menge $Per(X) \subset Map(X)$ der Permutationen versehen mit der [[Verknüpfung]] ist eine Gruppe und wird Permutationsgruppe von X gennannt.

Siehe [[Symmetrische Gruppe]]



#Arnold #Mathe-I #Carter #Algebra

[^1]: Gerkmann - Definition 1.7
[^2]: Gerkmann - Satz 1.6
[^3]: Gerkmann - Proposition 1.19