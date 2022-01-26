## Beschreibung
Ein Dispatcher ist ein [[Prozess]], der einen Benutzer-Prozess, der sich in Bearbeitung befindet, unterbrechen und einen anderen Prozess dem Prozess zuweisen kann.

Dazu wird der [[Prozesskontext]] des alten Programms gespeichert und der des neuen geladen. (Siehe [[Prozesswechsel]])

*Obacht: Der Dispatcher entscheidet nicht über eine Prozessänderung, das macht der [[Scheduler]]. Der Dispatcher handelt nur auf dessen Anweisungen.*

#Betriebssysteme 