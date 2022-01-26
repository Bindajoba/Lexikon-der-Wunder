## Beschreibung
Die **Komplexitätsklasse $\mathcal{P}$** ist eine [[Komplexitätsklasse (deterministisch)]], die alle [[Formale Sprache|Sprachen]] zusammenfasst, bei denen das [[Wortproblem]] schneller als [[Polynom|polynomiell]] festgestellt werden kann.

## Definition
Die Klasse $\mathcal{P}$ ist definiert als
$$\mathcal{P} = \bigcup\limits_{p \text{ Polynom}} TIME(p(n))$$

## Beispiele
- $n \log n$ hat polynomielle Komplexität, da $n \log n \in O(n^2)$
- $2^n$ hat keine polnomielle Komplexität
- $n^{\log n}$ hat keine polynomielle Komplexität

## Sprechweisen
- Ein Alpgorithmus ist **effizient**, wenn er polynomielle Komplexität hat
- Ein Problem ist **effizient lösbar**, wenn das Problem in $\mathcal{P}$ liegt

## Eigenschaften
- Die **Klasse P** ist eine Teilmenge der [[Komplexitätsklasse NP]]
Die Umkehrung ist aber [[P-vs-NP-Problem|noch nicht gelöst]]!

#FSK 