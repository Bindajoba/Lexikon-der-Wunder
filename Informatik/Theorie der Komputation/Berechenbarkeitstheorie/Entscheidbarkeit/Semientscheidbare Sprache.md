## Beschreibung
Eine [[Formale Sprache]] heißt **semi-entscheidbar**, wenn für ein beliebiges Wort, das berits in der Sprache liegt in endlicher Zeit festgestellt werden kann, ob es wirklich in der Sprache ist. (vgl. [[Berechenbarkeit]])
D.h.: Wenn das [[Wortproblem]] für alle Wörter $\Sigma^*$ [[Entscheidbarkeit|entscheidbar]] ist.


## Definition
Eine Sprache heißt **semi-entscheidbar**, falls $\chi_L': \Sigma^* \to \{0,1\}$ mit 
$$\chi_l'(w) = \begin{cases} 1, & \text{falls } w\in L \\ \text{undefiniert, } & \text{falls } w \notin L \end{cases}$$ [[Berechenbarkeit|berechenbar]] ist.

## Eigenschaften
- Die **semi-entscheidbaren Sprachen** sind genau die [[Rekursiv Aufzählbare Sprache|rekursiv aufzählbaren Sprachen]]


#FSK 