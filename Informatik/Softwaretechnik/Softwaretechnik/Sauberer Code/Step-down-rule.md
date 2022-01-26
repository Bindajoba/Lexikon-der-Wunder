## Beschreibung
Die **Step-down-rule** besagt, dass der Code einer Methode am besten unter der Methode aufgehoben ist, die sie ausführt.

Ruft eine Muttermethode zwei Kindmethoden auf, sollten diese in der richtigen Reihenfolge unter der Muttermethode deklariert sein.

Sollte das erste Kind wieder eine Kindmethode aufrufen, kommt diese nach oberem Prinzip unter Kindmethode 1.

