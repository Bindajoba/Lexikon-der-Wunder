## Befehle
| Befehl          | Funktion                                                                                                                                                    |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PUSH val        | legt den Wert val auf den Keller                                                                                                                            |
| PUSH reg        | legt den Inhalt des Registers reg auf den Keller                                                                                                            |
| PUSHR           | sichert den gesamten CPU-Register-Kontext, d.h. die Inhalte der Register R0 bis R14 werden nacheinander auf den Keller gelegt                               |
| POP reg         | legt den Inhalt der obersten Kellerzelle ins Register reg                                                                                                   |
| POPR            | stelle den gesamten Register-Kontext wieder her, d.h. die Inhalte der obersten 15 Kellerzellen werden nacheinander in die Register R14 bis R0 zurückkopiert |
| MOVE addr, reg  | Kopiert die Adresse addr ins Register reg                                                                                                                   |
| MOVE reg1, reg2 | Kopiert den Inhalt (Wert) von reg1 ins Register reg2                                                                                                        |
| CALL addr       | Sprung zu addr und Sicherung der Rücksprungadresse auf dem Keller                                                                                           |
| RET             | Rücksprung zum Aufrufer                                                                                                                                                            |

#Betriebssysteme 