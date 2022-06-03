TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Client-Server ist ein Verteilung-[[Architekturmuster]]. Es handelt sich hierbei nicht wirklich um einen Client und einen Server, sondern um eine Abstraktion davon.

Q: Wann wird die [[Client-Server Architektur]] verwendet?
A: Wenn eine Untere Schicht einer oberen Schicht einen Dienst anbietet.
<!--ID: 1645543050450-->


# Struktur
Client-Server ist eine Weiterentwicklung eines Schichtenmodells.
Da ist es üblich, dass [[Softwarekomponente]] auf einen Dienst einer tiefer liegenden Komponente zugreifen. Da ist es sinnvoll, ein Client-Server-Modell zu etablieren.
![[Client-Server Architektur.png]]
*A ist Client vom Server B und B ist Client vom Server C.*

# Übungen
## Übung SWT 13-1
Bei Client-Server-Architekturen gibt es zwei grundlegende Varianten: „thick clients“ und „thin clients“. Letzere führen keine eigenen Berechnungen durch und besitzen keine Funktionalität, außer vom Server gesendete Daten anzuzeigen und Benutzereingaben zurückzusenden. Erstere
enthalten dagegen eigene Funktionalität und greifen nur für bestimmte Dinge auf den Server
zu.
- Welche Vor- und Nachteile ergeben sich durch „thick“ bzw. „thin“ clients?
Thick-Client-Vorteile: Server benötigt weniger Berechnungen. Es müssen weniger Daten versendet werden, *erlauben direkte lokale und daher schnellere Reaktion auf Benutzereingaben.*
Thin-Client-Vorteile: Server kann entscheiden, welche Daten an der Client erhalten soll. Client muss wenig berechnen. Client-Software ist klein, Programm ist leichter wartbar, da Änderungen nur am Server vorgenommen werden müssen, *können gut für andere Sachen wiederverwendet werden (Browser)* 
- Für welche Art von Software eignet sich die jeweilige Architektur? Nennen Sie Beispiele!
Thick-Client: Videospiele
Thin-Client: Clouds, Interfaces für Rechenmaschinen, Zugriff auf Datenbanksysteme


#Softwaretechnik 