# Definition
Ein [[Ring]] $R$ mit $0_R$ als einzigen **Nullteiler** heißt Integritätsbereich.
Ringe, die keine Integritätsbereiche sind, sind ziemlich komisch.


# Eigenschaften
## Kürzungsregel
In jedem Integritätsbereich gilt die Kürzungsregel
Sind $a,b,c \in R$ mit $c \neq 0_R$, dann folgt aus $ac=bc$ die Gleichung $a=b$

## Charakteristik
Die [[Charakteristik (Ring)|Charakteristik]] eines Integritätsbereiches ist entweder gleich Null oder eine [[Primzahl]].

*Wäre die Charakteristik keine Primzahl, dann hätte der Ring mehrere [[Nullteiler]]*

## Existenz eines Quotientenkörpers
Zu jedem Integritätsbereich existiert ein [[Quotientenkörper]].[^1]

## Kleine Eigenschaften aus Lemma
Sei $R$ ein Integritätsbereich
1. Seien $a, a', b, b' \in R$, wobei $a,a'$ bzw. $b, b'$ miteinander [[Assoziierte Elemente|assoziiert]] sind und $a|b$ gilt. Dann gilt auch $a'|b'$
2. Jedes Element in $R$, das eine [[Einheit]] teilt ist selbst eine Einheit
3. Ein Element, das von einem Primelement geteilt wird ist keine Einheit.[^2]

## Nicht-Existente ggT
In Integritätsbereichen ist es möglich, dass der $ggT$ zweier Zahlen nicht definiert ist. Betrachte das untere Beispiel $\Z[\sqrt 3]$:
Die Zahl $a=4$ hat die Zerlegung
$$4 = 2*2 = (1+\sqrt{3})(1-\sqrt 3)$$
Die Zahl $b = 2(1+\sqrt 3)$ ist bereits in Zerlegter Form.

Offensichtlich sind $2$ und $(1+\sqrt 3)$ Teiler von $a$ und $b$. Es gibt aber keinen Teiler, der durch $2$ und $(1+\sqrt 3)$ geteilt wird.




# Beispiele
## Beispiel $\Z[\sqrt 3]$:
$R = \Z[\sqrt 3]$ ist ein Integritätsbereich.




#Zahlentheorie 

[^1]: Gerkmann - Satz 4.2
[^2]: Gerkmann - Lemma 11.2