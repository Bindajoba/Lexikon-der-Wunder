TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Adapter (auch Wrapper) dient dazu, eine Schnittstelle anzupassen, die sonst mit einem Client inkompatibel wäre. (Wie ein Adapter!)

# Problemsituation
Will man ein Objekt/Klasse in sein Programm einbinden, aber die Schnittstelle stimmt nicht überein, dann ist es sinnvoll einen Adapter zu verwenden. 

Q: Wozu verwendet man das [[Adapter]]-Entwufssmuster?
A: Um zwischen zwei verschiedenen Schnittstellen zu kommunizieren.
<!--ID: 1645454018814-->


# Struktur
## Objektadapter mit Kontext
Ein Zeichenprogramm soll Texte darstellen können. Dazu wird das Drittanbieter-Klasse TextView verwendet.
TextView ist aber kein Shape, kann also nicht perfekt in die Software eingegliedert werden. Als Lösung wird eine Klasse TextShape erstellt, welche ein Adapter ist.
Sie repräsentiert Text im Zeichenprogramm und bedient sich dazu der TextView.

![[Objektadapter mit Kontext.png]]

Unten wird das auf ein Patter verallgemeinert. Die Positionen der Klassen entsprechen dem Beispiel oben.

## Objektadapter
![[Ojektadapter.png]]


## Klassenadapter
![[Klassenadapter.png]]


# Beispiel
## Videospielroboter
![[Adapter Videobeispiel.png]]
Der EnemyRobot soll die Methoden eines EnemyAttackers haben. Also wird ein Adapter verwendet, der diese Methoden besitzt und die Methoden eines EnemyRobot zugreift.[^1]


# Konseqeuzen
Siehe GoF.



#Softwaretechnik 


[^1]: https://www.youtube.com/watch?v=qG286LQM6BU&list=PLhkg-R66TRTV1-mDPLQ1HL7Wk9dGRBgSd&index=1