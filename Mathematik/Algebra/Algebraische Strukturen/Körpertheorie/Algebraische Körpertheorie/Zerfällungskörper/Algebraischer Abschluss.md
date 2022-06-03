TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Der Algebraische Abschluss ist der [[Erweiterungskörper]] der algebraisch abgeschlossen ist und sich aus Polynomen des ursprünglichen Körpers erzeugen lässt.

# Definition
Sei $K$ ein [[Körper]]. Ein Erweiterungskörper $L$ von $K$ wird algebraischer Abschluss von $K$ genannt, wenn $L|K$ algebraisch und $L$ algebraisch abgeschlossen ist.[^1]


# Charakterisierungen
$L$ ist ist ein Algebraischer Abschluss von $K$, genau dan wenn_

## Charakterisierung 1
Die Erweiterung $L|K$ ist algebraisch und jedes nicht konstante Polynom $f \in K[x]$ zerfällt über $L$ in Linearfaktoren.

## Charakterisierung 2
Die Erweiterung $L|K$ ist minial mit der Eigenschaft, dass jedes nicht-konstante Polynom $f \in K[x]$ in Linearfaktoren zerfällt. Es gibt also abgesehen von $L$ selbst keinen Zwischenkörper von $L|K$ mit dieser Eigenschaft

## Charakterisierung 3 (Folgerung)
Sei $S_K$ die Menge aller nicht-konstanten Polynome über $K$. $L$ ist ein Zerfällungskörper von $S_K$.[^2]

## Eindeutigkeit
Algebraische Abschlüsse eines Körpers $K$ sind bis auf [[Körperisomorphismus|Isomorphie]] eindeutig.[^3]




# Beispiele
## Zerfällungskörper aller Polynome über einen Grundkörper $K$
Durch den [[Zerfällungskörper]] $\tilde K$ aller Polynoms $S_K$ über einen Grundkörper $K$ erhält man den algebraischen Abschluss des Körpers.

**Beweis:**
1) $\tilde K$ ist offensichtlich algebraisch
2) Sei $f \in \tilde K(x)$ nicht-konstant, irreduzibel, o.b.d.A normiert und irreduzibel. Zeige: Dann $f$ hat eine Nulltelle in $\tilde K$
   $f$ hat eine Nullstelle $\alpha$ mit $f(\alpha) = 0$. Damit ist $\tilde K(\alpha) \mid \tilde K$ algebraisch $\implies \tilde K(\alpha) \mid K$ ist algebraisch. Damit hat $\alpha$ ein Minimalpolnom in $K$. Dieses Minimalpolynom muss in $S_K$ enthalten sein $\implies \alpha \in \tilde K$.
   



#Algebra 

[^1]: Gerkmann - Definition 14.6
[^2]: Gerkmann - Folgerung 14.8
[^3]: Gerkmann - Folgerung 14.11


