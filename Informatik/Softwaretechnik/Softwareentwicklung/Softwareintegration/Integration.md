TARGET DECK: Universität::Informatik::SWT

 # Beschreibung
Nach Abschluss der Codierung und der Qualitätssicherung einzelner Programmmodule liegt die Software im Sinne der Realisierung weitgehend fertiggestellt vor.  Das darauf folgende Zusammenbauen des Systems wird **Integration** genannt.

Üblicherweise versteht man darunter eine Integration aller Komponenten gleichzeitig. Für eine kontinuierliche Integration siehe [[Continuous Integration]].

# Vorgehen
Das Integrieren wir üblicherweise in mehreren Schritten durchgeführt:
1. Prüfung der Einzelsysteme/**Modultest**
2. Integration der Einzelsysteme
3. Prüfung des integrierten Systems (Verifikation)/**Integrationstest**
4. Identifikation von Fehlern (Defekten)
5. Diagnose, Korrektur von Fehlern
6. Nachprüfung



## 1. Modultest
Der Modultest [[Software-Test|testet]] alle Module separat auf:
- Bugs und Fehler
- Spezifikation 


## 3. Integrationstest
Während der Modultest einzelne Einheiten isoliert betrachtet werden im Integrationstest die Einheiten im Zusammenspiel getestet.

### Methoden der Integration
Das kann unterschiedlich passieren und hängt davon ab, welches Integrationsmethode man verwendet.
Prinzipiell gibt es drei verschiedene Methoden:
- **Big-Bang**
Alle Komponenten werden fertiggestellt, auf einmal zusammengesetzt und getestet.
- **Bottom-Up**
Zu erst werden von anderen Modulen unabhängige Module getestet (meist auf der Datenschicht). Dann werden Module die auf getestete Module zugreifen angeschlossen und getestet. Dies wird fortgeführt, bis die Software fertig ist.
- **Top-Down**
Als erstes wird das Modul getestet, das in der Abhängigkeitshierarchie ganz oben steht. (meist die Präsentationsschicht). Dieses Moduls muss trotzdem auf Daten zugreifen. Dafür werden Dummies (was vermutlich das gleiche wie ein [[Mock]] ist) verwendet, also leere Klassen die das Minimum an Daten bereitstellen.

Das Vorgehen schrittweise neue Kompoentenen hinzuzufügen und zu testen wird **Schrittweise Teilintegration** genannt.

Q: Welche Strategien für die Integration gibt es?
A: - Big-Bang
- Bottom-Up
- Top-Down
<!--ID: 1644666513988-->




## 4. Identifikation der Fehler
Taucht beim Integrationstest ein Fehler auf, welcher kein Modulfehler ist (der hätte schon im vorherigen Schritt entdeckt werden sollen), so kann er folgende Ursachen haben:
- **Kopplungsfehler**
Ein falsches Modul wurde geladen, nicht angebunden oder inkorrekt aufgerufen
- **Schnittstellenfehler**
An eine Schnittstelle wird ein falscher Datentyp übergeben (int statt double) oder die falsche Einheit verwendet (Meilen statt Kilometer)
- **Protokolllfehler**
Verstehe ich nicht ganz
- **Zeitfehler**
Nachrichten können zwar richtig gesendet und empfangen werden, jedoch zum falschen Zeitpunkt oder in falschen Zeitintervallen
- **Synchronisationsfehler**
Module verursachen einen Deadlock

## Am Ende: Abnahmetests
Abnahmetests dienen der Überprüfung eines Softwaresystems bei der Auslieferung bzw. Übergabe an den Autgraggeber und die Nutzer.
Hier wird vor allem getestet, ob alle Spezifikationen erfüllt sind.

Der Testschwerpunkte liegen auf den Aspekten:
- Test der Funktionen nach Anforderungen
- Test des Verhaltens unter Normalbenutzerbetrieb
- Test des Verhaltens in Ausnahmesituationen und im Dauerbetrieb
- Test der Leistungskenngrößen

Der Test gleicht damit einem [[Software-Test#Black-Box-Test]]

#Softwaretechnik 