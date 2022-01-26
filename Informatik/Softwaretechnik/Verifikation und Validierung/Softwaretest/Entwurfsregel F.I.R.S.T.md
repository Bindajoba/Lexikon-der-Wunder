# Beschreibung
Im Kontext des [[Sauberer Code|Clean-Code-Prinzips]] führt Martin (Der Autor des ersten Lesetexts) die F.I.R.S.T. Entwurfsregel für Tests – primär für automatisierte Tests – auf. Er weist auch besonders darauf hin, dass:
„If you let your test rot, then your code will rot too.“ Das Akronym F.I.R.S.T. steht hierbei
für:

Das Akonym steht für:
- **Fast**
Test sollen schnell sein. Großen Tests werden weniger oft durchgeführt, wodurch in der Zwischenzeit mehr Fehler entstehen können
- **Indepentent**
Test sollen voneinander unabhängig sein. Die Reihenfolge der Tests darf keine Rolle spielen. 
- **Repeatable**
Test sollen wiederholbar sein
- **Self-Validating**
Test sollen sofort ein boolean ausgeben, das feststellt, ob der Test erfolgreich war. Details werdem im log ausgegeben
- **Timely**
Tests sollen immer zeitnah zum Programmcode erstellt werden auf den sie sich beziehen.	


#Softwaretechnik 