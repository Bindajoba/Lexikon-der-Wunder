TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Verklemmung (oder Deadlock) bezeichnet einen Zustand, bei dem sich alle [[Prozess|Prozesse]] in einer solchen Konstellation zur Anfrage von Ressourcen ([[Betriebsmittel]]) ausschließen, dass kein Prozess etwas tun kann.
Sie befinden sich in einem wechselseitigen Wartezustand



# Definition Petrinetze
Eine **Verklemmung** ist eine eine [[Markierung]], die keine Nachfolgemarkierungen hat.

*Das heißt, dass es keine [[Aktivierte Transition]] gibt.*

Jede Verklemung ist eine [[Teilweise Verklemmung]]

Q: Woran erkennt man eine Verklemmung in einem Erreichbarkeitsgraph? ([[Verklemmung]])
A: Es gibt keinen Nachfolgenden Knoten.
<!--ID: 1642897215651-->



# Bedingungen
Damit eine Verklemmung entstehen kann müssen einige Bedingungen erfüllt sein:
1. **Mutual Exclusion**: Mindestens 2 unteilbare Ressourcen
2. **Hold and Wait**: Prozess hält Ressource, während er auf eine andere wartet
3. **No Preemption**: Prozess kann Ressource nicht entzogen werden, während er sie hält

Q: Was sind die 3 Rahmenbedingung für einen Deadlock?
A: - Mutual Exclusion
- Hold and Wait
- No Preemption
- Zusatzbedingung : Circular Wait
<!--ID: 1643668653650-->



Des Weiteren muss der Prozess in die Verklemmungssituation kommen:
1. **Circular Wait**: Es entsteht eine zyklische Wartesituation

*Die ersten 3 Bedingungen sind aber für Programme des [[Multiprogramming]] essentiell und können kaum umgangen werden.*

# Prävention
Siehe [[Deadlockprävention]]

# Beispiel
## Philosophenproblem
Siehe [[Philosophenproblem]]

#Betriebssysteme 