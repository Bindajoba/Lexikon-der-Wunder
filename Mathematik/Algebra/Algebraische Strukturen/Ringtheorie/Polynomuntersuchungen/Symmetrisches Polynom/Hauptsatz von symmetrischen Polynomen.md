TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Der Hauptsatz sagt aus, dass jedes [[Symmetrisches Polynom]] als Polynom in den [[Elementarsymmetrisches Polynom|Elementarsymmetrischen Polynomen]] geschrieben werden kann.

# Übungen
## Waerden 5.17 Potenzsumme
Für beliebige $n$, beschreibe die "Potenzsummen" $\sum x_i, \sum x_i^2, \sum x_i^3$ durch elementarsymmetrische Polynome.

Beginne mit $\sum x_i^2$:
Nach dem Beweis von Hadlock und Waerden können wir $s_1^2 = \sum_{i_1, i_2 \in  \{1, ..., n\}} x_{i_1}x_{i_2}$. Davon abziehen. Es bleibt übrig $-\sum_{\{i_1, i_2\} \subseteq \{1, .., n\}}x_{i_1}x_{i_2}$. Das ist einfach $s_2$.
Wir erhalten also $s_1^2-s_2$.

Beginne mit $\sum x_i^3$:
Nach dem Beweis von Hadlock und Waerden können wir $s_1^3 = \sum_{i_1, i_2, i_3 \in  \{1, ..., n\}} x_{i_1}x_{i_2}x_{i_3}$ davon abziehen. Es bleibt übrig ein Term $-x_1^2x_2$ und $-x_1x_2x_3$. 
Der erste Term ist auch in $s_1s_2$ enthalten. Addiert man $s_1s_2$, dann verschwindet der erste Term. Stattdessen erhalt man $3x_1x_2x_3$. $3$ für alle Möglichkeiten, diesen Term zu erzeugen.

Ich denke, die Antwort ist: $s_1^3-s_1s_2+4s_3$.


## Waerden 5.18
Sei $S_q := \sum x_i^q$
Zeige
$$s_\varrho-s_{\varrho-1}\sigma_1+s_{\varrho-2}\sigma_2-...+(-1)^\varrho \varrho\sigma_\varrho = 0 \text{ wenn } \varrho \leq n$$$$s_\varrho-s_{\varrho-1}\sigma_1+s_{\varrho-2}\sigma_2-...+(-1)^n s_{\varrho-n}\sigma_{n} = 0 \text{ wenn } \varrho > n$$



$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Algebra 


