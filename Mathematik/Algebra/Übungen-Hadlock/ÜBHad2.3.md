TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\t}{\theta}$

# Aufgabe 1
Ist es möglich einen beliebigen Winkel zu fünfteln? (Vg. [[Dritteln eines Winkels]])

Wende die Additionstheoreme für sin und cos an, um $cos(5\theta)$ als Polynom zu schreiben:
$$\cos(5\theta) = \cos(\theta)\cos(4\theta) - \sin(\t)\sin(4\t)$$
Wir berechnen links und rechts einzeln:
$$\begin {align} 
\cos(4\t) &= \cos^2(2\t)-\sin^2(2\t)\\
&= 2\cos^2(2\t)-1 \\
&= 2(2\cos^2(\t)-1)^2-1\\
&= 8\cos^4(\t)-8\cos^2(\t)+1
\end{align}$$
$$\cos(\t)\cos(4\t) = 8\cos^5(\t)-8\cos(\t)+\cos(\t)$$

$$\begin{align} 
\sin(4\t) &= 2\sin(2\t)\cos(2\t)\\
&= 2(2\sin(\t)\cos(\t))(\cos^2(\t)-\sin^2(\t))\\
&= 4(\sin(\t)\cos(\t))(2\cos^2(\t)-1)
\end{align}$$
$$\begin{align} 
\sin(\t)\sin(4\t)
&= 4(\sin^2(\t)\cos(\t))(2\cos^2(\t)-1)\\
&= 4(1-\cos^2(\t))\cos(\t)(2\cos^2(\t)-1)\\
&= 4\cos(\t)(-2\cos^4(\t)+\cos^2(\t)+2\cos^2(\t)-1)\\
&= -8\cos^5(\t) + 12\cos^3(\t)-4\cos(\t)
\end{align}$$
Somit ist:
$$\begin{align}\cos(5\t) &= (8\cos^5(\t)-8\cos(\t)+\cos(\t)) - (-8\cos^5(\t) + 12\cos^3(\t)-4\cos(\t))\\
&= 16\cos^5(\t)-20\cos^3(\t)+5\cos(\t)\end{align}$$
Wähle $\t$, sodass $\cos(3\t) = \frac{5}{6}$ und substituiere $2\cos(\theta) = x$ und bringen eine Seite der Gleichung auf $0$
$$0 = x^5-5x^3+5x-\frac{5}{3}$$
$$0 = 3x^5-15x^3+15x-5$$
Nach dem Eisenstein Kriterium ist dieses Polynom irreduzibel und die Erweiterung hat Grad 5.
Es ist nicht konstruierbar, da die [[Konstruierbare Zahlen|Konstruierbaren Zahlen]] aus (mehrfachen) [[Quadratische Erweiterung|Quadratischen Erweiterungen]] erzeugt werden, wodurch ihr Erweiterungsgrad eine 2-Potenz ist. 

# Aufgabe 2
Ist die Menge aller drittelbaren Winkel abzählbar?

Gehe vor, wie beim [[Dritteln eines Winkels]]. Behauptung: Ein Winkel $3\t$ ist genau dann drittelbar, wenn 
$$\cos(3\t) = 4\cos^3(\t)-3\cos(\t)$$
nach $\cos(\t)$ lösbar ist und es einen Turm von Quadratischen Erweiterungen von $\Q(\cos(3\t))$ gibt, der $\cos(\t)$ enthält. D.h. $[\Q(\cos(3\t), \cos(\t)): \Q(\cos(3\t))] = 2^n$

Multipliziere oben beide Seiten mit 2, substituiere oben $x = 2\cos(\t)$ und $a = 2\cos(3\t)$
Dann erhält man:
$$0 = x^3-3x-a =: f_a$$
Damit eine Zahl konstruierbar ist, muss sein Minimalpolynom den Grad einer 2-Potenz haben. Ein Winkel $3\t$ ist drittelbar, wenn $x^3-3x-2\cos(3\t)$ reduzibel ist.
In dem Fall muss es ein Element aus $\Q(\cos(3\t)) = \Q(2\cos(3\t)) = \Q(a)$ als Nullstelle haben.
Jedes Element aus $\Q(a)$ lässt sich schreiben als $\frac{g(a)}{h(a)}$, wobei $g, h$ Polynome aus $\Q$ sind.

Prüfe ob das möglich ist:
$$f(\frac{g(a)}{h(a)}) = (\frac{g(a)}{h(a)})^3-3\frac{g(a)}{h(a)}-a = 0$$
und damit
$$g(a)^3-3g(a)h(a)^2-ah(a)^3 = 0$$
???



#Hadlock 