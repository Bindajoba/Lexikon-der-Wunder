TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Das Kompositum ist ein [[Entwurfsmuster (Softwaretechnik)]], welches wir schon in der Schule gemacht haben. Es wird genutzt, um in Datenstrukturen Enden anzuzeigen oder allgemeiner, um solche Datenstrukturen zu definieren.

# Struktur
![[Kompositum.png]]

Das Buch der [[Gang of Four]] beschreibt das Kompositum als Muster, um hierarchische Anwendungungen zu strukturieren. Z.B. Gui-Elemente: Manche Gui-Elemente sind Container für weitere Gui-Elemente (Bild) oder Blätter (Text, Rectangle) und enthalten keine weiteren Elemente.

# Bewertung
## Vorteile
- Es können sowohl komplexe als auch einfache Strukturen gleichermaßen entgegengenommen werden
- Die Schnittstellen von Komplexen und Einfachen Objekten ist genau die gleiche
- Ermöglicht das Hinzufügen neuer Komponententypen (Triangle, Gruppe).

## Nachteile
- Das Kompositum kann dazu führen, dass zu viele Freiheiten enttehen. Es ist nur schwer eine bestimmte Struktur zu erzwingen 

# Implementierung
```
class Composite; 
class Component {
	public:
	//...
	virtual Composite* GetComposite() { return 0; }
};

class Composite : public Component {
	public:
	void Add(Component*);
	// ...
	virtual Composite* GetComposite() { return this; }
};

class Leaf : public Component {
	// ...
};

```

```
Composite* aComposite = new Composite;
Leaf* aLeaf = new Leaf;

Component * aComponent;
Composite* test;

aComponent = aComposite;
if (test = aComponent->GetComposite()) {
	test->Add(new Leaf);
}

aComponent = aLeaf;

if (test = aComponent->GetComposite()) {
	test->Add(new Leaf);
	// Es wird kein Leaf-Objekt hinzugefügt
}
```


#Softwaretechnik 


