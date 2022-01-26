## Beschreibung
Software-Verifikation stellt Techniken zur Verfügung, mit der die [[Korrektheit]] eines Programms mathematisch nachgewiesen werden kann.

Es stellt grundsätzlich die Frage: "Entsprcht das Progamm den konkreten (funktionalen und nichtfunktionalen (?)) Spezifikationen?"

Damit ist die Verifikation ein Teil der [[Software-Validierung]]

## Ziel
Sei $I$ die Impementierung eines Programms und $S$ die Spezifikation.
Wir wollen zeigen, dass die Implementierung die Spezifikation erfüllt, d.h. $I \models S$

Dazu müssen aber sowohl der Programmcode als auch die Anforderungen mathematisch modelliert werden. 
![[Software-Verifikation.png]]

## Techniken
### Deduktion
Durch [[Logikkalkül]] werden die Anforderungen aus dem Code [[Deduktion|deduktiert]]. Diese Methode kann aber bei komplexen Programmen schnell unübersichtlich werden, daher wird sie heute ungerne verwendet.

### Modellprüfung
Ein Programm wird zuerst in eine [[Kripke-Struktur]] umgewandelt, eine Struktur, die einem [[Automat]] gleicht.
Mit speziellen [[Traversierungsalgorithmus|Traviersierungsalgorithmen]] wird die Spezifikation irgendwie bewiesen oder widerlegt.

### Abstrakte Interpretation
???

## Dimensionen der Techniken
- **Ausdrucksstärke**
Eine Technik ist Ausdrucksstark, wenn viele Spezifikationen formal beschrieben werden können. Damit ist die Dedutkion die Ausdrucksstärkste Technik zur Verifikation. Generell sinkt mit steigender Ausdruckskraft die Skalierung.
- **Skalierung**
Die Skalierung beschreibt, wie gut ein Verfahren, dass für kleine Programme funktioniert auch für die Verifikation größerer Programme funktioniert.
- **Automatisierung**
Lässt sich die Technik durch ein Programm automatisieren?
- **Präzision**
Ist der Schluss, der aus der Technik gezogen wird immer richtig? Tauchen [[Alphafehler]] oder [[Betafehler]] auf?

#Softwaretechnik 