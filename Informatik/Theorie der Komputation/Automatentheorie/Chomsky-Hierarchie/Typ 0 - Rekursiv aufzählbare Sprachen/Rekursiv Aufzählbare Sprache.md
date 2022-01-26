## Beschreibung
**Rekursiv aufzählbare Sprachen** oder **Typ 0**-Sprache ist eine Sprache, die durch eine [[Rekursiv Aufzählbare Grammatik|Typ 0 Grammatik]].

## Äquivalente Definition
Eine Sprache $L \subseteq \Sigma^*$ heißt **rekursiv aufzählbar**
- falls $L \neq \emptyset$
- falls es eine totale berechenbare Funktion $f: \mathbb{N} \to \Sigma^*$ gibt, sodass $L = \bigcup_{i \in \mathbb{N}} f(i)$
Man sagt dann "$f$ zählt $L$ auf".


## Eigenschaften
Eine Sprache ist genau dann **rekursiv aufzählbar** wenn sie 
- [[Semientscheidbare Sprache|semi-entscheidbar]] ist.
- [[Turingberechenbarkeit|Turing-berechenbar]] ist


## Beispiele
- Die Sprache $L = \{a^p:p \text{ ist eine Primzahl}\}$ ist rekursiv aufzählbar.
- Die Sprache $L = \{a^n:n \text{ ist keine Primzahl}\}$ ist rekursiv aufzählbar.
- Die Sprache $L = \{a^n:n \text{ ist Quadratzahl}\}$ ist rekursiv aufzählbar.
- Die Sprache $L = \{a^{2^n}:n \in \mathbb{N} \}$ ist rekursiv aufzählbar.

#FSK 