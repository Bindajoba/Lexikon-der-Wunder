TARGET DECK: Universität::Informatik::Lösch

# Beschreibung
Broy und Kuhrmann stellen ein eher traditionelleses Vorgehen zur Anforderungsermittlung dar.

# Vorgehen
Die [[Anforderungserhebung]] nach Broy ist komisch strukturiert aber ich würde es so aufteilen:
- Anforderungsermittlung
- Modellierung

## Anforderungsermittlung
Die Anforderungsermittlung besteht grundsätzlich aus folgenden Schritten:
- **Domänenanalyse**
- Allgemeiner Prozess der **Anforderungserhebung**
- **Lastenheft und Anwenderforderungen**
- **Anforderungsfestlegung und Dokumentation**

### Domänenanalyse
Bevor man die Anforderungen ermittelt sollte man sich mit der Domäne des Systems vertraut machen. Ist die Software ein Spiel, ein Messenger, eine Datenbank. Man soll sich mit den entsprechenden Gebieten vertraut machen. Der Einbezug eines [[Domain Expert|Domänenexperten]] ist dafür unverzichtbar.

### Anforderungserhebung
Die Anforderungserhebung wird durch folgendes Diagramm veranschaulicht:
![[OOAD Anforderungserhebung.png]]

Wie man sehen kann gliedert sich die Anforderungserhebung in 6 Schritte:
1. **Stakeholder und Ziele**
Warum und für welchen Zweck soll das System entwickelt werden?
Was ist seine wesentliche und was muss es nicht tun?
Was sind die Erfolgskriterien?
Zur Formulierung der Ziele hat sich das [[S.M.A.R.T.-Schema]] etabliert
2. **Kontext**
Was ist der Problembereich und die sich daraus ergebende Systemgrenze?
Welche Fachterminologie ist im Projekt erforderlich?
Gibt es Systeme, mit denen interagiert werden muss?
Welche Grundsätzlichen Qualitätseigenschaftn muss das System haben?
3. **Lösungsoptionen**
Welche Lösungsoptionen gibt es und worin unterscheiden sie sich?
Welche Lösungsoptionen versprechen die effizienteste Zielerreichung?
Welche Lösungsoptionen balancieren Ziele und Rahmenbedingungen am besten?
Welche Lösungsoptionen hat das Verwerfen bestimmter Lösungsoptionen?
4. **Definieren und Beschreiben von Anforderungen und Dienste**
Welches fachliche, logische Daten- und Prozessmodell soll dem System zugrundeliegen?
Wie sollen die fachlichen Schnittstellen beschaffen sein und welches Verhalten haben sie?
Wie sollen die erforderlichen Leistungsparameter des Systems gewählt werden?
5. **Risiken und Erfolgsfaktoren**
Mit welchen Risiken ist die Entwicklung des Systems verbunden?
Welche Erfolgsfaktoren gibt es und wie verhalten sich diese zu den Risiken?
Welceh Erfolgsfaktoren sind für die Systementwicklung maßgeblich und sind diese in den Anforderungen reflektiert?
6. **Weitere Nebenbedingungen**
z.B.: Infrastrukturen, technische und organisatorische Fragen 



### Lastenheft und Anwenderforderungen
Aus den oberen Anforderungen wird ein [[Lastenheft]] erstellt, welches die Anforderungen zusammenfasst.

### Anforderungsfestlegung und Dokumentation
Die Anforderungen werden festgelegt und dokumentiert. *Wobei, das doch schon im letzten Schritt passiert ist?*
Dazu kann man [[User Story Map|User Story Maps]] verwenden.


### Techniken für die Anforderungserhebung
#### Quellen für Anforderungen
Um an Anforderungen des Systems zu kommen, sollte man sich folgender Quellen bedienen:
- Stakeholder
- Ideen von Fachleuten
- Literatur und [[Randbedingung|Gesetze]]
- Existierende Systeme und deren Dokumentation
- [[Prototyping|Prototypen]]
- Marksumfeld (um konkurrenzfähige, spezielle Produkte zu erstellen)

Q: Was sind 2 mögliche Quellen für Anforderungen?
A: - Stakeholder
- Ideen von Fachleuten
- Literatur und Gesetze
- Existierende Systeme und deren Dokumentation
- [[Prototyping|Prototypen]]
- Marksumfeld (um konkurrenzfähige, spezielle Produkte zu erstellen)
<!--ID: 1645543054437-->



## Modellierung
Die Modellierung dient wahrscheinlich dazu, die Anfordeurngen in Softwaremodelle umzuwandeln.
Konkret werden [[Use-Case|Use-Cases]] in UML-Diagramme umgewandelt.

Der Schritt scheint mit somit der [[Anforderungsanalyse (Seemann)#Analyse|Analyse]] von Seemann sehr ähnlich. 
Der größte Unterschied besteht darin, dass die Use-Cases von Broy sehr ausformuliert sind.

Es scheint so, als hätte Broy eine Reihenfolge im Sinn gehabt, behauptet aber selbst, dass diese bei speziellen Projekten verändert werden sollte.

### Modellierung des logischen Datenmodells
Die Use-Cases werden in ein [[Klassendiagramm]] umgewandelt.

### Modellierung der Systemzustände
Die Use-Cases werden in ein [[Zustandsdiagramm]] umgewandelt.

### Modellierung als Sequenzdiagramm
Die Use-Cases werden in ein [[Sequenzdiagramm]] umgewandelt.

### Modellierung als Aktivitätsdiagramm
Die Use-Cases werden in ein [[Aktivitätsdiagramm]] umgewandelt.


## Qualitätssicherung für Anforderungen
Während der Implementierung muss immer wieder darauf geachet werden, ob das richtige System entwickelt wird, d.h. ob das System den gestellten Anforderungen entspricht.

### Prüfbare Anforderungen
Um diesen Prozess zu vereinfachen sollen schon die Anforderderungen *verifizierbar* formuliert werden. 
Dazu sollten folgende Aspekte der Anforderungen erfüllt sein:
- **Konsistenz**
Die Anforderungen sind widerspruchsfrei
- **Vollständigkeit**
Alle für das System wichtigen Aufforderungen wurden erfasst
- **Korrektheit**
Alle Anforderungen treffen valide Anforderungen
- **Eindeutigkeit**
Anforderungen sind klar und unmissverständlich formuliert
- **Überprüfbarkeit**
Anforderungen können überprüft werden
- **Änderbarkeit**
Änderungen an Anforderungen können in einer systematischen und kontrollierbaren Weise vorgenommen werden
- **Verfolgbarkeit**
Die Umsetzung der Anforderunge soll im ganzen Lebenszyklus des Projekts nachverfolgt werden können.
- **Priorisierung**
Anforderungen sollen gemäß ihrer Wichtigkeit geordnet werden

*Diese Qualitätsaspekte sind eine Verfeinerung des [[S.M.A.R.T.-Schema]] bzgl. der Messbarkeit*

Anforderungen, die diese Qualitätsaspekte nicht erfüllen, geben nach Broy einen Requirement-Smell ab. In seinem Buch ist das so beschrieben: *„A requirements smell is an indicator of a quality violation, which may lead to a defect, with a concrete indication and a concrete detection mechanism“*


Q: Nenne 5 von 8 Qualitätsaspekte für prüfbare Anforderungen ([[Anforderungserhebung (Broy)]])
A: - **Konsistenz**
- **Vollständigkeit**
- **Korrektheit**
- **Eindeutigkeit**
- **Überprüfbarkeit**
- **Änderbarkeit** 
- **Verfolgbarkeit**
- **Priorisierung**
<!--ID: 1642761437069-->


Q: Was ist ein Requirement-Smell? ([[Anforderungserhebung (Broy)]])
A: Ein Requirement ist ein Indikator für schlecht formulierte Anforderungen.
<!--ID: 1642761437178-->



### Validierung von Anforderungen
Die Prüfung auf Validität der Anforderungen wird als Validierung bezeichnet. Es dient der Frage: "Wird das richtige System entwickelt?", "Sind die erfassten Anforderungen zutreffend und vollständing?".

Die Validerung deckt sich damit mit der [[Software-Validierung]]

### Verifizierbarkeit von Anforderungen
Verifikation zielt darauf ab, für das entwickelte Softwaresystem nachzuweisen, dass es die dokumentierten Anforderungen erfüllt. (Ist das nicht genau das gleiche wie oben?!?!)

Aber generell gilt die Anforderungen hinreichend konkret zu formulieren, sodass eine eindeutige Verifikation möglich ist.




#Softwaretechnik 


