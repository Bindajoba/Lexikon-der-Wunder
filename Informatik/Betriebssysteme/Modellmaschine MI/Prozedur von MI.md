## Ausführung
Lass uns bei der [[Modellmaschine MI|MI]] eine [[Prozedur]] ausführen, betrachte dazu die [[Befehle von MI]]:

**Code des Hauptprogramm:**
```
4000 ...
..
40?? PUSH p_n bzw. p_(n+1)
..
4098 PUSH p_2
4099 PUSH p_1
4100 CALL 4500
4101 POP p_1
4102 POP p_2
..
..
41?? POP p_n bzw. p_(n+1)
```

**Code der Prozedur**
```
4500 PUSHR           # (1)
4501 MOVE 64+SP, R12 # (2)
4502 MOVE SP, R13    # (3)
..
???? MOVE R13, SP    # (4)
     POPR            # (5)
     RET             # (6)
```

Dies lässt sich in mehrere Abschnitte unterteilen.

### Speicherung der Argumente
```
40?? PUSH p_n bzw. p_(n+1)
..
4098 PUSH p_2
4099 PUSH p_1
```
Die Argumente $p_1, ..., p_n$ sowie das Feld für die Ausgabe $p_{n+1}$ werden auf den [[Stack von MI|Stack]] gelegt.

### Aufruf der Unterprozedur
```
4100 CALL 4500

```
Die Unterprozedur wird ausgeführt. Dabei wird die [[Prozedur|Rückkehradresse]] auf dem Stapel gespeichert.

### Prolog des Unterprogramms
```
4500 PUSHR           # (1)
4501 MOVE 64+SP, R12 # (2)
4502 MOVE SP, R13    # (3)
```
1. Sichert die Register R0 bis R14 auf dem Stack, der dadurch um 15 Speicherzellen wächst (beachte: die Adressen fallen dabei).
2. Addiert zum Wert des Stack-Pointers 64 Bytes; man erhält die Adresse der Speicherzelle, die 16 (= 64:4 wegen 4 Bytes Wortgröße) Zellen unterhalb der obersten Kellerzelle liegt. Die Zahl 16 setzt sich zusammen aus 15 Zellen für die Register und einer Zelle für die Zelle mit der Rücksprungadresse. Dies ist die Ablageadresse, die in R12 gespeichert wird.
Die **Ablageadresse R12** wird genutzt, damit das Unterprogramm auf die übergebenen Argumente zugreifen kann.
3. Sichert die **Basisadresse** des lokalen Datenraums in R13.
Den Platz oben drüber kann das Programm für Variablen nutzen.

### Epilog des Unterprogramms
```
???? MOVE R13, SP    # (4)
     POPR            # (5)
     RET             # (6)
```
4. Setzt den Stack-Pointer auf die “alte” Basisadresse zurück. Bei einer “sauberen” Programmierung wurde der Keller vollständig abgeräumt, und der Stack-Pointer enthält bereits vor Ausführung dieses Befehls die korrekte Adresse.
5. Versetzt alle Register wieder in den Zustand, den sie zum Zeitpunkt der Ausführung des PUSHR-Befehls hatten.
6. Realisiert den Rücksprung.

### Lesen der Ausgabe
```
4101 POP p_1
4102 POP p_2
..
..
41?? POP p_n bzw. p_(n+1)
```
Zuletzt nimmt das Programm die Eingaben, und noch wichtiger, die Ausgabe aus dem Stapel, damit diese weiterverarbeitet werden kann.



#Betriebssysteme 