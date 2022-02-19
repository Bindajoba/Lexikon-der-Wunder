# Beschreibung
Ein Erzeuger erstellt Produkte und stellt die auf einen Speicher (mit begrenztem Platz). Parallel dazu entnimmt ein Verbraucher die Produkte aus dem Speicher und verbraucht sie.
Das Problem besteht darin, dass beide Prozesse synchronisiert werden müssen.

# Lösungen
## Semaphore
Das Problem kann gelöst werden, indem man 3 [[Semaphor|Semaphore]] verwendet:
- init(s, 1): Realisiert exklusiven Zugriff auf den Speicher
- init(b, 0): Vermittelt, wie viel Bestand da ist
- init(p, MAX): Vermittelt, wie viel Platz da ist (MAX ist der maximale Platz)

**Code:**
```
Erzeuger:
REPEAT
	<erzeuge Element>;
	wait(p);
	wait(s);
	<lege Element im Speicher ab>;
	signal(s);
	signal(b);

Verbraucher:
REPEAT
	wait(b);
	wait(s);
	<entnimm Element aus Speicher>;
	signal(s);
	signal(p);
	<verbrauche Element>;

```

Der Semaphor s wird benötigt, um zu modellieren, dass nur eine Person gleichzeitig auf das Lager zugreifen kann. Das könnte zum Beispiel passieren, wenn ein Bestand und ein Platz da ist. Gabe es den Semaphor s nicht, könnte das ablegen und entnehmen gleichzeitig passieren.



#Betriebssysteme 