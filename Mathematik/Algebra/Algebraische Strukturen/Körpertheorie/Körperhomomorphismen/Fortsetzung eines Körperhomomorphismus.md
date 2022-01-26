# Beschreibung
Eine Fortsetzung eine Körperhomomorphismus ist eine Erweiterung eines Körperhomomorphismus auf eine größere Definitionsmenge, welche auch ein [[Körper]] ist.

# Definition
Sei $L|K$ eine [[Körpererweiterung]] und $\phi: K \to \tilde K$ ein [[Körperhomomorphismus]] von $K$ in einen weiteren Körper $\tilde K$.
Ein Körperhomomorphismus $\psi: L \to \tilde K$ wird Fortsetung genannt, wenn $\psi|_K = \phi$ erfüllt ist.  

# Eigenschaften
## Eindeutigkeit
Sei $L|K$ eine [[Körpererweiterung]]. $S \subseteq L$ eine ein Erzeuger mit $L = K(S)$ und $\phi: K \to \tilde K$ ein [[Körperhomomorphismus]] in einen weiteren Körper $\tilde K$. Sind dann $\psi_1, \psi_2$ zwei Fortsetzungen mit $\psi_1|_S = \psi_2|_S$, dann gilt $\psi_1 = \psi_2$.

*D.h. ein Körperhomomorphismus ist durch Definition des Erzeugers eindeutig.*[^1]

## Fortsetzungssatz
Sei $\phi: K \to \tilde K$ ein [[Körperisomorphismus]]. Seien außerdem $L|K$ und $\tilde L | \tilde K$ Körpererweiterungen und $\alpha \in L$ ein über $K$ [[Algebraisches Element]] mit [[Minimalpolynom]] $f \in K[x]$. Ist dann $\tilde \alpha \in \tilde L$ eine Nullstelle von $\tilde f = \phi(f) \in \tilde K[x]$, dann gibt es eine eindeutig bestimmte Fortsetzung $\psi$ von $\phi$ auf $K(\alpha)$ mit $\psi(\alpha) = \tilde \alpha$. Dieser Homomorphismus $\psi$ definiert einen Isomorphismus zwischen beiden Körpern $K(\alpha)$ und $\tilde K(\tilde \alpha)$ 

*Cool dieser Satz zeigt dass wenn man die Nullstellen des Minimalpolynoms $\mu_{K, \alpha}$ vertauscht, dass dann der entstehende Körper $K(\tilde \alpha)$ isomorph zum vorherigen ist. Der nächste Satz verallgemeinert das auf beliebige Polynome.Und er ist eine Umkehrung. Schmarrn! Wann anders anzupassen*

**Konkretere Formulierung:**
$\phi: = id, K = \tilde K, L = \tilde L$
Sei $L|K$ eine Körpererweiterung und $\alpha \in L$ ein über $K$ [[Algebraisches Element]] mit [[Minimalpolynom]] $f \in K[x]$. Ist dann $\tilde \alpha \in L$ eine Nullstelle von $f$, dann gibt es eine eindeutig bestimmte Fortsetzung $\psi$ von $id$ auf $K(\alpha)$ mit $\psi(\alpha) = \tilde \alpha$. Dieser Homomorphismus $\psi$ definiert einen Isomorphismus zwischen beiden Körpern $K(\alpha)$ und $\tilde K(\alpha)$ 

## Anzahl der Fortsetzungen
Sei $\phi: K \to \tilde K$ ein [[Körperisomorphismus]]. Seien außerdem $L|K$ und $\tilde L | \tilde K$ Körpererweiterungen, $\alpha \in L$ algebraisch über $K$ und $f = \mu_{K, \alpha}$. Dann stimmt die Anzahl der Fortsetzungen $\psi: K(\alpha) \to \tilde L$ von $\phi$ überein mit der Anzahl der Nullstellen von $\tilde f = \phi(f)$ in $\tilde L$[^2]



#Algebra 

[^1]: Gerkmann - Satz 13.1
[^2]: Gerkmann - Satz 13.4