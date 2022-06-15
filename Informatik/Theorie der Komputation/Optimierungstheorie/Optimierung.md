# Beschreibung
Es geht darum ein Problem zu optimieren.

# Definition
Sei $\mathcal{X}$ eine willkürliche Menge, genannt Zustandsraum (*state space*). Sei $\mathcal{T}$ eine willkürliche Menge, genannt Zielraum *target space*, und $\leq$ eine [[Totale Ordnung]] auf $\mathcal{T}$.
Eine [[Totale Funktion]] $\tau : \mathcal{X} \to \mathcal{T}$ wird Zielfunktion genannt. Optimierung ist der Prozess, nach einem $x \in \mathcal{X}$ zu suchen, sodass $\tau(x)$ optimal (minimal/maximal) ist.

*Üblicherweise gehen wir von Minimierung der Zielfunktion*

# Visualisierungen
![[Zielraum und Zustandsraum.png]]
![[Target Space und State Space 2.png]]

# Charakteristika Schwieriger Landschaften
- **Smoothness** (= [[Stetigkeit]])
  Ist eine Landschaft nicht stetig, können manche 
- **Deception**
  Die Landschaft hat eine solche Form, dass sie zur falschen Lösung verleitet. z.B. ein Brunnen auf einem Hügel. Etwas formaler: Die Landschaft ist global anders als man von einer Lokalen Betrachtung erwarten würde
- **Premature Konvergence**
  Die Landschaft hat einige Lokale Optima, bei denen der [[Optimierungslauf]] stecken bleiben kann.

Q: Nenne drei Charakterisitka schwieriger Ziellandschaften
A: - Smoothness
- Deception
- Premature Konvergence

# Beispiele
## Shortest Path
[[Shortest Path Problem]] bei einem [[Graph|Graphen]]:
*Sei ein Graph gegeben, was ist der kürzeste Abstand von einem Knotenzu einem anderen. (Gewichte eingeschlossen)*

## Lineare Regression
Was ist die Gerade, sodass der Abstand aller Punkt zu [[Gerade]] minimal ist.

## Knapsack Problem
Siehe [[KNAPSACK-Problem]].

## Schach
Was ist der Zug, mit dem meine Siegwahrscheinlichkeit maximier wird?






$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Natural-Computing 
