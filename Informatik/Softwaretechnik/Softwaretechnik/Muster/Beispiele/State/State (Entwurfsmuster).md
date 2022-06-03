TARGET DECK: Universität::Informatik::SWT

# Beschreibung
State ist ein [[Entwurfsmuster (Softwaretechnik)]].
Es dient dazu Methoden eines Objekts in unterschiedlichen Zuständen zu modellieren.



# Struktur
Folgendes Beispiel illustriert den Verwendungszweck
Eine TCP-Verbindung soll unterschiedlich reagieren, abhängig davon, ob die Verbindung offen, listening oder closed ist.

TCP hat ein Objekt TCPState gespeichert, welcher den aktuellen Zustand der Verbindung repräsentiert. Das Ausführen der Open(), Close() Methode in der TCPState ist nun an den aktuellen Zustand angepasst.

![[State Beispiel.png]]

![[State Struktur.png]]

# Beispiel
![[State Beispiel ATM.png]]
*Eine ATM-Maschine soll sich unterschiedlich verhalten, je nachdem, in welchem Zustand sie sich befindet.*

```
public class ATMMachine {
	ATMState hasCard;
	ATMState noCard;
	ATMState hasCorrectPin;
	ATMState atmOutOfMoney;

	ATMState atmOutOfMoney;
	
	public ATMMachine() {
		hasCard = new HasCard(this);
		noCard = new NoCard(this);
		hasCOrrectPin = new HasPin(this);
		atmOutOfMoney = new NoCash(this);
	
		atmState = noCard;
		
		

		
		if(cashInMachine < 0) {
			atmState = atmOutOfMoney;
		}
	
		void setATMState(ATMState new ATMState) {
			atmState = newATMState;
		}
	
		public void setCashInMachine(int newChashInMachine) {
			cashInMachine = newCashInMachine;
		} 

		public insertCard() {
			ATMState.insertCard();
		}

		public expelCard() {
			ATMState.expelCard();
		}

		public enterPin(int pin) {
			ATMState.enterPin(pin);
		}

		public retractMoney(int moneyValue) {
			ATState.retractMoney();
		}


		public ATMState getATMState() {
			return ATMState;
		}
	
	}
}
```
*Die möglichen Zustände werden immer gespeichert, so können diese etwas umfangreicher gestaltet sein oder sogar Informationen merken, auf die zugegriffen werden soll, wenn das Programm wieder in diesen Zustand kommt (z.B. wie oft Geld herausgenommen wurde, während das Programm im atmOutOfMoney State).*





#Softwaretechnik 


