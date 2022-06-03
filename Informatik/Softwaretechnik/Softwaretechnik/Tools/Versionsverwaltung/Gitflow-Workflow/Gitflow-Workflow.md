TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Git-Flow ist eine nun veraltete Strategie Branches zu nutzen, um sein Projekt zu strukturieren.
Sie baut auf dem [[Gitlab-Workflow]] auf und ist nicht damit zu verwechseln.


# Branchunterteilung
Bei Git Flow werden viele Branches erstellt. Diese Branches lassen sich in vier Typen unterteilen.

![Git-flow-Workflow – Hotfix Branches](https://wac-cdn.atlassian.com/dam/jcr:cc0b526e-adb7-4d45-874e-9bcea9898b4a/04%20Hotfix%20branches.svg?cdnVersion=140)


Q: Welche Brancharten gibt es beim Gitflow-Workflow
A: - Main
- Release
- Develop
- Feature
- Hotfix
<!--ID: 1642952243062-->


## Main-Branch
Im Main-Branch befinden sich die offiziellen Releases des Projekts. Die Versionen im Main-Branch werden üblicherweise mit Versionsnummern betitelt.

Jede Version sollte vollkommen funktionsfähig sein und keine Bugs besitzen.

## Develop-Branch
Der Develop-Branch wird für alles Entwicklungbezogene verwendet.

## Feature-Branch
Will man ein neues Feature hinzufügen, dann erstellt man einen Feature-Branch. Ist das Feature implementiert, dann wird der Branch wieder mit den develop-Branch gemergt.

## Release-Branch
Hat ein der Develop-Branch genug Features, dann wird ein Release-Branch abgespalten. Dieser wird weitestgehend wie der development-ranc behandelt, es werden aber keine neuen Features mehr hinzugefügt, sondern nur noch Bugs behoben.

Sind alle Bugs behoben oder das release-date erreicht, dann wird der Release-Branch mit dem Main-Branch gemergt.

## Hotfix-Branch
Gibt es einen großen Bug, der so schnell wie möglich nachträglich behoben werden muss, dann wird aus der zuletzt ausgelieferten Version ein Hotfix in einen eigenständigen Hotfix-Branch abgespalten.

Ist der Hotfix behoben, werden die Änderungen sowohl in den Main und Development-Branch gespeichert.

#Softwaretechnik 