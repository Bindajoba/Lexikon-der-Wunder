# Fragestellung
Wenn man komplexe Zahlen in der Schreibweise $re^{2\pi i \cdot t}$ aber für $r$ und $t$ nur rationale Zahlen verwenden kann, was erhält man für eine Menge und welche Eigenschaften hat sie?

# Antwort von 11Hades11
Offensichtlich ist diese Menge (im Folgenden $M$) eine Gruppe bezüglich der Multiplikation. Sie ist aber kein Körper, da mit Addition auch die einzelnen Real- und Imaginärteile herauskommen können, die nicht rational sind. $$r e^{2\pi it}+re^{-2\pi i t}=2\cos(2\pi t)$$ Diese Zahl muss auch für $t\in\mathbb Q$ nicht rational sein. Die Gruppe $(M,\cdot)$ ist isomorph zur Gruppe $(\mathbb Q\times ([0,1)\cap \mathbb Q),\circ)$ mit der Verknüpfung $$(r,t)\circ (s,u)\mapsto(r\cdot s,(t+u)\operatorname{mod}1)$$ indem man nur Argumente von $t$ zwischen 0 und 1 zulässt, da die anderen den gleichen Zahlen entsprechen. Eine interessante Frage ist natürlich, was nun der kleinste Körper ist, der $M$ enthält. Da $M$ abzählbar ist, kann der Körper nicht mit den komplexen Zahlen übereinstimmen. Beliebige Summen der Zahlen in $M$ ergeben folgende Menge (vermutlich ein Körper): $$\{\sum\limits_{z\in N} z\ \vert\vert\ N\subset M,\ \vert N\vert<\infty\}=\{r\cos(2\pi t)+is\sin(2\pi u)\ \vert\vert\ r,s,t,u\in \mathbb Q\}=:\mathbb M$$ Gewissermaßen ist $\mathbb M$ eine komplexe Version der Menge $\{r\cos(2\pi t)\ \vert\vert\ r,s\in \mathbb Q\}$. Dies ist eine Art Produktmenge aus den rationalen Zahlen und dem Bild des Sinus unter den rationalen Vielfachen von $\pi$. $$\begin{align} \mathbb M&=\{a+ib\ \vert\vert\ a,b\in P\}\\ P&=\{c\cdot d\ \vert\vert\ c,d\in \mathbb Q,d\in \sin[R]\} \\ R&=\{\pi \cdot q\ ||\ q\in \mathbb Q\} \end{align}$$

## Summe zwei komplexer Zahlen
Sei $z_3 = z_1 + z_2 = r_1e^{i2\pi t_1} + r_2e^{i2\pi t_2}$
Gesucht ist der Betrag und das Argument von $z_3$. Der Betrag ist leicht mit $|z_1+z_2|$ zu errechnen.
Das Argument stellt sich als etwas komplizierter heraus.
Zerlegen wir $z_1 + z_2 = (z_1 + x_2)+iy_2 = (z_1 + \cos(2\pi t_2))+i\sin(2\pi t_2)$
![[Addition von reeller Zahl.png]]

$\beta$ lässt sich mit dem Tangens aus dem Verhältnis von Gegenkathete und Ankathete des Rechtwickligen Dreiecks berechnen, das im Bild eingezeichnet ist.
D.h.
$$\beta = \tan^{-1}(\frac{Im(z_1+x_2)}{Re(z_1+x_2)}) = \tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})$$
$z_1' := z_1 + x_2 = |z_1+x_1|e^{i\beta} = |z_1+x_1|e^{i\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})}$

Nun addieren wir die Imaginäre Zahl $iy_2$ dazu:
![[Additin von imaginärer Zahl.png]]
Wir erhalten die Formel
$$\frac{\pi}{2}-\beta = \tan^{-1}(\frac{Re(z_1'+iy_2)}{Im(z_1'+iy_2)}) = \tan^{-1}(\frac{Re(z_1')}{Im(z_1')+ \sin(2\pi t_2)})$$
Setzen wir $z_1' = z_1 + x_2 = |z_1+x_1|e^{i\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})}$ ein erhalten wir:
$$\beta = \frac{\pi}{2}-\tan^{-1}(\frac{Re(|z_1+x_1|e^{i\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})})}{Im(|z_1+x_1|e^{i\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})})+\sin(2\pi t_2)}) = \frac{\pi}{2}-\tan^{-1}(\frac{|z_1+x_1|\cos(\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)}))}{|z_1+x_1|\sin(\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})+\sin(2\pi t_2)})$$
Mit $\cos(\tan^{-1}(x)) = \frac{1}{\sqrt{1+x^2}}$ und $\sin(\tan^{-1}(x)) = \frac{x}{\sqrt{1+x^2}}$ könnten wir ein paar Trigonometrische Funktionen herausnehmen.
$$\frac{\pi}{2}-\tan^{-1}(\frac{

\frac{|z_1+x_1|}{\sqrt{1+\left(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})\right)^2}}

}{

\frac{|z_1+x_1|x}{\sqrt{1+\left(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)}\right)^2}}

+\sin(2\pi t_2)})$$


Somit gilt $$z_1 + z_2 = |z_1+z_2|e^{i\left(\frac{\pi}{2}-\tan^{-1}(\frac{|z_1+x_1|\cos(\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)}))}{|z_1+x_1|\sin(\tan^{-1}(\frac{\sin(2\pi t_1)}{\cos(2\pi t_1)+\cos(2\pi t_2)})+\sin(2\pi t_2)})\right)}$$
