## Beschreibung
Eine **linear beschränkte Turingmaschine** (auch **linear bounded automaton** **LBA**) ist eine [[Turingmaschine]], dessen Schreib-Lesekopf den Bereich der Eingabe auf dem Band nicht verlassen darf.

Damit das Ende des Bandes erkannt wird, wird das letzte Zeichen markiert.
Zur Markierung wird eine Kopie $\hat\Sigma$ des Alphabets $\Sigma$ benutzt.

Das Symbol links muss nicht markiert werden, da das die Turingmaschine selbst kann.

## Definition
Eine NTM $M = (Z, \Sigma \cup \hat{\Sigma}, \Gamma, \delta, z_0, \square, E)$ heißt linear beschränkt (LBA, linear bounded automaton), wenn für alle $a_1...a_m \in \Sigma^{+}$ und alle [[Turingmaschine#Konfiguration einer Turingmaschine|Konfigurationen]] $uzv$ mit $z_0a_1...a_{m-1}\hat{a}_m \vdash^*_m uzw$ gilt: $|uv|\leq m$[^1]

Die entstehende LBA ist im Regelfall **nicht-deterministisch**, sie kann sich also in mehreren Zuständen gleichzeitig befinden.

### Akzeptierte Sprache
Die durch $M$ akzeptierte Sprache $L(M)$ ist definiert als
$$L(M) := \{a_1...a_m \in \Sigma^*:z_0a_1...\hat{a}_m \vdash^*_M uzw \text{ wobei } u, v \in \Gamma^*, z \in E\}$$[^1]

## Eigenschaften
### Satz von Kuroda
Die [[Kontextsensitive Sprache]] werden genau von den LBA erkannt.[^2]
*Auf den Beweis habe ich keinen Lust. Er steht aber ausführlich im Skript.*

## Probleme
### Erstes LBA-Problem
Siehe [[Erstes LBA-Problem]]

### Zweites LBA-Problem
Das zweite LBA-Problem wurde von [[Sige-Yuki Kuroda|Kuroda]] formuliert und stellt die Frage, ob [[Kontextsensitive Sprache]] unter [[Formale Sprache#Komplement|Komplementbildung]] abgeschlossen sind.[^3]

#FSK 

[^1]: Sabel - Definition 6.3.1
[^2]: Sabel - Theorem 6.3.2
[^3]: Sabel - Theorem 6.5.1