TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Paging bezeichnet das Vorgehen, [[Page|Pages]] in [[Frame|Frames]] zu laden.

# Paging-Strategien
- **Demand Paging**
Fehlt eine Seite im Hauptspeicher, so wird diese on demand aus dem HGS geladen
*Kelnner spült und bringt bei Anforderung einen Teller*
- **Demand Prepaging**
Fehlt eine Seite im Hauptspeicher, werden gleichzeitig mehrere Seiten geladen und verdrängt. Dadurch wird die Zahl der Zugriffe geringer gehalten als beim ersten Verfahren
*Kellner spült mehrere Teller auf einmal und bringt alle*
- **Look-Ahead-Paging**
Nicht nur bei Seitenfehlern, sondern auch bei anderen Kriterien können Nachladeoperationen stattfinden
*Kellner schaut, ob neue Kunden ein Teller brauchen könnten und wenn ja, holt er welche.*

Q: Welche Paging-Strategien gibt es?
A: - Demand Paging
- Demand Prepaging
- Look-Ahead-Paging
<!--ID: 1643668651418-->



# Policies
Bei Anwendung der Strategien gibt es verschiedene Policies/Vorschriften, die das Betriebssystem für den [[Virtueller Speicher]] macht.

- **Resident Set Management Policy**
Macht Vorschriften, ob sich eine feste oder eine variable Anzahl von Seiten eines bestimmten Prozesses während der Abarbeitung ständig im Hauptspeicher befinden sollte.
- **Fetch Policy**
Bestimmt ob Seiten nur nachgeladen dürfen, wenn ein Seitenfehler besteht oder auch, wenn kein Fehler besteht
- **(Placement Policy)**
- **Replacement Policy**
Hat mit der Ersetzung von Pages in Frames zu tun.

## Ersetzungsstrategien
1. **OPT (Optimalstrategie)**
Ich räume die Seite weg, die ich am längsten nicht mehr brauchen werde. *Zum Beispiel: Ich habe eine Winter, Fürhlings, Sommer und Herbstseite. Gerade ist Ende des Winters, also entferne ich die Winterseite, da ich diese erst nächstes Jahr brauche.* Optimal aber leider ist diese Strategie nicht realisierbar.
2. **FIFO (First in First Out Strategie)**
Die Seite, die ich am ich als erstes eingefügt habe, kommt raus
3. **LRU (Least Recently Used)**
Ich lagere die Seite aus, die vor längster Zeit genutzt wurde. Dafür erstellen wir eine Tabelle in der alle Frames verzeichnet sind. Diese sortieren jedem Seitenaufruf so um, dass die zuletzt genutze Seite ganz oben steht. Dann ist die wenigsten genutze Seite unten.
4. **LFU (Least Frequently Used)**
Es wird auf die Seiten zugegriffen, die die niedrigste Nutzungshäufigkeit hat. Diese Strategien sind theoretisch gut, haben sich aber in der Praxis nicht bewährt.
5. **Climb**
Bei jedem Aufruf steigt eine Seite eine Position höher. Die niedrigste Seite wird bei einem Seitenfehler ausgetauscht.
Neue Seiten kommen unten rein.
6. **Clock-Strategie**
Die Clock-Strategie kombiniert Aspekte aus LRU und LFU.
Die Frames haben die Struktur einer Uhr (modulo). Hat ein Speicher $3$ Frames, dann kann man sich das wie folgt visualisieren:
Eine Scheibe wird in drei Teile geteilt. Jeder Teil hat eine Zahl auf der Innen und auf der Außenseite. Die Zahl auf der Innenseite steht für den gespeicherten Frame, die Zahl auf der Außenseite ist ein Use-Bit.
Das Use-Bit beschreibt grob gesagt, ob die Seite vor kurzem benutzt wurde. (Wenn ja, wird sie nicht gelöscht, sondern eine andere). 
Des Weiteren gibt es einen Zeiger, der immer auf die Älteste Seite zeigt. 
![[Clock-Strategie.png]]
Zu Beginn werden die Frames ganz normal gefüllt. Ist der Speicher voll und es wird eine Seite benötigt, beginnt der Zeiger im Uhrzeigersinn zu rotieren.
Konkret: Er springt immer auf das nächste Feld. Jedes mal, wenn er ein 1-Use-Bit verlässt, setzt er es auf 0. Gelangt der Zeiger auf ein Frame mit einem ß-Use-Bit, wird dessen Seite ersetzt. So werden tendentiell alte Seiten ausgetauscht.
Das Use-Bit wird jedes Mal auf 1 gesetzt, wenn auf die Seite zugegriffen wird. (Auch beim ersten Einsetzen der Seite). Das Use-Bit sorgt dafür, dass keine häufig benutzten Seiten entfernt werden.

Q: Welche 6 Paging Ersetzungsstrategien gibt es?
A: - OPT
- FIFO 
- LRU (Least Recently Used)
- LFU (Least frequently Used)
- Climb
- Clock
<!--ID: 1643668651536-->

# Kenngrößen
Indem man 3 Informationen weiß, kann man ein Paging-System eindeutig festlegen. Die Kenngrößen sind:
1. Reference String
2. Distance String

#Betriebssysteme 


