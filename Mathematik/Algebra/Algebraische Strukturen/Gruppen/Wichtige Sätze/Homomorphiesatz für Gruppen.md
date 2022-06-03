# Definition
Sei $\phi: G\to H$ ein Gruppenhomomorphismus. Dann induziert $\phi$ einen Isomorphismus
$$\overline \phi: G/ker(\phi) \tilde \to im(\phi)$$
Ist der Homomorphismus $\phi$ surjektiv, dann erhält man also einen [[Isomorphismus]] $G/ker(\phi) \cong H$
*$im(\phi)$* ist das Bild von $\phi$


# Übungen
## Klausuren 2016 Aufgabe 3
![[Klausur 2016 Aufgabe 3.png]]
### a) 
- Neutrales Element
$\phi(e, e) = e^{-1}e = e$
- Inverses
$\phi((z, g)^{-1}) = \phi((z^{-1}, g^{-1})) = zg^{-1} = (gz^{-1})^{-1} = (z^{-1}g)^{-1} = \phi((z, g))^{-1}$
- Erhalt der Verknüpfung
$\phi((z_1, g_1)(z_2, g_2)) = \phi(z_1z_2, g_1g_2) = z_2^{-1}z_1^{-1}g_1g_2 = z_1^{-1}g_1z_2^{-1}g_2 = \phi(z_1g_1)\phi(z_1g_2)$

### b)
- Nach a) Hom
- Surjektivität
Sei $g \in G$: dann gilt $\phi(e, g) = g$
- Kern
$\phi(z, g) = 0 \iff z^{-1}g = e \iff g = z \iff (z, g) = (z, z) \in N$

Damit gilt die obere Isomrphie.


#Algebra 