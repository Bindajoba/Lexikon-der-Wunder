TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Manche Tests müssen erst eine Umgebung aufbauen, damit diese überhaupt getestet werden kann.

Dabei ist es möglich, dass die gleiche Umgebung durch mehrere Tests erstellt werden müssen, was unnötige Redundanz im Code erzeugt.

Um das Problem zu umgehen, entwickeln wir Test-Fixtures, also eine gemeinsame Grundlage für die Tests einer Testklasse.
Der Text-Fixture ist eine Methode, der erst die Umgbung der Tests erstellt.

Q: Was ist ein Test-Fixture?
A: Eine Menge von Objekten und Operationen, die eine Testumgebung bereitstellen.
<!--ID: 1645610668218-->


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

Q: Was ist die Syntax von AssertTrue()?
A: assertTrue(bedingung : boolean)
<!--ID: 1645610668347-->


Q: Was ist die Syntax von assert()
A: assert(wert1, wert2)
<!--ID: 1645610668463-->


Q: Wie erzeugt man ein Objekt mit JUnit?
A: @Before
setUp() {}
<!--ID: 1645610668558-->


Q: Wie beseitigt man ein Objekt mit JUnit?
A: @After
tearDown() {}
<!--ID: 1645610668657-->


Q: Wie schreibt man eine Testmethod mit JUnit?
A: @test
test1() {}
<!--ID: 1645610668762-->


Q: Wie stellt man einen Zustand vor allen Tests einer Testklasse her?
A: @BeforeClass
<!--ID: 1645610668858-->


Q: Wie beseitigt man einen Zustand nach einem Test?
A: @AfterClass
<!--ID: 1645610668956-->


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