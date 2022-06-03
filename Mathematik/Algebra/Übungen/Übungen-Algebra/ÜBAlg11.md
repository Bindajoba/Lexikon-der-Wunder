TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$

![[blatt11.pdf]]

# Aufgabe 1
## a)
Zu Zeigen: $[L:K] \leq n!$
Ohne Einschränkung ist $f$ normiert.

Löse die Aufgabe durch  über den Grad $n$ des Polynoms $f$
### Induktionsvoraussetzung
Induktionsvoraussetzung: $n = 1$ 
Dann liegt $f$ bereits in Linearform vor.
$\implies L = K \implies [L:K] = 1 = 1!$

### Induktion
Induktion für ein $n+1$:
Zu Zeigen: Für ein $K$-Polynom von Grad $n+1$ gilt:  $[L:K] \leq (n+1)!$

Der Zerfällungskörper von $f$ über $K$ ist definiert als die Adjunktion aller $n+1$ Nullstellen $\{\alpha_1, ..., \alpha_{n+1}\}$ von $f$ an $K$.
$f$ hat die Nullstelle $\alpha_{n+1}$. In $K(\alpha_{n+1})$ ist $f$ somit in einen Linearfaktor und ein Restpolynom $g \in K(\alpha_{n+1})[x]$ zerlegbar, sodass $f = (x-\alpha_{n+1})g$.
$g$ ist dabei ein Polynom von Grad $n$. Der Zerfällungskörper von $g$ über $K(\alpha_{n+1})$ ist $K(\alpha_{n+1})(\alpha_1, ..., \alpha_n)$.

Der Körper $K(\alpha_{n+1})$ ist ein Zwischenkörper von $L|K$. Somit gilt die Gradformel:
$$[L:K] = [K(\alpha_{n+1})(\alpha_1, ..., \alpha_n) : K(\alpha_{n+1})] \cdot [K(\alpha_{n+1}):K]$$
Nach Induktionsvoraussetzung gilt: $[K(\alpha_{n+1})(\alpha_1, ..., \alpha_n) : K(\alpha_{n+1})] \leq n!$

$f$ ist nach Angabe ein $K[x]$-Polynom mit der Nullstelle $\alpha_{n+1}$. Damit teilt $\mu_{K, \alpha_{n+1}}|f$ und es gilt $[K(\alpha_{n+1}):K] = grad(\mu_{K, \alpha_{n+1}}) \leq grad(f) = n+1$

Daraus folgt
$$[L:K] = [K(\alpha_{n+1})(\alpha_1, ..., \alpha_n) : K(\alpha_{n+1})] \cdot [K(\alpha_{n+1}):K] \leq n! \cdot (n+1) = (n+1)!$$

## b)
Zu Zeigen: $[L:K] = n! \implies f$ ist irreduzibel.

Aus der Gradformel folgt:
$$[L:K] = [K(\alpha_{n})(\alpha_1, ..., \alpha_{n-1}) : K(\alpha_{n})] \cdot [K(\alpha_{n}):K] \leq (n-1)! \cdot n$$
Für $[L:K] = n!$ muss also $[K(\alpha_{n}):K] = n$ erfüllt sein.
Das gilt genau dann wenn $grad(\mu_{K, \alpha_{n}}) = n = grad(f)$. 

$f$ hat die Nullstelle $\alpha_n$, somit gilt $\mu_{K, \alpha_n} | f$. Da beide Polynome aber den gleichen Grad haben, kann eine Division $f/\mu_{K, \alpha_n}$ nur einen Konstante ergeben, nämlich den Koeffizienten des Leitterms.

Normiert man $f$ zu $f'$ so ergibt die Division $f'/\mu_{K, \alpha_n} = 1$, d.h. $f' = \mu_{K, \alpha_n}$.
$f$ ist somit eine Skalarmultiplikation des irreduziblen Minimalpolynoms und ist damit selbst irreduzibel.

Die Umkehrung gilt nicht. Ist $\gamma$ eine Nullstelle des irreduziblen Polynoms $h(x) = x^3 + x+ 1 \in \F_2[x]$, dann zerfällt das Polynom nach dem Übungsblatt zu $(x-\gamma)(x-\gamma^2)(x-(\gamma^2+\gamma))$. Offensichtlich ist jeder Linearfaktor ein $\F_2(\gamma)[x]$-Polynom. $\F_2(\gamma)$ ist somit der Zerfällungskörper von $h$, dessen Erweiterungsgrad ist aber $3 \neq 3! = 6$

%%
# Aufgabe 2
## a)
Anzahl der Teilkörper von $\F_{3^6}$
Nach VL müssen alle Teilkörper die Form $\F_{3^n}$ haben und $n$ muss 6 ganzzahlig teilen. Die Teilkörper existieren und sind in dem Fall eindeutig.
D.h. $\F_{3^6},\F_{3^3},\F_{3^2}, \F_{3^1}$

## b)

Für ein $\alpha \in \F_{3^6}$ ergibt $\F_3(\alpha)$ den kleinsten Erweiterungskörper $K' \subseteq \F_{3^6}$ von $\F_3$, der $\alpha$ enthält.

Beh: $F_3(\alpha) = K \iff \alpha \notin \F_{3^3},\F_{3^2}$ oder $\F_{3^1}$ 
Damit für ein $\alpha \in \F_{3^6}$ $\F_3(\alpha) = \F_{3^6}$ sein kann, ist notwendig, dass $\alpha \notin \F_{3^3},\F_{3^2}, \F_{3^1}$, also kein Element eines echten Teilkörpers von $K$ ist. (sonst wäre $F_{3^6}$ nicht der kleinste Erweiterungskörper)
In dem Fall ist der einzig übrig bleibende, d.h. der kleinste erzeugte Zwischenkörper, von $\F_{3^6} |\F_3$, der $\alpha$ enthält $\F_{3^6} = K$.

Der Schnitt von $\F_{3^3}$ und $\F_{3^2}$ ist wieder ein Körper, muss also der größte gemeinsame Teilkörper (d.h. $\F_{3^1}$) sein.
Alle anderen Elemente sind verschieden. Deshalb gibt es $3^3 + 3^2 - 3^1 = 33$ Elemente in $\F_{3^3},\F_{3^2}$ oder $\F_{3^1}$.
Damit gibt es $3^6 - 33$ Elemente, die in $\F_{3^6}$ aber nicht in $\F_{3^3},\F_{3^2}$ oder $\F_{3^1}$ liegen.

## c) 
$K^\times$ hat $3^6-1 = 728$ Elemente. Nach VL sind Teilmengen endlicher Multiplikativer Gruppen zyklisch. D.h. $K^\times \cong C_{728}$.
Die Untergruppen der Zyklischen Gruppen sind geau die Zyklischen Gruppen deren Ordnung $728$ teilen.
$728 = 2 * 2 * 2 * 91 = 2*2*2*7*13$.
Die Ordnungen sind $\{728, 364, 182, 104, 91, 56, 52, 28, 26, 14, 13,  8,  7 , 4, 2, 1\}$ und vermutlich noch andere, ich war zu faul alle durchzugehen

## d)
Sei $\alpha$ ein Erzeuger von $C_{728}$
Nach Vorlesung erzeugt $\alpha^i \in C_{728}$ für $i \in \{1, ..., 728\}$ die Zyklische Gruppe genau dann, wenn $ggT(728, i) = 1$, also teilerfremd sind. Das ist nach Definition das Ergebnis der Eulerschen Phi-Funktion $\varphi(728) = \varphi(2^3)\varphi(7)\varphi(13) = 4*6*12 = 288$.
%%

# Aufgabe 3
%%
## a) 
In $\F_2[x]:x^6 + 1 = (x^3+1)^2$
In $\F_3[x]: x^6 + 1=(x^2+1)^3$
Ist das Polynom reduzibel.

Alternativ kann man auch [[Freshmans Dream]] anwenden.

## b)
$|\F_{p^2}^\times| = p^2-1 = (p+1)(p-1)$.
$p$ ist eine Primzahl $\neq 2$ und damit ungerade. D.h. $(p-1)$ und $(p+1)$ sind durch gerade. $\implies p^2-1$ ist durch vier teilbar.

$p$ ist als Primzahl $ \neq 3$ nicht durch drei teilbar. $\implies (p-1)$ oder $(p+1)$ ist durch drei teilbar.
$\implies p^2-1$ ist durch 3 und 4, also auch durch $ggT(3, 4) = 12$ teilbar.
%%

## Aufgabe 3 c)
Nullstellen von $f$ in $\F_5$. 
2 ist eine Nullstelle: $2^6 + 1 = 64 + 1 = 5 = 0$.
$(x^6+1)/(x-2) = x^5 - 2x^4 + 4x^3 - 8x^2 + 16x - 33 = x^5 +3x^4 + 4x^3 +2x^2 + x + 3$

Element hat Ordnung 12, wenn sie das $p^2-1/12$-te (mal k) Element sind.

$\alpha$ ist ein ELement aus $\F_{p^2}$ und Ordnung 12, also Nullstelle von $f$. 
Damit gilt $\mu_{\alpha, \F_2}|f$.
Bestimme nun den Grad des Minimalpolynoms.
Offensichtlich ist $\F_2(\alpha)$ ein Zwischenkörper von $\F_{2^2}|\F_2$.
Damit gilt die Gradformel
$$2 = [\F_4:\F_2] = [\F_{4}:\F_2(\alpha)] \cdot [\F_2(\alpha):\F_2]$$
Damit muss $[\F_2(\alpha):\F_2]$ 1 oder 2 $< 6$ sein. $f$ ist reduzibel.

%%
# Aufgabe 4
## a)
$d = ggT(a, b)$, also gibt es ein $a'm b'$ mit $a = a'd$ und $b = b'd$.

### cd teilt ac, bc
Zeige $\frac{ac}{cd} \in R$.

Im Quotientenkörper $K$ existert das Element $\frac{ac}{cd}$ und es gilt:
$$\frac{ac}{cd} = \frac{a'dc}{cd} = a' \in R$$
Somit gilt $\frac{ac}{cd} \in R$. und $cd$ teilt $ac$.
Der Beweis für $bc$ erläuft analog.

### cd ist ggT
Sei $e \in K$ ein Teiler von

%%

