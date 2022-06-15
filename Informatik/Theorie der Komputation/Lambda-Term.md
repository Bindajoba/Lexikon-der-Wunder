TARGET DECK: Universität::Informatik::NaCo

# Beschreibung


# Definition
Sei $V$ eine Menge von Variablen ($V = \{'a', 'b', ...\}$). $\Lambda$ ist die Menge der validen Ausdrücke im $\lambda$-Kalkül gegeben durch die Induktion:
- **Variable**: Wenn $x \in V$, dann $x \in \Lambda$
- **Abstraktion**: Wenn $x \in V$ und $M \in \Lambda$, dann $(\lambda x. M) \in \Lambda$
- **Applikation**: Wenn $M \in \Lambda$ und $N \in \Lambda$, dann $(MN)\in \Lambda$

Jedes Element $L \in \Lambda$ wird ein $\lambda$-term gennant. Die freien Variablen eines $\lambda$-Terms $K\in\Lambda$, geschrieben $\mathfrak{F}(L)$ mit $\mathfrak{F}: \Lambda \to \mathscr{p}(V)$ ist Induktiv gegeben durch:
- Wenn $L=x$ für ein $x \in V$, dann $\mathfrak F (L) = \{x\}$,
- Wenn $L = (\lambda x. M)$ für ein $x \in V, M \in \Lambda$, dann $\mathfrak{F}(L) = \mathfrak{F}(M) \backslash \{x\}$,
- Wenn $L = (M \, N)$ für ein $M, N \in \Lambda$, dann $\mathfrak{F}(L) = \mathfrak{F}(M) \sup \mathfrak{F}(N)$

Q: Welche drei Typen von Lambda-Term Strukturelementen gibt es?
- Variable
- Abstraktion
- Applikation


#Natural-Computing 
