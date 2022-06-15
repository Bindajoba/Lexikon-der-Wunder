TARGET DECK: Universität::Informatik::NaCo

# Beschreibung
Eine Lambda-Evaluation ist das [[Ableitung (Informatik)|Ableiten]] für funktionale Programmiersprachen. Es ist vergleichbar mit der [[Ableitung eines Wortes]].

# Definition
Eine Evaluation eines [[Lambda-Term]] $L$ ist eine Sequenz von $\lambda$-Termen $L_0 \mapsto ... \mapsto L_n$ wobei $L_0 = L$ und $L_{i+1}$ wird generiert von $L_i$ durch die Anwendung einer Operation $\mapsto: \Lambda \to \Lambda$zu einem beliebigen Unterterm von $L_i$. Wir definieren die folgenden Operationen:
- ($\alpha$-conversion) $(\lambda x.M ) \mapsto_\alpha (\lambda y . M [x := y])$ für $y \notin \mathfrak{F}(M)$
- ($\beta$-reduction) $(( \lambda x . M) N ) \mapsto_{\alpha} M [x:= N]$,
- ($\eta$-reduction) $(\lambda x . (N \, x)) \mapsto_{\eta} M$ für $x \notin \mathfrak{F}(M)$

*Eventuell ist das $\mapsto$-Symbol falsch. In den Folien ist der Strich rechts gekrümmt.*

**Normal-order Evaluation** wendet die Operation immer auf den Äußersten linkensten Unterterm an. (Dazu kann man sich den Term als Baum zeichnen und dann fängt man mit dem obersten Element an und geht dann nach links). Diese Excecution unterscheidet sich stark von der Berechnung bei gängigen Programmiersprachen, wo zuerst dass innerste berechnet wird.
Normal-order Evaluation ermöglicht bei Haskell [[Lazy-Evaluation]]

Q: Welche drei Arten der Lambda-Evaluation gibt es?
- ($\alpha$-conversion) 
- ($\beta$-reduction) 
- ($\eta$-reduction) 


#Natural-Computing 
