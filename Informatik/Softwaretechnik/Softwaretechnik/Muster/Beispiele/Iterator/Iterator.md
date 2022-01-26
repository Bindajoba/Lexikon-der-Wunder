TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Der Iterator ist ein [[Entwurfsmuster (Softwaretechnik)]].
Er dient dazu, durch eine Liste zu iterieren, ohne die Struktur der Liste zu offenbaren.


# Struktur
Der Iterator hat folgenden Aufbau:
![[Iterator.png]]
Wichtig sind die Methoden des Iterators:
- First() gibt das erste Element der Liste zurück
- Next() gibt das nächste Element der Liste zurück
- IsDone() ist true, wenn das letzte Element erreicht wurde
- CurrentItem() gibt das aktuelle Element zurück

So können alle Elemente der Liste durchgegangen werden.
Die Liste kann auch irgendwie den Iterator erstellen aber das habe ich nicht verstanden.
#Softwaretechnik 


