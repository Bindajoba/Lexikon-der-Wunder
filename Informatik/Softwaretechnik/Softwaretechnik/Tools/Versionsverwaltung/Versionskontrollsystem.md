TARGET DECK: Universität::Informatik::SWT

# Beschreibung


# Beschreibung
Ein Versionskontrollsystem(engl. **Version Control System**, **VCS**) zeichnet Informationen über die Vorgeschichte von Dokumenten auf.
Es ermöglicht
- Aus alte Versionen zuzugreifen
- An verschiedenen Versionen gleichzeitig zu entwickeln und diese zu warten

Q: Wie entstehen Merge-Konlikte?
A: Wenn zwei Programmierer sich widersprechende Änderungen am gleichen Programmteil vornehmen. 
<!--ID: 1642952243312-->


# Aufgaben
- Stellt **gemeinsamen Datenspeicher** für das Team bereit
- Stellt Möglichkeiten zur **arbeitsteiligen Entwicklung** einer Software bereit
- **Entwicklungshistorien** können nachverfolgt werden
- Es können in sich konsistente, **arbeitsfähige Softwarestände** erstellt (und wiederhergestellt) werden 
- Es kann das Release-Management eines Softwareprodukts realisiert werden. (?)

Q: Was sind zwei Vorteile von Versionskontrollsystemen?
A: - Gleichzeitiger Zugriff auf den Code
- Einfacher Zugriff auf alte Versionen
- Vergleich mit alten Versionen
- Ermöglicht kleine häufige Commits
- Ermöglicht [[Continuous Integration|Continous-Integration]]
<!--ID: 1642952243428-->


# Zentrale Konzepte
- **Mainbranch**
Der Hauptentwicklungszwei, der allen Entwicklern zur Verfügung steht
- **Branch**
Ei nicht-öffentlicher Entwicklungsast, welcher etwa durch einen Entwickler ausgekoppelt wird, um Weiterentwicklugen vorzunehmen.
- **Commit**
Das Quellcodefragment wird dem Versionskontrollsystem hinzugefügt.
- **Checkout**
Eine bestimmte  (normalerweise die aktoellste) Version des Projekts wird vom Versionskontrollsystem auf dem Computer angelegt.
- **Merge**
Zusammenführen von verschiedenen Versionen, etwas zwei Branches

# Variationen
- **Zentrales VKS** 
Versionierten Dateien werden auf einem zentralen Server aufbewahrt. Dadurch erhält man ein Single-Point-of-Failure. Wird der Server beschädigt, sind die Dateien verschwunden.
- **Dezentrales VKS** (z.B. Git)
Alle Benutzer erhalten eine vollständige Kopie der Versionskontrolle auf ihrem Computer. Dadurch kann man den Server wiederherstellen und sogar offline arbeiten.

Q: Welche zwei Arten von Versionsverwaltungssystemen gibt es?
A: - Zentrales VKS
- Dezentrales VKS
<!--ID: 1642952243553-->



# Workflow
## GitLab-Workflow
Siehe [[Gitlab-Workflow]]

## GitFlow-Workflow
Siehe [[Gitflow-Workflow]]
