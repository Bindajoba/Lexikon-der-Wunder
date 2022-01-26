## Beschreibung
Eine Zahl- oder Wortfunktion heißt **Turingberechenbar**, falls eine [[Turingmaschine]] die Funktion berechnen kann und das Ergebnis ausgeben kann.

## Definition
Sei $bin(n)$ die Binärdarstellung von $n \in \mathbb{N}$

Eine Funktion $f: \mathbb{N} \to \mathbb{N}$ heißt **Turingberechenbar**, falls es eine Turingmaschine gibt, sodass für alle $n_1, ..., n_k, m \in \mathbb{N}$
$$f(n_1, ..., n_k) = m \iff z_0bin(n_1)\#...\#bin(n_k) \vdash^* \square...\square z_e bin(m)\square...\square \text{ mit } z_e\in E$$

Eine Funktion $f: \Sigma^* \to \Sigma^*$ heißt **Turingberechenbar**, falls es eine Turingmaschine gibt, sodass für alle $u, v \in \Sigma^*$ gilt:
$$f(u) = v \iff z_0 u \vdash^* \square...\square z_e v \square...\square \text{ mit } z_e\in E$$

## Beispiele
- Die [[Nachfolgerfunktion]], die 1 zu einer Zahl addiert ist Turingberechenbar.
- Die [[Identität (Mathematik)]] ist turingberechenbar
- Die Überall undefinierte Funktion ist turingberechenbar

#FSK 