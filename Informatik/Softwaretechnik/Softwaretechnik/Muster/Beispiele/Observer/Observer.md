TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Der Observer ist ein [[Entwurfsmuster (Softwaretechnik)]]
Mit dem Observer-Muster können Objekte automatisch über Änderungen der Daten informiert werden.

![[Observer Beispiel.png]]
*Werden die Werte der Tabelle verändert, dann ändern sich die anderen Werte mit.*

# Struktur
Ein Observer-Pattern setzt sich aus einem Subjekt und beliebig vielen Observern zusammen. Bei jeder Zustandsänderung werden alle Observer benachrichtigt. Als Reaktion darauf wird jeder Observer das Subjekt kontaktieren, um seinen eigenen Zustand mit demjenigen des Subjekts zu synchronisieren. 
*Ich denke, genau so etwas brauche ich für Chasch. Der Server sendet den Spielbrettzustand an alle Spieler, ohne diese zu kennen.*

![[Observer Struktur.png]]

# Anwendbarkeit
Das Pattern epfiehlt sich in folgenden Situationen:
- Wenn eine Abstraktion zwei Aspekte besitzt und einer vom anderen abhängig ist. Die Kapselung in verschiedene Objekte gestattet ihre unabhängige Änderung und Wiederverwertung
- Wenn eine Modifikation an einem der Objekte das Ändern anderer Objekte erfordert und nicht bekannt ist, wie viele der anderen Objekte geändert werden müssen
- Wenn ein Objekt andere Objekte benachrichten soll, ohne zu wissen, um welches Objekt es sich handelt




#Softwaretechnik 


