## Definition
### Definition Ordnung einer Gruppe
Sei $G$ eine [[Gruppe]].
Die Anzahl der Elemente $|G|$ von $G$ wird die **Ordnung von $G$** genannt

### Definition Ordnung eines Elements
Sei $G \in G$ ein Element einer Gruppe. Dann bezeichnen wird $ord(g) = |\langle g \rangle|$ als die Ordnung von $g$.

## Charakterisierungen
### Zyklische Charaktierisierung
Bildlich ist das die kleinste Anzahl, wie oft man $g$ potenzieren muss, sodass wieder sich selbst ergibt:
$$g^{ord(g)} = e_G$$

Offensichtlich erfüllt jedes Vielfache von $ord(g)$ die gleiche Gleichung.


## Folgerung
Ist $G$ eine zyklische Gruppe der Ordnung $n$, dann gibt es genau $\varphi(n)$ Elemente $h \in G$ mit $G = \langle h \rangle$

$\varphi$ ist die [[Eulersche Phi Funktion]].

### Reduzierte Definition
Sei $G$ eine [[Gruppe]] und $n \in \mathbb{N}$. Ein Element $g \in G$ hat genau dann die Ordnung $n$, wenn $g^n = e_G$ und für jeden Primteiler $p$ von $n$ jeweils $g^{n/p} \neq e_G$ gilt.[^1]

# Eigenschaften
## Endliche Zyklische Gruppe
Bei endlichen Zyklischen Gruppen, hat die Ordnung eine Menge interessanter Eigenschaften. Siehe dazu [[Endliche Zyklische Gruppe]]

# Übungen
## Klausur 2016 Aufgabe 2
![[Klausur 2016 Aufgabe 2.png]]
### b)
Darauf folgt $g^n = e$. Es gilt $(g^{-1})^n = (g^n)^{-1} = e$ aber nicht für kleinere $n$.

### c)
Die Ordnung ist der ggT der Zykellängen der disjunkten Zykel also 6.
$\sigma^{61} = \sigma^1 \implies$ Ordnung 6.


#Algebra 

[^1]: Gerkmann - Satz 3.8 