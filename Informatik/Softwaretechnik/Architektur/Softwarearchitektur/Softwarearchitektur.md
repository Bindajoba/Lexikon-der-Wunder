TARGET DECK: Universität::Informatik::SWT

# Beschreibung

# Definition
## Systemarchitektur
Die Systemarchitektur gliedert ein [[Softwaresystem]] in Teilsysteme ([[Softwaresystem#Komponente]]), die nicht notwendigerweise nur aus Software bestehen, sondern auch Hardware oder mechanische Teile umfassen kann. 

Q: Was ist eine Systemarchitektur?
A: Eine Unterteilung ein Kompoenten (niecht zwingend Software)
<!--ID: 1645543049603-->


## Softwarearchitektur
Die Gliederung eines Softwaresystems in Softwarekomponenten und deren Zerlegung in [[Modul|Module]]

Q: Was ist Softwarearchitektur?
A: Unterteilung in Softwarekomponenten
<!--ID: 1645543049725-->


# Prinzipien
Einer Architektur sind einige wichtige Prinzipien unterlegt, auf die man beim Entwurf achten sollte, diese sind:
- KISS
- Kopplung und Kohäsion
- Kapselung und Information Hiding
- Seperation of Concerns
- Divide and Conquer
- Design by Contract

Q: Was sind die 3 von 6 Prinzipien einer guten Softwarearchitektur?
A: - KISS
- Kopplung und Kohäsion
- Kapselung/Information Hiding
- Seperation of Concerns
- Divide and Conquer
- Design by Contract
<!--ID: 1645543049833-->


## KISS
KISS steht für, "keep it simple and stupid". Es soll auf ein Problem eine möglichst einfach verständliche aber tragfähige Lösung gefunden werden. (Das heißt nicht zu einfach!)

## Kopplung und Kohäsion
Siehe [[Kohäsion und Kopplung]]
*Das ist wie bei einem Zug, da muss die Kopplung zwischen Wagons niedrig ist aber die Stärke/Kohäsion der Wagons selbst hoch.*


### Kopplung
Ein [[Softwaresystem]] ist in mehrere [[Softwarekomponente]] zerlegbar. Diese Komponenten kommunizieren über Schittstellen miteinander. Je häufiger auf eine Schnittstelle zugegriffen wird, desto größer ist die Abhängigkeit/**Kopplung** zwischen den Komponenten.
Je niedriger die Kopplung, desto eigenständiger ist die Komponente und desto höher ist die Wartbarkeit des Systems.

Es wird zwischen unterschiedlichen Arten der Kopllung unterschieden:
- Inhaltskopplung (content coupling)
- Bereichkopplung (common-environment coupling)
- Hybridkopplung (hybrid coupling)
- Kontrollkopplung (control coupling)
- Datenkopplung (data coupling)
- Pathologische Kopplung (pathological coupling)

Q: Was ist Kopplung? ([[Softwarearchitektur]])
A: Ein Maß dafür, wie stark Module vernetzt sind.
<!--ID: 1645260973933-->


### Kohäsion
Die Köhäsion beschreibt den Grad des inneren Zusammenhangs der Komponenten, Klassen eines Systems. In einem System mit starker Kohäsion erfüllt jede Programmeinheit genau eine wohldefinierte Aufgabe.

Q: Was ist Kohäsion? ([[Softwarearchitektur]])
A: Ein Maß dafür, wie stark die Bestandteile eines Moduls vernetzt sind.
<!--ID: 1645260974065-->


## Kapselung und Information Hiding
Eine gute Architektur versteckt das Innenleben einer Komponente, indem nur über eine klar definierte Schittstelle darauf zugegriffen werden kann. Das Vorgehen, den Inhalt einer Komponente auf diese Weise von äußeren EInflüssen zu trennen, nennt man Kapselung.

## Seperation of Concerns
[[Seperation of Concerns]] ist ein Grundprinzip des Software Engineering, welches besagt, dass unterschiedliche Aspekte möglichst nicht vermischt werden sollen, um die Komplexität von Aufgaben zu reduzieren.
Jede Komponente soll sich auf eine Sache konzentrieren und diese so gut wie möglich machen.
Dsa Prinzip wird von Robert C. Martin durch das [[Single-Responsibility-Prinzip]] umschrieben.

## Teile und Herrsche (Divide and Conquer)
[[DIvide-and-Conquer]] ist ein Prinzip, dass besagt, dass sich eine komplexe Aufgabe am besten lösen lässt, indem man es in viele kleine Probleme zerteilt. Eine Architektur soll genau das unterstützen. Das Resultat ist gewöhnlich ein [[Modularisierung|Modularisiertes]] System
Typische Modularisierungskonzepte sind:
- Funktionale Dekomposition
Eine Aufgabe wird in Unteraufgaben zerlegt
- Strukturelle Dekomposition
Eine Struktur wird in Teilstrukturen zerlegt
- Parametrisierung
Eine modulare Struktur wird so gebildet, dass sie durch eine passende Konfiguration über Parameter an bestimmte Bedürfnisse angepasst werden kann

Es gibt verschiedene Strategien für die Modularisierung:
- **Hierarchische Dekomposition**
Das System wird in grobe Module zerlegt, die werden in feinere Module zuerlegt und die wieder, bis man Module erhält, die nicht mehr zerlegbar sind.
- **Schichtenbildung**
Bestimmte Funktionen werden in Schichten zusammengefasst und es wird eine Schnittstelle spezifiziert, die beschreibt, welche Funktionalität anderen, darüber liegenden Schichten angeboten wird. 
![[Softwarearhcitektur Schichtenbildung.png]]

## Design by Contract
Schnittstellen werden zu Beginn vertragsartig festgelegt und über den Systemlebenszyklus weitgehend stabil gehalten.
So können Softwareentwickler, die ein bestimmtes Modul benötigen arbeiten, ohne das das Modul schon vollständig implmentiert ist und die Entwickler des Moduls können darauf vertrauen, dass ihr Modul wie spezifiziert verwendet wird.

Generell verallgemeinert man eine Aufgabe eines Moduls, damit die Schnittstellen simpler werden.

Q: Was ist Design by Contract? ([[Softwarearchitektur]])
A: Schnittstellen werden zu Beginn vertraglich festgelegt und über den Systemlebenszyklus verfeinert.
<!--ID: 1645543049955-->


# Architekturmustern
Siehe [[Architekturmuster]]


#Softwaretechnik 