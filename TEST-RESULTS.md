# REZULTATI TESTIRANJA

## Black Box testovi

45 + 154 = 199 `OK`
36 +786 = 822 `OK`
0 + 0 = 0 `OK`
0 + 180 = 180 `OK`
10000000+30000000 = 4.0E7 `OK`
789 - 96 = 693 `OK`
98 - 785 = -687 `OK`
0 - 7892 = -7892 `OK`
785 - 0 = 785 `OK`
78 - 96 = -18 `OK`
30 - (-5) = ERROR `Not OK`
-5 - 30 = -35 `OK`
45 - 0 = 45 `OK`
78 / 100 = 0.78 `OK`
0 / 100 = 0 `OK`
78 / 0 = Infinity `OK`
45 + 89 - 4*720 = -2746 `OK`
-56 * 32 + 18 = -1774 `OK`
78/2 - 88 /8 = 28 `OK`
"Enter bez unosa brojeva" - Aplikacija se sruši `Not OK`

## Zapažanja

- Kalkulator ne podržava zagrade. U slučaju da se unese zagrada, rezultat je ERROR. Nije moguće napraviti kalkulaciju množenja/dijeljenja sa negativnom brojem - primjer 78/(-2).
- Java aplikacija se sruši uz unhandled exception u slučaju da ne unesemo nikakvu vijednost
- Svi rezultati koji vraćaju cijele brojeve imaju jedno decimalno mjesto sa decimalnom vrijednošću "0". Npr. "12 + 5 = 17.0"
- Veliki rezultati se vraćaju u float formatu

## Jedinični test

```java
import org.junit.jupiter.api.Test;
import java.util.ArrayList;
import java.util.List;

    import static org.junit.jupiter.api.Assertions.assertEquals;

    public class CalculatorTest {

        @Test
        void testCalculateMethod() {
            List<Double> numbers = new ArrayList<>();
            List<String> operations = new ArrayList<>();

            numbers.add(12.0);
            numbers.add(36.0);
            operations.add("+");

            Calculator.Calculate(numbers, operations);
            assertEquals(48.0, Calculator.finalResult);

            // Reset for the next test
            Calculator.finalResult = 0.0;
        }

    }

```
