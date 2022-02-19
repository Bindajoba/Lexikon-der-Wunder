TARGET DECK: Universität::Mathematik::Algebra

*Beim vorletzten Übungsblatt habe ich auf die Aufgabe 0 Punkte bekommen und der obere Code wurde eingekreist. Daher sehe ich mich verpflichtet, zu erklären was es damit auf sich hat:*
*Ich verwende zum Bearbeiten und zur Dokumentation meiner Vorlesungsmaterialien den Markdown-Editor Obsidian. Diesen habe ich mit der Karteikartenapp Anki synchronisiert, sodass ich in den Vorlesungsdateien Fragen und Antworten im Format Q: Frage/A: Antwort formulieren kann und diese automatisch in eine Karteikarte umgewandelt wird, die auf meinem Handy gespeichert wird. Da ich jedoch für meine unterschiedlichen Fächer getrennte Stapel zum Lernen haben will, muss ich zu Beginn jedes Dokuments festlegen, in welchen Stapel die später definierten Karteikarten kommen werden. (Oberer Pfad sagt, die Karte soll in den Uni-> Mathe -> Algebra-Stapel) Das bei jeder Seite hinzuschreiben ist allerdings eine Heidenarbeit, deshalb habe ich mir für Algebra-Notizen ein Template angefertigt, die mir den oberen Code immer mit generiert. Natürlich muss ich für Übungsblätter dieses Template nicht laden. Die Sache ist: mit diesem Template werden auf Latex-Befehle geladen, auf die ich in Algebra und besonders beim Übungsblatt benötige. Mit den Befehlen kann ich beispielsweise \mathbb{Q} durch \Q abkürzen. Um konsequent zu bleiben, entferne ich den Pfad für gewöhnlich nicht. Ich hoffe du hast damit Verständnis.*

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\Z}{\mathbb Z}$



# Aufgabe 1
## a)
$|\F_{125}| = 124 = 2*62 = 4*31$
Die Zyklische Gruppe der Ordnung 124 hat Untergruppen der Ordnung $1, 2, 4, 31, 62, 124$.
Es gibt demnach nur erzeugende Elemente für Untergruppen dieser Ordnungen. Für alle anderen gibt es keine
- $n=124:$ Die Anzahl der Elemente errechnet sich mit der Eulerschen $\varphi$-Funktion. Das geht, da die Gruppe zyklsísch ist und maximal eine Untergruppe einer Ordnung $d$ haben kann, die dan ebenfalls zyklisch ist.
$\varphi(124) = \varphi(4)\varphi(31) = 60$.
- $n = 62: \varphi(62) = 30$
- $n=31: \varphi(31) = 30$
- $n=4: \varphi(4) = 2$
- $n=2: \varphi(2) = 1$
- $n = 1$: Nur das neutrale Element

## b)
$K^\times$ ist zyklisch und lässt sich somit durch einen Erzeuger $\beta$ beschreiben.
D.h. $A_n := \{\alpha^n: \alpha \in K^\times\} = \{(\beta^i)^n: i \in \{0, ..., 123\}\} = \{(\beta^n)^i: i \in \{0, ..., 123\}\}$
Die Menge $A_n$ ist also die Größe der Untergruppe, die durch $\beta^n$ erzeugt wird.

Ist $g$ ein Element der Ordnung $124$, dann gilt nach VL:
Für ein $i$ gilt $ord(g^n) = \frac{124}{ggT(124, n)}$

Für alle $n \in \mathbb{N}$ mit $ggT(124, n) = 1$ gibt es 124 Elemente mit der oberen Bedingung aus b). Den Rest kann man explizit ausrechnen.

## c)
Die Anzahl der Elemente mit $[\F_5(\alpha): \F_5] = n$.

$\alpha \in K = \F_{5^3}$, $\F_5(\alpha)$ ist somit ein Zwischenkörper von $K|\F_5$.
Nach Vorlesung sind die einzigen möglichen Zwischenkörper die Körper $\F_{5^m}$ mit $m\mid 3$. 
Für $n \neq 1, 3$ gibt es kein Element $\alpha \in \F_{5^3}$ mit $\alpha \in \F_{5^3}$.

D.h. $[\F_5(\alpha): \F_5] = n \iff$ der kleinste Oberkörper von $\F_5$, der $\alpha$ enthält ist $\F_{5^n} $$\iff \alpha \in \F_{5^n}$ und $\alpha \notin \F_{5^i}$ mit $i < n$

- $n = 1$: Offensichtlich alle Elemente aus $\F_5$, das sind 5 Elemente
- $n = 3$: Die Anzahl der Elemente sind alle Elemente in $K$, nachdem man die Elementen seiner echten Unterkörper abzieht (also nur $\F_5$). Damit gibt es $120$ Elemente
## d)
Nach dem Tutorium ist $f = x^{5^3}-x$ ein Produkt aller irreduziblen, normierten Polynome, deren Grad $3$ teilt.
Die Polynome können daher nur Grad $1, 3$ haben.
- $n = 1$: Es gibt 5 normierte Polynome mit Grad $1$, die alle irreduzibel sind.
- $n = 3$: In $K$ zerfälllt $f$ in $125$ verschiedene Linearfaktoren. $5$ davon liegen in $\F_5$.
Damit bleiben $120$ Nullstellen übrig, die Nullstellen der irreduziblen normierten Polynome sind (die nach Ausschlussprinzip Grad $3$ haben müssen), aus denen $f$ sich ja zusammensetzt. Damit gibt es $120/3=40$ Polynome dritten Grades.

# Aufgabe 2
## a)
Durch Substitution $x^2 = u$ erhält man ein Polynom mit den Nullstellen $\frac{1 \pm \sqrt{5}}{2}$. Damit hat $f$ die Nullstellen $\sqrt{\frac{1 \pm \sqrt{5}}{2}}$ und $-\sqrt{\frac{1 \pm \sqrt{5}}{2}}$.

$\sqrt{\frac{1 + \sqrt{5}}{2}}$ ist eine reelle Zahl. Damit ist $\Q(\sqrt{\frac{1 + \sqrt{5}}{2}})$ ein Teilkörper von $\R$. $\sqrt{\frac{1 - \sqrt{5}}{2}}$ ist aber wegen $1-\sqrt{5} < 0$ nicht reell, also $\sqrt{\frac{1 - \sqrt{5}}{2}} \notin \Q(\sqrt{\frac{1 + \sqrt{5}}{2}})$

$f$ kann somit nicht in Linearfaktoren zerfallen.

## b)
$\Q(\alpha, i)$ mit exemplarischer Nullstelle $\alpha = \sqrt{\frac{1 + \sqrt{5}}{2}}$  von $f$ ist normal, wenn $f$ über $\Q(\alpha, i)$ in Linearfaktoren zerfällt.
Jede Nullstelle von $f$ liegt dann in $\Q(\alpha, i)$ erzeugbar.

Beobachtung: $\sqrt{\frac{1 + \sqrt{5}}{2}} \cdot \sqrt{\frac{ \sqrt{5}-1}{2}}= \frac{1}{\sqrt{2}}\sqrt{\sqrt{5}-1}\cdot\frac{1}{\sqrt{2}}\sqrt{\sqrt{5}+1} = 1$.
D.h. $\frac{1}{\alpha} = \frac{1}{\sqrt{\frac{1 + \sqrt{5}}{2}}} =\sqrt{\frac{ \sqrt{5}-1}{2}} \iff \frac{i}{\alpha} = \frac{i}{\sqrt{\frac{1 + \sqrt{5}}{2}}} =i\sqrt{\frac{ \sqrt{5}-1}{2}} = \sqrt{\frac{1 - \sqrt{5}}{2}}$ womit die Nullstelle $\sqrt{\frac{1 - \sqrt{5}}{2}}$ von $f$ als Quotient von $i, \alpha \in \Q(\alpha, i)$ in $\Q(\alpha, i)$ liegt.
Damit liegen auch die anderen Nullstellen $-\sqrt{\frac{1 + \sqrt{5}}{2}}, -\sqrt{\frac{1 - \sqrt{5}}{2}}$ in $\Q(\alpha, i)$.

Wählt man für $\alpha$ eine andere Nullstelle, dann kann man das Verfahren analog anwenden.

![[blatt12.pdf]]
## c)
Jede endliche Erweiterung $L|K$ vom Grad $n$ ist algebraisch. 
Desweiteren gibt es eine endliche Basis $\{\alpha_1,..., \alpha_n\} \subseteq L$ des $K$-Vektorraums $L$.
Bilde das Minimalpolynom $\mu_{\alpha_i, K}$ von $\alpha_i \in L$. Bezeichne die $m_i$-Nullstellen von $\mu_{\alpha_1, K}$ mit $\alpha_{i, j}$, wobei $j \in \{1, ..., m_i\}$ 
Das Polynom $\mu_{\alpha_1, K}...\mu_{\alpha_n, K}$, dass durch das Produkt aller Minimalpolynome entsteht hat die endlich vielen Nullstellen $\{\alpha_{1, 1}, ... \alpha_{1, m_1}, \alpha_{2, 1}, ..., \alpha_{n, m_n}\}$. Dessen Zerfällungskörper $Z = K(\alpha_{1, 1}, ... \alpha_{1, m_i}, \alpha_{2, 1}, ..., \alpha_{n, m_n})$ erhält man durch Adjunktion dieser Nullstellen.
Da in der Adjunktion auch die ursprünglichen Nullstellen $\alpha_i$ mit dabei waren, ist $Z|K$ eine endliche, normale Erweiterung.

![[blatt12.pdf]]

# Aufgabe 3
$'\implies':$ Zeige: Jede algebraische Erweiterung von $K$ ist separabel. $\implies$ $\varphi: K \to K, a \mapsto a^p$ ist surjektiv.

Sei $b \in K$ ein Bild von $\varphi$, zeige: Es gibt ein $a \in K$, sodass $\varphi(a) = a^p = b$. 

Sei $a \in K^{alg}$ eine Nullstelle des Polynoms $f := x^p-b \in K[x]$. 
Da $K$ Primzahlcharakteristik hat gilt Freshmans Dream: $(x-a)^p = (x^n) + (-a)^p =$
- für $p=2:(x-a)^2 = x^2 + (-a)^2 = x^2 + a^2 = x^2 + b = x^2 - b$ (wegen Charakteristik 2)
- für $p \neq 2:(x-a)^p = x^p + (-a)^p = x^p - a^p = x^p - b$

Nach Aufgabenstellung ist aber jede algebraische Erweiterung $L$ von $K$ separabel. Damit hat jedes irreduzible Polynom $g \in K[x]$ nur einfache Nullstellen.

Da $f$ aber ein Produkt aus Linearfaktoren $x-a$ ist, ist die einzig mögliche Zerlegung in irreduzible Polynome die Zerlegung in Linearfaktoren (da sonst ein Faktor eine mehrfache Nullstelle hätte)

Folglich ist $(x-a)$ ein Polynom $K[x]$ und damit auch $a \in K$.

$'\impliedby':$ Zeige: $\varphi: K \to K, a \mapsto a^p$ ist surjektiv. $\implies$Jede algebraische Erweiterung von $K$ ist separabel.

Zu Zeigen ist: Jedes irreduzible Pokyom in $K[x]$ hat nur einfache Nullstellen. Das gilt gdw. wenn für alle $b \in K^{alg}: \mu_{b, K}$ einfache Nullstellen hat. 

Sei $f$ ein in $K[x]$ irreduzibles, normiertes Polynom. Wir wollen zeigen, dass $ggT(f, f') = 1$. 
Angenommen, es gilt $ggT(f, f') \neq 1$, dann muss $ggT(f, f') = f$, denn angenommen es gäbe ein nichtkonstantes Polynom $g = ggT(f, f')$ mit $grad(g) < grad(f)$, dann wäre $f$ reduzibel.

Desweiteren gilt $f' = 0$, den wäre $f'$ ein nichtkonstantes Polynom mit $grad(f')<grad(f)$, hätten $f'$ und $f$ einen gemeinsamen Teiler oder wären Teilerfremd (d.h. $ggT(f, f') = 1$ im Widerspruch zu oben)
$f$ ist nach Voraussetzung normiert $f' = 0$ hat als Folge, dass der Leitterm von $f$ eine $np$-Potenz (mit $n \in \N$) ist. Da $K$ ein Körper und damit ein Integritätsbereich ist, kann die Ableitung eines nichtkonstantes Monoms $a_ix^i$ von $f$ nur dann $0$ sein, wenn beim Ableiten der Koeefizient mit $0$ multipliziert wird. Dazu muss der Exponent $np$ mit $n \in \N$ sein.
$f$ hat also die Form:
$$f = b_{np}x^{np} + b_{(n-1)p}x^{(n-1)p} +... + b_{2p}x^{2p} + b_1x^p + b_0$$
Jedes Element $b_{ip}, i \in \{0, n\}$ ist ein Element aus $K$. Da der Frobenius-Homomorphismus surjektiv ist, gibt es eine $p$-te Wurzel $a_{ip}$, sodass $\varphi(a_{ip}) = (a_ip)^p = b_{ip}$
$f$ lässt sich umschreiben:
$$\begin{align}f &= a_{np}^px^{np} + a_{(n-1)p}^px^{(n-1)p} +... + a_{2p}^px^{2p} + a_1^px^p + a_0^p \\ &= (a_{np}x^{n})^p + (a_{(n-1)p}x^{(n-1)})^p +... + (a_{2p}x^{2})^p + (a_1x)^p + a_0^p \\
 &= \left(a_{np}x^{n} + a_{(n-1)p}x^{(n-1)} +... + a_{2p}x^{2} + a_1x + a_0\right)^p
\end{align} $$
was man durch wiederholtes Anwenden von Freshmans Dream erhält.
Offensichtlich ist $f$ aber nicht mehr reduzibel, was einen Widerspruch zur Annahme erzeugt.
$\implies ggT(f, f') \neq 0 \implies ggT(f, f') = 1 \implies$ Jede algebraische Erweiterung von $K$ ist separabel.

# Aufgabe 4
## a)
$f = 2x(x^3+2x^2+2x+1)$
$g:=x^3+2x^2+2x+1$ hat als letzten und ersten Koeffizienten $1$. Angenommen $g$ hat eine rationale Nullstelle dann muss diese nach dem Satz über rationale Nullstellen entweder $1$ oder $-1$ sein. Einsetzen ergibt $g(1) = 6, g(-1) = 0$.
$g:(x+1) = x^2 + x + 1$
$x^2 + x + 1$ könnte weiter nur in zwei Linearfaktoren zerlegt werden. Wenn das ginge, dann müsste es 2 rationale Nullstellen haben Nach dem Satz über rationale Nullstellen hat es aber nur die möglichen Nullstellen $1$ und $-1$. Einsetzen zeigt aber, dass das keine Nullstellen sind. $x^2 + x + 1$ ist also in $\Q[x]$ irreduzibel. Damit lautet die vollständige Zerlgung
$$f = 2x(x+1)(x^2+x+1)$$
Die obere Zerlegung ist eine Zerlegung in in $\Q[x]$ irreduzible Polynome. Diese $\Z$ Polynome sind damit insbesondere in $\Z[x]$ irreduzibel.
![[blatt12.pdf]]

## b)
$f = x^3+ax^2-(3+a)x+1$ hat Grad $3$. Die einzige Zerlegung in nicht-konstante Polynome ist also eine Zerlegung in ein Polynom von Grad $1$ und $2$ (oder dreimal $1$).
In dem Fall muss es einen Linearfaktor aus $\Q[x]$ geben, der $f$ teilt. Dann muss $f$ eine rationale Nullstelle haben.

Angenommen, $f$ hätte eine rationale Nullstelle. Nach dem Satz für rationale Nullstellen können diese nur $1$ und $-1$ sein. Einsetzen ergibt aber $f(1) = -1, f(-1) = 2a+3$. 
Somit hat $f$ keine Zerlegung.



#Algebra 


