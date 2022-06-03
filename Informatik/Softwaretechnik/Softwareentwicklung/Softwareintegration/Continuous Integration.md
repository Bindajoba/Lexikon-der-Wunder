TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Continuous Integration steht für die Denkschule, dass Änderungen am Code so häufig wie möglich (mehrmals am Tag) mit der Code-Basis [[Integration|integiert]] werden sollen.

*Ich habe das Gefühl, das steht im Konflikt zur Idee des [[Gitflow-Workflow]], bei dem nur bei Fertigstellung eines Relases gemergt werden soll. Die Sache hat sich geklärt. Es sollen nur erfolgreich getestete Komponenten integriert werden. Testet man die Features vor dem Merge, gibt es keinen Widerspruch.*


# Bewertung
## Vorteile
- mehr Transparenz -> Bessere Kommuniktion und Organisation
- Bugs und Errors könne früher entdeckt und behoben werden
- Bessere Einschätzung des Systemzustands -> Planung und Einhaltung eines Zeitplans
- Reduziert Wartezeiten
	- Risikominimierung?
	- Steigerung der Effizienz



# Übliche Praktiken
- Nutzung eines gemeinsamen [[Versionskontrollsystem|Repositories]]
- Build-Automatisierung
- Automatisiertes Testen der Builds
- Mindestens einmal pro Tag Code einreichen und builden lassen
- Ständige Verfügbarkeit und Sichtbarkeit von aktualisiertem Code

*Es ist nicht immer möglich alle Module zu integrieren, wenn noch nicht alle fertiggestellt sind. Hier kann es sinnvoll sein einen [[Mock]] zu verwenden.*

Q: Nenne 3 Praktiken, die für [[Continuous Integration]] genutzt werden?
A: - Gemeinsamen [[Versionskontrollsystem|Repositories]]
- Build-Automatisierung
- Automatisiertes Testen
- Mindestens einmal pro Tag Code einreichen und builden lassen
- Ständige Verfügbarkeit und Sichtbarkeit von aktualisiertem Code
<!--ID: 1645610670250-->



#Softwaretechnik 