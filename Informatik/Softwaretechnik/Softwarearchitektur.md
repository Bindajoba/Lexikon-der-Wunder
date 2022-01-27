TARGET DECK: Universität::Informatik::SWT

# Beschreibung

# Definition
## Allgemeine Architektur
Die Systemarchitektur gleidert ein [[Softwaresystem]] in Teilsysteme ([[Softwaresystem#Komponente]]), die nicht notwendigerweise nur aus Software bestehen, sondern auch Hardware oder mechanische Teile umfassen kann. 

## Softwarearchitektur
Die Gliederung eines Softwaresystems in Softwarekomponenten und deren Zerlegung in [[Modul|Module]]

# Prinzipien
Einer Architektur sind einige wichtige Prinzipien unterlegt, auf die man beim Entwurf achten sollte, diese sind:
- KISS
- Kopplung und Kohäsion



## KISS
KISS steht für, "keep it simple and stupid". Es soll auf ein Problem eine möglichst einfach verständliche aber tragfähige Lösung gefunden werden. (Das heißt nicht zu einfach!)
## Kopplung und Kohäsion
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

### Kohäsion
Die Köhäsion beschreibt den Grad des inneren Zusammenhangs der Komponenten, Klassen eines Systems. In einem System mit starker Ko




#Softwaretechnik 