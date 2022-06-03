$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\C}{\mathbb C}$
![[blatt10.pdf]]

# Aufgabe 4
## a)
### Hauptideale)
Ideale $I$ werden durch Erzeugendensysteme $S \subseteq \C[x]$ erzeugt, diese werden nun untersucht.

Als Polynomring über einem Körper ist $\C[x]$ ein [[Euklidischer Ring]] und somit ein [[Hauptidealring]].
Somit hat jedes Ideal die Form $I=(f)$

Ohne Einschränkung ist $f$ normiert. Sonst kann man $f$ durch seine Normierungen ersetzen und dabei das gleiche Ideal erzeugen.

Soll $(f)$ maximal sein, dann darf $f$ keine Konstante $a \in \C, a \neq 0$ sein, da man sonst durch Multiplikation mit Elementen aus $\C[x]$ alle Elemente aus $\C[x]$ erzeugen kann.

Es gilt $f \neq \{0\}$, sonst ist $(f)$ nicht maximal.

$f$ kann nur noch ein normiertes Polynom sein.

$grad(f) = 1$. Hätte $f$ einen Grad größer als $1$, dann wäre es in $\C[x]$ in Linearfaktoren $(x-\alpha_1)...(x-\alpha_n)$ zerlegbar. Jeder der Linearfaktoren würden ein Ideal erzeugen, welcher größer ist, als $(f)$. Damit kann $(f)$ nicht maximal sein.

Sei damit $f = x + \alpha$
Sei $g \in \C[x]$. 
- Sind $f$ und $g$ teilerfremd, dann gilt $(f, g) = (1)$
- Sind $f$ und $g$ nicht teilerfremd, dann ist der einzige mögliche Teiler $f = (x+\alpha)$. Somit gilt: $(f, g) = f$ 

Damit gibt es keine Erweiterung von $(f)$, die eine größere Menge, die nicht $(1)$ ist, erzeugt.
$\implies (f)$ sind alle maximalen Ideal.

## b)
