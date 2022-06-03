TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Git ist ein Dezentrales Versionskontrollsystem.

# Befehle
Die meisten Befehle habe ich von der Seite[^1]
## Repository erstellen
- git init: 
Erstellt ein neues Repository
- git clone path/to/repository
Kopiert ein existierende Repo

# Dateien stagen
- git add Dateiname.txt
Fügt die Datei der Stagingarea hinzu. Das muss vor jedem Commit gemacht werden, damit der Computer weiß, was commitet werden soll.

## Commiten
- git commit
Öffnet ein vim (?) Fenster bei dem man seine Commit-Nachricht eingeben kann. Das ist sehr umständlich benutze deshalb lieber:
- git commit -m "Commit-Nachricht"
Commitet mit Nachricht.

## Branches
- ```git checkout -b "Branchname"```
Wechselt zum Branch oder erstellt ihn, wenn er nicht existiert (Dabei wird aber, so denke ich, nicht der Main-Branch kopiert)
- ```git checkout -b "Neuer Branch" "Alter Branch"```
Kopiert die Inhalte aus dem alten Branch in einen neuen.
- ```git branch```
Gibt eine Liste aller Branches aus.[^2]

## Merge
- ```git merge "Branchname"```
Mergt den Ausgewählten Branch mit dem akuellen

# Übungen
## Übung SWT 4-1
### a)
Weche Rolle hat der HEAD-Verweis auf Git?


## Übung SWT 4-2
![[Übung SWT 4-2.png]]
1. git init
2. git add Navigation.java
3. git commit -m "JavaDoc hinzugefügt"
4. git checkout -b "refactoring" "master"
5. git add "Navigation.java" -> git commit "System.out.println aufgeräumt"
6. git checkout "master"
7. git add "Navigation.java"
git commit "Exceptionnachricht angepasst"
8. Mache ich wann anders...




#Softwaretechnik 

[^1]: https://www.hostinger.com/tutorials/basic-git-commands
[^2]: https://www.atlassian.com/git/tutorials/using-branches/git-merge