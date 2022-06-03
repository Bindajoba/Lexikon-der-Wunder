TARGET DECK: Universität::Mathematik::Algebra

Hehe, Konstruierbarkeit von Polynomen ist irgendwie interessant aber eigentlich will ich mich jetzt auf Vorlesungsrelevante Sachen konzentrieren. Deshalb habe ich ein paar Seiten übersprungen. 

# Aufgabe 1
Lösungsformel für Polynome dritten Grades herleiten.
Ohne Einschränkung sei $f = x^3 + bx^2+cx+d$
Substituiere $x = y+L$.
$$\begin{align}f &= y^3 + (3L +b)y^2+(3L^2+2bL+c)y+(L^3+bL^2+cL+d)\end{align}$$
Setze $L = -\frac{1}{3}b$, um den zweiten Koeffizienten zu vernichten.
$$\begin{align}f &= y^3+(\frac{1}{3}b^2-\frac{2}{3}b^2+c)+(\frac{8}{27}b^3-\frac{1}{3}bc+d) \\&= y^3+(-\frac{1}{3}b^2+c)y+(-\frac{1}{27}b^3+\frac{1}{9}b^3-\frac{1}{3}bc+d)\end{align}$$
Formuliere, um mir das Arbeiten leichter zu machen nun um zu:
$$f = y^3+cy+d$$
Substituiere $y = z+\frac{K}{z}$:
$$\begin{align}f=(z^3 + 3Kz + 3\frac{K^2}{z}+ \frac{K^3}{z^3})+(cz+\frac{cK}{z})+d \end{align}$$
wird zu 
$$\begin{align}f&=(z^6 + 3Kz^4 + 3K^2z^2+ K^3)+(cz^4+cKz^2)+dz^3 \\
&=z^6 + (3K+c)z^4 + dz^3 + (3K^2+cK)z^2+K^3\end{align} $$
Setzen wir ein $K = -\frac{1}{3}c$:
$$\begin{align}f&=z^6 + dz^3 -\frac{1}{27}c^3\end{align} $$
Dieses Polynom können wir mit der Mitternachtsformel lösen:
$$z = \sqrt[3]{\frac{-d\pm\sqrt{d^2+\frac{4}{27}c^3}}{2}}$$
Die vorherigen Substitutionen waren $y = z-\frac{c}{3z}$ und $x = y - \frac{1}{3}c$. Vielleicht können wir sie rückgängig machen. 
$$y = \frac{ \sqrt[3]{\frac{-d\pm\sqrt{d^2+\frac{4}{27}c^3}}{2}}^2-c}{3 \sqrt[3]{\frac{-d\pm\sqrt{d^2+\frac{4}{27}c^3}}{2}}}$$
Die Formel habe ich nicht bekommen. Ich habe aber gezeigt, dass jedes Polynom dritten Grades durch Radikale auflösbar ist. Das war, was die Aufgabe verlangt hat.

# Aufgabe 3
Finde ein Polynom von Grad $n$ in $\Q$, dessen Zerfällungskörper einen kleineren Erweiterungsgrad als $n!$ hat.
Wähle $f = x^4+x^3+x^2+x+1$. $f$ hat als Nullstellen die $4$ Primitiven [[Einheitswurzel|Einheitswurzeln]] $\sqrt[5]{1}$. Diese kann man durch Multiplizieren ineinander umwandeln, heißt, beim Hinzufügen einer zerfällt das ganze Polynom. $f$ hat Grad $4$, womit der Erweiterungsgrad des Zerfällungskörpers auch $4 < 4!$ sein muss.





$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


#Hadlock 