TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Ene [[Körpererweiterung]] $L|K$ wird [[Galois-Erweiterung]] genannt, wenn sie [[Normal|normal]] und seperabel ist. Die Gruppe $Gal(L|K) = Aut_K(L)$ heißt dann die **Galoisgruppe** der Erweiterung $L|K$.[^1]


# Eigenschaften
## Normalteiler
Sei $M$ ein Zwischenkörper von $L|K$ und $U = Gal(L|M)$ die zugehörige Untergruppe von $G = Gal(L|K)$. Dann sind folgende Aussagen äquivalent:
1. Die Erweiterung $M|K$ ist normal
2. Die Untergruppe  $U$ ist Normalteiler von $G$

In diesem Fall erhalten wir durch $\sigma \mapsto \sigma|_M$ eine Abbildung $G \to Gal(M|K)$ und diese induziert einen natürlichen Isomorphismus $G/U \cong Gal(M|K)$

# Beispiele
## Galoisgruppe von Wurzel 2, 3
Bestimme die [[Galoisgruppe]] von $\Q(\sqrt 2, \sqrt 3)$.

Es wurde bereits mal gezeigt $\Q(\sqrt 2, \sqrt 3) = \Q(\sqrt 2 + \sqrt 3)$.
Finde das [[Minimalpolynom]] von $\sqrt 2+ \sqrt 3$.
$(x-\sqrt 2 - \sqrt 3) \to ((x-\sqrt 2)^2 - 3) = x^2 - 2\sqrt 2 x + 2 -3 = (x^2-1)-2\sqrt 2x$
$\to (x^2-1)^2-8x^2 = x^4-10x^2+1$

Man kann prüfen: $\sqrt 2 + \sqrt 3$ bildet einen $4$-dimensionalen Vektorraum und $\Q(\sqrt 2 + \sqrt 3)$ hat damit den Erweiterungsgrad $4$. Das gefundene Polynom ist also wirklich das Minimalpolynom.

Das Minimalpolynom hat vier verschiedene Nullstellen. Damit gibt es vier Homomorphismen, einen für jedes Bild von $\sqrt 2 + \sqrt 3$. Konkret:
- $\phi_1(\sqrt 2 + \sqrt 3) = \sqrt 2 + \sqrt 3$
- $\phi_2(\sqrt 2 + \sqrt 3) = \sqrt 2 - \sqrt 3$
- $\phi_3(\sqrt 2 + \sqrt 3) = -\sqrt 2 + \sqrt 3$
- $\phi_4(\sqrt 2 + \sqrt 3) = -\sqrt 2 - \sqrt 3$

Die [[Galoisgruppe eines Polynoms|Galoisgruppe]] von $f$ kann also nur die [[Zyklische Gruppe]] $C_4$ oder die [[Klein 4-Gruppe]] $V_4$ sein. Es sollte nicht so schwer zu erkennen sein, dass $\phi_1, \phi_2, \phi_3$ bei doppelter Hintereinanderausführung die Identität ergeben, was genau die Struktur von $V_4$ wiederspiegelt.

## Folgerung ihrer Auflösbarkeit
Ist eine Galois-Gruppe $L|K$ [[Auflösbare Gruppe|auflösbar]], d.h. es gibt eine [[Normalreihe]] für sie, dann gibt es wegen der Galois-Korrespondenz eine ähnliche Reihe von Körpererweiterungen:
$$K = K_0 \subset K_1\subset... \subset K_r = L$$
wobei für alle $i$: $K_{i+1}$ eine [[Normale Erweiterung]] von $K_i$ mit Primzahlgrad ist.
*Merke, wie die Reihe hier antiton im Vergleich zur Normalreihe der Gruppen benannt wurde.*




[^1]: Gerkmann - Definition 17.1


#Algebra 


