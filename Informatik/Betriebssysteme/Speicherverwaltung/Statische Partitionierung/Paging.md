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
Ich lagere die Seite aus, die vor längster Zeit genutzt wurde. Dafür sortieren wir die Pages bei jedem Seitenaufruf so um, dass die zuletzt genutze Seite ganz oben steht. Dann ist die wenigsten genutze Seite unten.
4. **LFU (Least Frequently Used)**


#Betriebssysteme 


