## Beschreibung
Das SAT Problem ist das erste Problem, dessen [[NP-Vollständigkeit]] man nachweist.
Alle anderen Probleme kann man dann auf dieses [[Reduktion (Sprache)|reduzieren]].

## Definition
Das **Erfüllbarkeitsproblem der Aussagenlogik** (kurz **SAT**) ist:
- gegeben: Eine Aussagenlogische Formel $F$
- gefragt: Ist $F$ [[Erfüllbarkeit|erfüllbar]], d.h. geibt es eine erfüllende Belegung der Variablen mit den Wahrheitswerten 0 und 1, sodass F den Wert 1 erhält.

Bzw.:
$$SAT = \{code(F)\in \Sigma^*: F \text{ ist erfüllbare Formel der Aussagenlogik}\}$$

## Eigenschaften
### Komplexitätsklasse NP
SAT hat die [[Komplexitätsklasse NP]] 

**Beweisskizze**
In die Aussagenformel werden alle möglichen Eingaben nichtdeterministisch gleichzeitig eingegeben. Dann werden alle Ergebnisse gleichzeitig ausgerechnet.


### NO-Vollständigkeit
**Satz von Cook**: SAT ist sogar NO-vollständig