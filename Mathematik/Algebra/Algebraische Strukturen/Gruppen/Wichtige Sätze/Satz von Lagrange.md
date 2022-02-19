# Satz
Sei $G$ [[Endliche Gruppe|endliche Gruppe]] und $U$ eine Untergruppe. 
Bezeichne mit $G : U$ die Anzahl der Nebenklassen von $U$.
Dann gilt:
$$|G|=(G : U)|U|$$
Insbesondere ist die Ordnung $|U|$ der Untergruppe immer ein Teiler der Gruppenordnung $|G|$[^1]

# Übungen
## Klausur 2018 Aufgabe 1
![[Klausur 2018 Aufgabe 1.png]]
### a)
Die Ordnung der erzeugten Untergruppen der Elemente muss die Ordnung von $\langle g, h, k \rangle$ teilen.
$\langle g, h, k \rangle$ ist also durch $2, 3, 5$ und damit durch $ggT(2, 3, 5) = 30$ teilbar. $\implies |\langle g, h, k \rangle| \geq 30$. Aber die Gruppe ist eine Untergruppe von $G$, d.h. $\leq 30$

### b)
Wäre es zyklisch, dann durch ein Element $(a, b), a, b \in \Z$ erzeugt. $\langle (a, b) \rangle  \{(na, nb): n\in \N\}$
Ist $a \neq 0$, dann ist aber $(a, 0)$ kein Element der Gruppe, denn dazu müsste $n = 0$ und wir erhalten das Element $(0, 0)$
Ist $b \neq 0$, dann ist $(0, b)$ nach dem gleichen Argument nicht in der Gruppe.
Ist $a, b = 0$: dann ist $(1, 1)$ kein Element der Erzeugten Gruppe.







#Algebra 

[^1]: Gerkmann - Satz 4.8