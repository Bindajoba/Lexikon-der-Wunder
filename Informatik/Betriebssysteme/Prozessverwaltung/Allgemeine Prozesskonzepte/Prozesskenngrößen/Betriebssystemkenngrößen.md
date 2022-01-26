TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Diese Kenngrößen beschreiben, wie Prozesse den Prozessor oder andere Geräte auslasten und sind bilden damit eine Vergleichsmetrik.

# Kenngrößen
- **Prozessorauslastung**
Gibt an, wie stark der Prozessor durchschnittlich in einem Zeitraum ausgelastet ist
- **Speichernutzung**
Wie viel Speicher pro Minute benötigt wird
- Plattenauslastung
- Druckerauslastung
- Gesamtausführungsdauer
- Durchsatz
- [[Schedulingalgorithmus|Mittlere Antwortzeit]]

Q: Was gibt die Prozessorauslastung eines BS an? ([[Betriebssystemkenngrößen]])
A: Wie stark ein Prozessor durchschnittlich in einem Zeitraum ausgelastet ist.
<!--ID: 1642897217647-->


*Wenn ich es richtig verstanden habe, bedeutet eine Prozessorauslastung eines Prozesses, wie oft ein Prozess einen Prozessor beansprucht. z.B. 30% heißt. zu 30% der Zeit wird dieser Prozess auf dem Prozessor ausgeführt.*

# Berechnung
Es ist ein wenig umständlich, überall zu erklären, wie die Werte berechnet werden, deshalb machen wir das an generischen Beispielen.
![[Prozesskenngrößen Programme.png]]
CPU-Auslastunglastung:
- Job 1: 75%
- Job 2: 5%
- Job 3: 5%

## Prozessorauslastung
**[[Multiprogramming]]**
$$\frac{75 \%\cdot 20min +5\% \cdot15min + 5\%\cdot10min}{20min} = 81,5\%$$
*Im Skript werden einfach andere Beispielwerte verwendet. Hier sollte es aber richtig sein. Beachte, dass obere Rechnung davon ausgeht, dass alle Programme gleichzeitig laufen. Nach meinem Verständnis geht as aber nur, wenn die CPU dabei nicht bei 100% Auslastung ist.*

**[[Uniprogramming]]**
$$\frac{75 \%\cdot 20min +5\% \cdot15min + 5\%\cdot10min}{20min+10min+5min} = ...$$

## Speichernutzung
**Multiprogramming:**
$$\frac{50KBytes +100KBytes + 80KBytes}{20min} = 115 KBytes/min$$

Uniprogramming verhält sich wie oben.


#Betriebssysteme 


