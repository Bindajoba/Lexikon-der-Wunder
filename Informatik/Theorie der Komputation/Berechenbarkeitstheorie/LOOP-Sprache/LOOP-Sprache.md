## Beschreibung
LOOP ist eine sehr einfache imperative Programmiersprache

## Definition Syntax
LOOP-Programme werden durch die [[Kontextfreie Grammatik]] $(V, \Sigma, P, Prg)$ erzeugt, wobei
$$\begin{array}{rcl} V &= &\{Prg, Var, Id, Const\} \\ \Sigma &= &\{LOOP, DO, END, x, 0, ... 9, ;, :=, +, -\} \\ P &= &\left\{\begin{array}{lcl} Prg &\to &LOOP \ Var \ DO \ Prg \ END \\ && |Prg; Prg \\ && |Var := Var + Const \\ && |Var := Var - Const \\ Var &\to &x_{Id} \\ Const &\to &Id \\ Id &\to &0|1|...|9|1Const|2Const|...|9Const\}\end{array}\right\}\end{array}$$

### Variablenbelegung
Eine **Variablenbelegung** $\rho$ ist eine endliche Abbildung mit Einträgen $x_i \mapsto n$ mit $x_i$ ist Variable und $N\in \mathbb{N}$
$$\text{Wir definieren } \rho(x_i) := \begin{cases} n, &\text{wenn } x_i \mapsto n \in \rho \\ 0, &\text{sonst} \end{cases}$$ *D.h. initial sind aulle Variablen auf 0 gesetzt.*

Wir schreiben $\rho\{x_i \mapsto m\}$ für
$$\rho\{x_i \mapsto m\}(x_j) = \begin{cases} \rho(x_j), &\text{wenn } x_j \neq x_i \\ m, &\text{wenn } x_j = x_i \end{cases}$$

## Definition Semantik
Ich hoffe, die Semantik wird aus der Syntax klar.

## Kompexere Befehle

### Fallunterscheidung
Die Fallunterscheidung kann auf ziemlich perfide Weise mit LOOP implementiert werden.

### Maximale Erzeugbare Zahl
Da ein Loop-Programm aus endlich vielen Methoden besteht, endlich viele Variablen besitzt, diese nur endliche Startwerte annehmen können und nur endlich oft geloopt werden kann, können die Variablen nur maximale Werte annehmen.
*Das stimmt alles nicht. LOOP-Programme sind ja vom Input abhängig, die maximale Zahl kann also mit anderen Eingaben steigen. Somit ist die Aussage nutzlos.*

#FSK 