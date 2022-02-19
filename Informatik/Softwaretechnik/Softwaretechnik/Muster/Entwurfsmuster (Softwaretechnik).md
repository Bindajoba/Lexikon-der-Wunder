TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Muster sind Lösungen auf varable Probleme der Softwaretechnik.

Q: Was ist ein Pattern?
A: Ein Pattern ist eine standardisierte Lösung auf ähnliche, wiederkehrende Probleme der Softwareerstellung.
<!--ID: 1642761437403-->

# Bestandteile
Design Patters umfassen vier Maßgebliche Elemente:
1. **Name**
2. **Problemstellung**
Die Situation, in der das Pattern anzuwenden ist.
3. **Lösung**
Die Beschreibung des Patterns
4. **Konsequenzen**
Die Auswirkungen und Kompromisse, die man berücksichtigen muss

Q: Durch welche 4 Elemente können Entwurfsmuster beschreiben werden?
A: 1. Name
2. Problemstellung
3. Lösung
4. Konsequenzen
<!--ID: 1645260971863-->


# Vorteile
1. Entwurfmuster haben sich als Lösung auf Probleme bewährt.
2. Entwurfsmuster sind vielseitig anwendbar
3. Entwurfmuster bilden Bausteine höherer Abstraktion, über die man reden kann
4. Entwurfsmuster sind vermutlich anerkannte Lösungen auf Probleme

# Anwendung
Will man Entwurfsmuster anwenden kann man sich an diese Schritte halten, die von der "Gang of Four" definiert wurden.
1. Passende Objekte finden
2. Objektgranularität bestimmen
3. Objektschnittstellen spezifizieren
4. Objektimplementierung spezifizieren
5. Wiederverwendungsmechanismen einsetzen
6. Strukturen der Laufzeit beim Kompilieren abstimmen
7. Designänderung berücksichtigen

*Puh, das ist, um es englisch auszudrücken eine Mundvoll. Ich verstehe das nicht ganz. Ich denke, ich lerne nur die Pattern selbst. Das wird schon passen.*

# Klassifikation
## Zweck
Entwurfsmuster lassen sich in drei Bereiche unterteilen.

Q: In welche drei Zweckarten von Mustern lassen sich Entwurtfmuster klassifizieren?
A: - Erzeugungsmuster
- Strukturmuster
- Verhaltensmuster
<!--ID: 1645260972042-->



- **Erzeugungsmuster**
Beziehen sich auf der Erstellungsprozess von Objekten
- **Strukturmuster**
Wirken sich auf die Zusammensetzung von Klassen und Objekten aus
- **Verhaltensmuster**
Charakterisieren die Art und Weise der Interaktion von Klassen und Objekten sowie die Verteilung der Zuständigkeiten.

## Gültigkeitsbereich
Entwurfsmuster lassen sich weiter dadurch klassifizieren, ob sie primär auf Klassen oder auf Objekten angewendet werden.
- **Klassenbasierte Entwurfsmuster**
Werden durch Unterklassen an die Situation angepasst und sind vor dem Kompilieren fest
- **Objektsbasierte Entwurfmuster**
Werden durch das Instanziieren von Objekten angepasst und sind auch noch nach dem Kompilieren veränderbar

## Klassifikationstabelle
| Gültigkeit/Zweck   | Erzeugungsmuster     | Strukturmuster | Verhaltensmuster           |
| ------------------ | -------------------- | -------------- | -------------------------- |
| **Klassenbasiert** | [[Factory Method]]   | [[Adapter]]    | [[Template Method]]        |
| **Objektbasiert**  | [[Abstract Factory]] | [[Kompositum]] | [[Iterator]]               |
|                    | [[Singleton]]        | [[Proxy]]      | [[Observer]]               |
|                    |                      |                | [[State (Entwurfsmuster)]] |
|                    |                      |                | [[Visitor]]                           |




#Softwaretechnik 


