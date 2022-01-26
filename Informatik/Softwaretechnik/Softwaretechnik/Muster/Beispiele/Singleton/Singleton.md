TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Mit dem Singleton-Pattern soll eine Klasseninstanz sichergestellt werden, auf die man von überall zugreifen kann.
Sie ist anwendbar, wenn es von einer Klasse nur ein Objekt geben darf.


# Struktur
![[Singleton Struktur.png]]

# Implementierung
```
class Singleton {
	public:
		static Singleton* Instance();
	
	protected:
		Singleton();

	private:
		static Singleton* _instance;

	Singleton* Singleton::_instance = 0;
	
	Singleton* Singleton::Instance () {
		if (_instance == 0) {
			_instance = new Singleton;
		}
		return _instance;
	}
};

```

# Bewertung
## Vorteile
- Kontrollierter Zugrif auf die einzige Instanz
Die Singleton-Klasse hat absolute Kontrolle, wie und wann darauf zugegriffen wird
- Eingeschränkter Namensraum
Verhindert Überfrachtung (?)
- Verbesserte Operationen und Darstellung
Singleton kann durch Unterklassen erweitert und spezialisiert werden (?)
- Variable Anzahl von Instanzen
Singleton muss sich nicht auf eine einzige Instanz beschränken.
- Mehr Flexibilität als bei Klassenoperationen
Modifikation ist leichter, als wenn alles statisch wäre


- 


#Softwaretechnik 


