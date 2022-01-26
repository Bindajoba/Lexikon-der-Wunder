TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Die Buddy-Systeme sind interessante Hybride aus Statischer und Dynamischer Partitionierung.
Bei Buddy-Systemen erhält man die Partitionierung des Speichers, indem Speicher-Segmente sukzessiv in kleinere Segmente geteilt werden. (zum Beispiel halbiert)
![[Buddy System.png]]

# Struktur
Ein Speicher der Größe $2^N$ wird durch halbieren in Speicherblöcke der Größen $2^K$ geteilt. 
Die Größe der kleinsten erlaubten Speicherpartitionen wird mit $2^L$ bezeichnet ($L$ für Lower-Bound)
Die Größe der größten erlaubten Speicherpartitionen wird mit $2^U$ bezeichnet ($U$ für Upper-Bound)

Buddy-Systeme lassen sich gut durch ein Baum-Diagramm repräsentieren.
![[Buddy-System Baumdiagramm.png]]


Will man ein [[Prozess]] hinzufügen, so teilt man die Speicherbereiche so lange, bis der Prozess gerade so noch reinpasst.

Bezeichnung von Elementen. Praktischerweise teilt die erste Teilung den Speicher durch $2$. Hatte der Speicher die Größe $2^N$ und alle Elemente sind listenförmig durchummeriert, dann ist die erste Stelle der Ersten Hälftigen Elemente eine Null und die anderen eine 1.
Wiederholt man das ganze merkt man, dass beim durchwandern eines Linken Pfades die Elemente durch eine 0 addressierbar sind. 

#Betriebssysteme 


