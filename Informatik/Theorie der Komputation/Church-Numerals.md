TARGET DECK: Universität::Informatik::NaCo

# Beschreibung


# Definition
EineNatürrliche Zahl $n \in \N$ kann als [[Lambda-Term]] verwendet werden:
$$n = (\lambda f . (\lambda x .(f^n x)))$$
wobei $(f^0 x) = x$ und $(f^nx) = (f(f^{n-1} x))$. Daraus folgt, dass die [[Nachfolgerfunktion]] geschrieben werden kann als 
$$succ = \lambda n. \lambda f \lambda x.(f ((n \, f)x))$$
Wir definieren weiter
$$plus = \lambda m. \lambda n.\lambda f. \lambda x.((m \, f)((n \,f)x))$$
*Multiplikation und Exponentiation kann genauso erzeugt werden.*


# Siehe auch
Die Nachfolgerfunktion baut auf den [[Peano-Axiomen]] auf.


#Natural-Computing 
