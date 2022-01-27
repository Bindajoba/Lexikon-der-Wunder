TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$



# Aufgabe 1
## a)
$|\F_{125}| = 124 = 2*62 = 4*31$
Die Zyklische Gruppe der Ordnung 124 hat Untergruppen der Ordnung $1, 2, 4, 31, 62, 124$.
Es gibt demnach nur erzeugende Elemente für Untergruppen dieser Ordnungen.
- $n=124:$ Die Anzahl der Elemente errechnet sich mit der Eulerschen $\varphi$-Funktion:
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
Nach Vorlesung sind die einzigen möglichen Zwischenkörper die Körper $\F_{5^m}, m\mid 3$. Wegen der Vektorraumeigenschaft gilt $[\F_{5^m}:\F_5] = m$ 

D.h. $[\F_5(\alpha): \F_5] = n \iff$ der kleinste Oberkörper von $\F_5$, der $\alpha$ enthält ist $\F_{5^n} $$\iff \alpha \in \F_{5^n}$ und $\alpha \notin \F_{5^i}$ mit $i < n$

Die Anzahl der Elemente mit $[\F_5(\alpha): \F_5] = n$ sind damit die Anzahl der Elemente aus $\F_{5^n}$, die es nicht in Teilkörpern von $\F_{5^n}$ gibt.

- $n = 1$: Offensichtlich alle Elemente aus $\F_5$, das sind 5 Elemente
- $n = 2$: Es gibt kein Element $\alpha \in K$ mit $[\F_5(\alpha): \F_5] = 2$, denn $\F_5(\alpha)$ ist ein Teilkörper von $(K = )\F_{5^3}\mid \F_5$ was nicht geht, da sonst $\F_5(\alpha) = \F_{5^2}$ aber $2 \nmid 3$.
- $n = 3$: Die Anzahl der Elemente sind alle Elemente in $K$, nachdem man die Elementen seiner echten Unterkörper abzieht (also nur $\F_5$). Damit gibt es $120$ Elemente
- $n \geq 4:$ $\F_5(\alpha)$ ist ein Teilkörper von $K$ weshalb der Erweiterungsgrad von $\F_5(\alpha)$ bzgl. $\F_5$ kleiner sein muss als der von $K$ ($=3$). Es gibt also kein $\alpha \in K$ mit $n \geq 4$

## d)
Nach dem Tutorium ist $f = x^{5^3}-x$ ein Produkt aller irreduziblen, normierten Polynome, deren Grad $3$ teilt.
Die Polynome können daher nur Grad $1, 3$ haben.
- $n = 1$: Es gibt 5 normierte Polynome mit Grad $1$, die alle irreduzibel sind.
- $n = 3$: In $K$ zerfälllt $f$ in $125$ verschiedene Linearfaktoren. $5$ davon liegen in $\F_5$.
Damit bleiben $120$ Nullstellen übrig, die Nullstellen der irreduziblen normierten Polynome sind (die nach Ausschlussprinzip Grad $3$ haben müssen), aus denen $f$ sich ja zusammensetzt. Damit gibt es $120/3=40$ Polynome dritten Grades.

# Aufgabe 2
![[blatt12.pdf]]

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

## c)
Jede endliche Erweiterung $L|K$ vom Grad $n$ ist algebraisch. 
Desweiteren gibt es eine endliche Basis $\{\alpha_1,..., \alpha_n\} \subseteq L$ des $K$-Vektorraums $L$.
Bilde das Minimalpolynom $\mu_{\alpha_i, K}$ von $\alpha_i \in L$. Bezeichne die $m_i$-Nullstellen von $\mu_{\alpha_1, K}$ mit $\alpha_{i, j}$, wobei $j \in \{1, ..., m_i\}$ 
Das Polynom $\mu_{\alpha_1, K}...\mu_{\alpha_n, K}$, dass durch das Produkt aller Minimalpolynome entsteht hat die endlich vielen Nullstellen $\{\alpha_{1, 1}, ... \alpha_{1, m_1}, \alpha_{2, 1}, ..., \alpha_{n, m_n}\}$. Dessen Zerfällungskörper $Z = K(\alpha_{1, 1}, ... \alpha_{1, m_i}, \alpha_{2, 1}, ..., \alpha_{n, m_n})$ erhält man durch Adjunktion dieser Nullstellen.
$Z|K$ ist eine endliche, normale Erweiterung.

# Aufgabe 3
![[blatt12.pdf]]

$\implies:$ Jede algebraische Erweiterung von $K$ ist separabel. $\implies$ $\varphi: K \to K, a \mapsto a^p$ ist surjektiv
#Algebra 


