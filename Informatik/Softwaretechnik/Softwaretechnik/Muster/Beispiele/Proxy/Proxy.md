TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Der Proxy ist ein [[Entwurfsmuster (Softwaretechnik)]]. 
Müssen immer wieder ressourcenlastiges Objekt geladen/erzeugt werden, wird das System verlangsamt.
Eine Lösung ist, statt der Objekte leichtere Stellvertreter/Proxys (wie Prewiews) zu laden. Erst wenn das das Objekt wirklich gebraucht wird, lädt der Proxy dieses.

# Struktur
![[Proxy Struktur Beispiel.png]]
![[Proxy Struktur B.png]]

# Anwendbarkeit
Der Proxy ist immer dann sinnvoll, wenn über einen simpel Pointer hinausgehenden Bedarf nach anpassungsfähigeren und intelligenteren Referenzierung eines Objekt besteht.
- Ein **Remote Proxy** stellt einen lokalen Stellvertreter für ein Objekt in einem anderen Adressbereich zur Verfügung (kann man verwenden, um Adressbeschränkungen zu umgehen)
- Ein **Virtual Proxy** erzeugt ressourcenlastige Objekte auf Anforderung. Siehe Beispiel aus Struktur
- Ein **Protection-Proxy** kontrolliert den Zugriff auf das Originalobjekt. Die Verwendung ist sinnvoll, wenn Objekte unterschiedliche Zugriffsrechte haben sollen.
- Eine **Smart Reference** dient als Ersatz für einen einfachen Pointer und führt beim Zugriff auf ein Objekt zusätzliche Operationen aus. 
Das kann verwendet werden, um Referenzen zu zählen, Objekte in den Speicher zu laden, zu überprüfen, ob das Objekt gesprett ist.

# Konsequenzen
## Vorteile
- Ein Remote Proxy kann verbergen, dass sich ein Objekt in einem anderen Adressbereich befindet
- Ein Proxy kann Sotware optimieren hervorrufen
- Erlaubt mehr Möglichkeiten beim Zugreifen auf das Objekt


# Implementation
*Ich lasse ab sofort die Implementationen weg, ich kann sowieso kein C++ lesen.*


#Softwaretechnik 


