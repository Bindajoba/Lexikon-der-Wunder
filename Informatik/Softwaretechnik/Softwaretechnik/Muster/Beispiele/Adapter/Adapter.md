TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Adapter (auch Wrapper) dient dazu, eine Schnittstelle anzupassen, die sonst mit einem Client inkompatibel wäre. (Wie ein Adapter!)

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





#Softwaretechnik 


