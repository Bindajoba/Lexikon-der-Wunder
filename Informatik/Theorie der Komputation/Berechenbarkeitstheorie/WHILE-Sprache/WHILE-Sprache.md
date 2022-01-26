## Beschreibung
Die WHILE-Sprache ist eine sehr kleine Programiersprache. Sie funktioniert genau so wie die [[LOOP-Sprache]], ist aber um ein WHILE-Konstrukt erweitert.

## Definition Syntax
LOOP-Programme werden durch die [[Kontextfreie Grammatik]] $(V, \Sigma, P, Prg)$ erzeugt, wobei
$$\begin{array}{rcl} V &= &\{Prg, Var, Id, Const\} \\ \Sigma &= &\{LOOP, DO, END, x, 0, ... 9, ;, :=, +, -\} \\ P &= &\left\{\begin{array}{lcl} Prg &\to & WHILE\ Var \neq 0 \ DO\ Prg\ END \\&& LOOP \ Var \ DO \ Prg \ END \\ && |Prg; Prg \\ && |Var := Var + Const \\ && |Var := Var - Const \\ Var &\to &x_{Id} \\ Const &\to &Id \\ Id &\to &0|1|...|9|1Const|2Const|...|9Const\}\end{array}\right\}\end{array}$$

Für den Rest schaue ins Skript, das Thema ist so laaangweilig,

## Eigenschaften
### LOOP-Sprache
Alle [[LOOP-Programme]] sind auch ein WHILE-Programm.
Das erkennt man schon daran, dass die LOOP-Syntax keine Zyklen und Rekursionen erlaubt.

### Eigenschaft 1
WHILE-Programme benütigen nur eine WHILE-Schleife


#FSK 