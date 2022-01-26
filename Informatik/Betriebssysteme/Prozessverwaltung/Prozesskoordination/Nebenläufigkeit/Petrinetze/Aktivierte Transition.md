# Beschreibung
EIne Transition eines [[Petrinetz]] heißt **aktiviert** unter einer Markierung $M$, wenn sie passieren kann, d.h., wenn die nötigen Marken zur Ausführung der Transition da sind und keine Kapazität durch die Ausführung übertreten wird.

*Eine Markierung ist eine Hashmap, die jeder Stelle die Anzahl der Marken zuordnet. Eine Markierung beschreibt also den Zustand des ganzen Netzes.*

# Feuern von Transitionen
Transitionen feuern sequentiell, also nicht zeitgleicht.

#Betriebssysteme 