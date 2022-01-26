# Beschreibung
Manche Tests müssen erst eine Umgebung aufbauen, damit diese überhaupt getestet werden kann.

Dabei ist es möglich, dass die gleiche Umgebung durch mehrere Tests erstellt werden müssen, was unnötige Redundanz im Code erzeugt.

Um das Problem zu umgehen, entwickeln wir Test-Fixtures, also eine gemeinsame Grundlage für die Tests einer Testklasse.
Der Text-Fixture ist eine Methode, der erst die Umgbung der Tests erstellt.

# Variationen
## Umgebung vor Test
*Das ist ein Beispiel einer Test-Fixture mit JUnit. Das @Before zeigt anscheinend an, dass diese Methode vor jeder @Test Methode ausgeführt werden soll.*
```
package verwaltung.mitarbeiter;
import org.junit.Assert;
import org.junit.Before;
import org.junit.Test;
public class Mitarbeiter2Test {
	Mitarbeiter m1;
	
	@Before
	public void setUp() throws Exception {
		m1 = new Mitarbeiter("Uwe","Mey");
		m1.addFachgebiet(Fachgebiet.ANALYSE);
		m1.addFachgebiet(Fachgebiet.C);
		m1.addFachgebiet(Fachgebiet.JAVA);
	}
	
	@Test
	public void testHatFaehigkeit1(){
		Assert.assertTrue("vorhandene Faehigkeit", m1.hatFachgebiet(Fachgebiet.C));
	}
	
	@Test
	public void testHatFaehigkeit2(){
		Assert.assertTrue("nicht vorhandene Faehigkeit", !m1.hatFachgebiet(Fachgebiet.TEST));
	}
}
```

## Umgebung vor Testklasse
Braucht das Aufbauen der Testumgebung lange, kann es vorteilhaft sein, die Umgebung nur ein einziges Mal vor ALLEN Tests zu erstellen.
Dies wird in [[JUnit]] mit einem @BeforeClass bezeichnet.
Symmetrisch dazu gibt es noch ein @AfterClass:

```
package spielerei;
import org.junit.After;
import org.junit.AfterClass;
import org.junit.Before;
import org.junit.BeforeClass;
import org.junit.Test;

public class Ablaufanalyse {
	@BeforeClass
	public static void setUpBeforeClass() throws Exception {
		System.out.println("setUpBeforeClass");
	}
	
	@AfterClass
	public static void tearDownAfterClass() throws Exception {
		System.out.println("tearDownAfterClass");
	}
	
	@Before
	public void setUp() throws Exception {
		System.out.println("setUp");
	}
	
	@After
	public void tearDown() throws Exception {
		System.out.println("tearDown");
	}
	
	@Test
	public void test1() {
		System.out.println("test1");
	}
	
	@Test
	public void test2() {
		System.out.println("test2");
	}
}
```

Das Auführen obigen Codes würde zu folgender System.out.print-Ausgabe/Ausführungsreihenfolge führen:
1. setUpBeforeClass
2. setUp
3. test1
4. tearDown
5. setUp
6. test2
7. tearDown
8. tearDownAfterClass