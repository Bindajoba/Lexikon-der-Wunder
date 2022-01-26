TARGET DECK: Universität::Informatik::Betriebssysteme

## Aufrufarten
Q: Welche zwei Aufrufarten gibt es bei einer Prozedur?
A: - Announcement
- Invocation
<!--ID: 1642897218211-->


### Announcement
Announcement ist eine Prozedur ohne Ergebnisparameter. (wie void in Java)

### Invocation
Invocation ist eine Prozedur mit Ergebnisparameter. Beobachte, dass das Announcement ein Spezialfall des Announcements ist.


## Kommunikation mit Mutterprozedur
Kommunikation beschreibt die Mittel, mit denen sich das Hauptprogramm und das aufgerufene Unterprogramm Informationen, Parameter und Ergebnisse austauschen.

Dazu gibt es zwei Möglichkeiten:

Q: Welche zwei Möglichkeiten der Parameterübergabe an eine Prozedur gibt es?
A: - Verwendung eines Stack
- Verwendung spezieller Register
<!--ID: 1642897218396-->


### Spezielle Register
Winzige Speicherzellen, die zum Zwischenspeichern bestimmter Ergebnisse im Prozessor liegen.
Konret wird das RA-Register (Rücksprungadresse)  verwendet. So kann nach Ausführung der Prozedur bei einem RET Befehl (siehe unten) auf das Oberprogramm zurückgesprungen werden.
In einem solchen Register kann aber nur eine Adresse gleichzeitig gespeichert werden, was es nicht möglich macht verschachtelte Prozeduraufrufe zu implementieren.


### Stack
Wie der Name [[Stack]] impliziert, werden Daten auf einen Stapel gelegt. Diese können danach von anderen [[Programm|Programmen]] entnommen werden.

Das Speichern auf einem Stack wird aber anscheinend für rekursive Funktionen bevorzugt.
Wie ein solcher Stack aussieht ist beispielhaft bei [[Stack von MI]] erklärt. 


## Ausführung
Die Prozedur kann durch einen JUMP-Befehl ausgeführt werden. Dabei wird der Programmzähler auf die Adresse der Zieladresse setzt, wodurch das Unterprogramm als nächstes ausgeführt wird.

Wenn wir das aber so machen, wird die Adresse, von der gesprungen wird nicht gemerkt. Der Computer kann also nicht zum Hauptprogramm zurückspringen.
Daher gibt es einen CALL und RET-Befehl:

Für eine Detailliertere Beschreibung in einem exemplarischen Betriebssystem siehe: [[Prozedur von MI]] 

Q: Welche Befehle werden verwendet, um einen Sprung innerhalb eines Programms zu realisieren? ([[Prozedurerzeugung]])
A: - CALL
- RET
<!--ID: 1642897218553-->


### CALL-Befehl
Die Rückadresse kann entweder in einem speziellen Register oder in einem Stack gespeichert werden.

#### Spezieller Register
Um sich die Position des Hauptprogramms zu merken, wird die Adresse im [[Register]] **RA (Rücksprungadresse)** gespeichert.
Die Methode ist so definiert:
```
COMMAND CALL addr
BEGIN
	RA := PC + 1;
	PC := addr;
END
```

Q: Wofür steht die Registerabkürzung RA? ([[Prozedurerzeugung]])
A: Rücksprungadresse
<!--ID: 1642897218715-->


#### Stack
Um sich die Position des Hauptprogramms zu merken, wird die Adresse im Stack gespeichert.
Die Methode ist so definiert:
```
COMMAND CALL addr
BEGIN
	PUSH (PC + 1);
	PC := addr;
END
```

### RET-Befehl
Der RET-Befehl kehrt zum Hauptspeicher zurück. Genau wie bei CALL wird dazu auf ein Spezielles Register (RA) oder einen Stack zugegriffen.

Q: Welche zwei wesentlichen Möglichkeiten gibt es den RET-Befehl zu implementieren 
A:  - Mit Register RA und MOVE
- Mit Stack und POP
<!--ID: 1642897218865-->


#### Spezieller Register
Um sich die Position des Hauptprogramms zu merken, wird die Adresse aus dem Register **RA (Rücksprungadresse)** entnommen.
Die Methode ist so definiert:
```
COMMAND RET
BEGIN
	PC := RA;
END
```

#### Stack
Um sich die Position des Hauptprogramms zu merken, wird die Adresse aus dem Stack entnommen.
Die Methode ist so definiert:
```
COMMAND CALL addr
BEGIN
	PC := POP;
END
```
