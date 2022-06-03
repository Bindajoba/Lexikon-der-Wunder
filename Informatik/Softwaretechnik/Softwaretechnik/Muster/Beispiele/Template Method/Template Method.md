TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Die Template Method (Schablonenmethode) ist ein [[Entwurfsmuster (Softwaretechnik)]].

# Problemstellung
Man hat eine Gruppe von Klassen, die ähnliche Methoden haben. Man möchte eine Klasse erstellen, die diese Aufrufe generalisiert.

Die Template Method löst dieses Problem. Damit kann man Skelette von Methoden erstellen, die sich erst später variabel befüllen. 

Q: Wozu verwendet man das [[Template Method]]-Entwurfsmuster?
A: - Um Skelette von Methoden zu erstellen, die durch Unterklassen ausgefüllt werden
<!--ID: 1645454018686-->


# Struktur
Es schlägt die Erstellung einer Klasse vor, in der eine wichtige Methode ist.
Diese Methode ist als als Skelett von primitiven, kleineren (nicht implementierten/nicht vorgegebenen) Methoden programmiert.

Eine Unterklasse kann die komplexe Methode implementieren, indem die primitiven Methoden "ausgefüllt werden."


![[Template Method.png]]

# Beispiele
## Sandwich Beispiel
![[Template Method Beispiel.png]]
Ein Hoagie ist ein Sandwich. Die Vorgehensweise zum Erstellen eines Sandwich ist immer die gleiche. Ein Italian Hoagie braucht also nur spezielle Änderungen vornehmen.
Daher ist es sinnvoll, dass die Strukur der Methode ```makeSandwich()``` bereits in der Oberklasse definiert ist.

Mit den sogenannten **Hooks** (den unteren Methoden von Hoagie) kann man angeben, welche der Methode ausgeführt werden soll. (Falls man einen veganen Hoagie haben will).

```
public abstract class Hoagie {
	final void makeSandwich() {
		cutBun();
		if(customerWantsMeat()) {
			addMeat();
		}
		// ...
	}

}

```



#Softwaretechnik 


