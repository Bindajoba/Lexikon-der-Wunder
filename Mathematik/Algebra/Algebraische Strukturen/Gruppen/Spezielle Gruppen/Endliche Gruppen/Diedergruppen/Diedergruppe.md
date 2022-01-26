# Beschreibung
Eine Diedergruppe beschreibt die [[Rotationssymmetrie|Rotations]]- und [[Achsenspiegelung|Achsensymmetrien]] eines [[Regelmäßiges Polygon|regelmäßigen Polygons]]

Diedergruppen eines $n$-Ecks werden mit $D_n$ bezeichnet.

# Aussehen
## Cayley-Diagramm
![[Cayley-Diagramm DiederGruppe.png]]

## Multiplikationstafel
![[Multiplikationstafel Diedergruppe.png]]

*Beobachte, dass die Tafel aussieht, als bestünden die Quadranten aus vier [[Multiplikationstafel]] von [[Zyklische Gruppe|zyklischen Gruppen]]. *

## Zykelgraph
![[Diedergruppe Zykelgraph.png]]
*Der Zykelgraph einer Diedergruppe besteht immer aus einem großen Ring der Größe $n$ und $n$ kleinen Ringen der Größe $2$*


# Definition
Sei $n\in \mathbb{N}$ mit $n \subseteq 3$. Dann wird die Untergruppe $D_n = \langle \sigma_n, \tau_n\rangle$ von $S_n$ die **$n$-te Diedergruppe** genannt.

*$\sigma$ ist der $n$-[[Zyklische Permutation|Zykel]]*


# Charakterisierungen
## Semidirketes Produkt
Für alle $n \in \mathbb{N}$ mit $n \subseteq 3$ gilt $D_n \cong \mathbb{Z}/n\mathbb{Z} \rtimes_\phi \mathbb{Z}/2\mathbb{Z}$.
Insbesondere ist $D_n$ eine nicht-abelsche [[Gruppe]] der [[Ordnung (Gruppe)]] $2n$.

# Eigenschaften
## Zusammenhang zu zyklischen Gruppen
$D_n$ hat doppelt so viele Elemente wie die [[Zyklische Gruppe]] $C_n$


## Semidirektes Produkt
Sei $n \in \mathbb{N}$ mit $n \geq 3$ eine Gruppe und $\{g,h\}$ ein [[Erzeugendensystem]] von  $G$, wobei $ord(g) = n, ord(h) = 2$ und $ghgh=e_G$ gilt.

Sei außerdem ein [[Gruppenhomomorphismus]] definiert:
$$\phi_n: \mathbb{Z}/2\mathbb{Z} \to Aut(\mathbb{Z}/n\mathbb{Z})$$ gegeben durch $\phi(\bar 0) = id$ und $\phi(\bar 1) = (gN)$ bla bla bla

Auf jeden Fall ist $G$ isomorph zum [[Semidirektes Produkt|Semidirekten Produkt]] $\mathbb{Z}/n\mathbb{Z} \rtimes_{\phi_n} \mathbb{Z}/2\mathbb{Z}$[^1]

Und das ist genau die Diedergruppe[^2]

# Beispiele
## Die Gruppe $D_2$
$D_2$ ist einfach die [[Klein 4-Gruppe]]

## Die Gruppe $D_3$
Wie man im Artikel über [[Neuverkabelung]] lesen kann, ist $D_3$ ein [[Semidirektes Produkt]] von $C_2$ und $C_3$:

![[Diedergruppe Beispiel D3.png]]

#Carter #Algebra 

[^1]: Gerkmann - Proposition 7.6
[^2]: Gerkmann - Folgerung 7.7