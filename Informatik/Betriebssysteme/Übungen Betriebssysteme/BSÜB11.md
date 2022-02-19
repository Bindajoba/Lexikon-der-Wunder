# Aufgabe Ü27
a)

| Bezeichner                | Zweck                                                                          |     |
| ------------------------- | ------------------------------------------------------------------------------ | --- |
| entnehmenFertig          | Gibt an, ob die Spülmaschine leer ist                                          |     |
| bestueckenFertig          | Gibt an, ob das Bestücken beendet ist                                          |     |
| spülenFertig              | Gibt an, ob die Spülmaschine fertig ist                                        |     |


b)

| Pseudocode                | Bedeutung                                           |
| ------------------------- | --------------------------------------------------- |
| init(entnehmenFertig, 1)  | Zu Beginn ist die Maschine leer                                                    |
| init(bestueckenFertig, 0) | Zu Beginn wurde noch nichts bestückt                |
| init(spülenFertig, 0)     | Zu Beginn hat die Spülmaschine nicht mal angefangen |

c)

```
Bestuecker() {
	while(true) {
		//auf leeren Geschirrspueler warten
		wait(entnehmenFertig);
		
		<Geschirrspueler mit Geschirr bestuecken>
	
		//Geschirrspueler den Start signalisieren
		signal(bestückenFertig);
	}
}

Geschirrspueler() {
	while(true) {
		//auf Signal zum Start warten
		wait(bestückenFertig);
	
		<Geschirr spuelen>

		//Fertigstellung signalisieren
		signal(spülenFertig);
	}
}

Entnehmer() {
	while(true) {
	
		//auf Geschirrspueler warten
		wait(spülenFertig);
		wait(spülmaschineFrei);
			
		<den Geschirrspueler entladen>;
		
		//leeren Geschirrspueler signalisieren
		signal(spülmaschineFertig);
		signal(entnehmenFertig);
	}
}
```

# Aufgabe Ü28
```
public class Lager {
    private int aepfel;
    private int apfelmus;

    public Lager(int aepfel, int apfelmus) {
		this.aepfel = aepfel;
		this.apfelmus = apfelmus;
    }

    public synchronized void aepfelEinlagern(int anzahl) {
        aepfel = aepfel + anzahl;
        System.out.println(anzahl + " Aepfel eingelagert, Anz. Aepfel:" + aepfel);
        notifyAll();
    }

    public synchronized void apfelmusEntnehmen(int id, int anzahl) throws InterruptedException {
        while (anzahl > apfelmus) {
            System.out.println("Identitaet " + id + 
					" muss warten. Anz. apfelmus:" + apfelmus);
			wait();
        }
        System.out.println(anzahl + " Apfelmus entnommen von " + id + 
					" , Anz. Apfelmus:" + apfelmus);
					
		apfelmus -= anzahl;		
    }

    public synchronized void aepfelEntnehmen(int anzahl) throws InterruptedException {
        while (anzahl > aepfel) {
            System.out.println("Koch muss warten. Anz. Aepfel:" + aepfel);
            wait();
        }
        System.out.println(anzahl + " Aepfel entnommen, Anz. Aepfel:" + aepfel);

		aepfel -= anzahl;

    }

    public synchronized void apfelmusEinlagern(int anzahl) {
		apfelmus = apfelmus + anzahl;
        System.out.println(anzahl + " Apfelmus eingelagert, Anz. Apfelmus:" + apfelmus);
        notifyAll();
    }
}

```


e)

notifyAll() weckt alle wartenden Prozesse, notify() weckt einen zufülligen wartenden Prozess.
Bei jedem Einlagern würde man 8 Äpfel hinzufügen. Da aber mit notify() nur (maximal) eine auf Apfelmus wartende Person gleichzeitig geweckt werden kann, kann es passieren, dass manche Arbeiter auf Apfelmus warten, obwohl gerade welcher im Lager ist!

# Aufgabe Ü29
a) i)
b) iii)
c) i)
d) iii)
e) ii)

#Betriebssysteme 


