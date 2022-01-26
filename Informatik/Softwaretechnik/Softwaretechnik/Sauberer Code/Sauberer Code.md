## Beschreibung
In einem Buch Clean Code wird ein [[Coding Standard]] beschrieben, durch den Code besonders sauber aussieht

## Erkennungsmerkmale
Sauberer Code ist:
- Angenehm zu lesen
- [[Broken Window Theory|Entmutigt weitere Fehler]]
- Vermittelt seinen Zweck
- Erlaubt Verbesserungen
- Sorgfältig
- Verhinderung von Redundanz
- Deckt alle Eingaben ab

## Allgemeine Richtlinien
- [[Aussagekräftige Namen]]

### Richtlinien für Funktionen/Methoden
Eine gute Definition einer Funktion zeichnet sich aus durch:
- Methoden sollten 3 Zeilen (im Skript <20 Zeilen) lang sein
	- In if- und for-Aufrufen sollte ein Funktionsaufruf stehen
- [[Step-down-rule]]
- Eine Abstraktionsebene pro Funktion
D.h. nicht .append(str); neben getHtml(); 
- [[Single-Responsibility-Prinzip]]
	- Nebeneffekte vermeiden
	- Keine Output-Argumente verwenden
- Methoden sollten maximal 2-3 Argumente entgegennehmen
- **Exception-Handling**
	- Try-Catch in seperate Funktion extrahieren
	- Exceptions Errors vorziehen


#### Argumente reduzieren
- Statt Flag-Argumenten lieber zwei verschiedene Funktionen
- Lieber object.edit(str) als edit(object, str)
- Konstante Argumente wenn möglich wegabstrahieren
- Mehrere Argumente zu einer Klasse zusammenfassen

### Richtlinien für Kommentare
Siehe [[Sauberer Kommentar]]

### Formatieren
- Spezifische Richtlinien des Gruppenprojekts beachten
- Nutze und beabeite automatisches Formatieren (Shortcuts)
- Gruppiere thematisch (z.B. alle getter beieiander) 

#Softwaretechnik 