## Beschreibung
Eine endliche [[Zyklische Gruppe]]

## Eigenschaften
### Untergruppen
Sei $G$ eine endliche zyklische Gruppe $g \in G$ mit $G = \langle g \rangle$ und mit $ord(G) = n$ 
Die verschiedenen Untergruppen sind gegeben durch $U_d = \langle g^m \rangle$ wobei $d$ die Teiler von $n$ durchläuft. Dabei gilt jeweils $|U_d|= \frac{n}{d}$

Es gilt $U_m \subset U_{m'}$ genau dann, wenn $m$ ein [[Teilbarkeit|Teiler]] von $m'$ ist.

### Isomorphie
Je zwei **endliche Zyklische Gruppen** gleicher [[Ordnung]] sind zueinander [[Isomorphismus|isomorph]][^1]

### Ordnung einer zyklischen Teilgruppe
Sei $G$ eine Gruppe und $g\in G$ ein Element der endlichen [[Ordnung (Gruppe)]] $n$
1. Für beliebiges $m \in \mathbb{Z}$ gilt $ord(g^m)=n$ genau dann, wenn $ggT(m,n)=1$ ist.
2. Ist $d \in \mathbb{N}$ ein Teiler von $n$, dann gilt $ord(g^m) = \frac{n}{d}$
3. Für beliebiges $m \in \mathbb{Z}$ gilt $ord(g^m) = \frac{n}{d}$ mit $d = ggT(m ,n)$

*Das kommt daher, dass $\langle g^m \rangle$ eine [[Zyklische Gruppe]], also die Rotation eines [[Regelmäßiges Polygon|regelmäßigen n-Ecks]] mit den Rotationswinkeln $\frac{m}{n}$ ist. Wenn $m = 2, n = 6$, dann muss man offensichtlich $g^m$ 3-mal anwenden (rotieren), um $e$ zu erhalten. Die Ordnung ist damit 3.*

*Hat man ein Achteck, dass man mit $\frac{6}{8}$ Umdrehungen rotieren will, dann ist jede Rotation gleich einer $\frac{3}{4}$ Rotation.*
*Offensichtlich erhält man mit 4 Rotationen alle Elemente der Gruppe.*

*Aus diesem Grund braucht man im allgemeinen Fall eine $ggT(m, n)$-fache Anwendung, um $e$ zu erhalten*

**Beweis:**
zu 3.)
Seien $m', n'$ sodass $m = m'd$ und $n = n'd$. Zu zeigen ist $ord(g^m) = n'$. Da $d$ ein Teiler von $n$ ist gilt $ord(g^d) = \frac{n}{d}=n'$. Ferner sind $m'$ und $n'$ teilerfremd. Damit lässt sich 1.) auf $g^d$ anwenden.
$\implies(g^d)^{m'} = n' \implies n' = g^{dm'} = g^m$



#Algebra 

[^1]: Gerkmann - Folgerung 3.12