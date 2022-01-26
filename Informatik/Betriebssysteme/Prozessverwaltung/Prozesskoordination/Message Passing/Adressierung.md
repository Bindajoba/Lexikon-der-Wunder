TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Bei der Adressierung geht es darum Nachrichten an Prozesse oder Datenstrukturen sicher zu versenden.
Dazu gibt es zwei Ansätze:

# Formen
Q: Welche Formen der Adressierung gibt es? ([[Adressierung]])
A: - Direkte Adressierung
- Indirekte Adressierung



## Direkte Adressierung
Die Nachricht wird direkt an den Zielprozess gesendet werden. Der Zielprozess kann dadurch für gewöhnlich angeben, von wem die Nachricht stammt.


## Indirekte Adressierung
Nachrichten werden nicht direkt versendet sondern an eine gemeinsam genutzte Datenstruktur, die temporär Nachrichten speichern kann. Einer oder mehrere Empfänger entnimmen die Daten dann aus dieser Struktur.
Diese Datenstruktur besteht im Wesentlichen aus einer Warteschlange und werden als **Mailboxen** bezeichnet.
*Der große Unterschied zur Direkten Addressierung ist, dass die destination die Mailbox, nicht der Zielprozess ist.*

Je nach [[Multiplizität]] haben die Mailboxen unterschiedliche Namen:
- 1:1: *Direkte Adressierung aber mit Mailbox dazwischen*
- n:1: **Port** (Mehrere Sender schicken an einen Port, ein Prozess entnimmt daraus Nachrichten)
- 1:n: **Broadcasting**
- n:m: **Mailbox**



#Betriebssysteme 


