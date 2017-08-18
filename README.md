# JUnitExample
Пример работы с JUnit
Наверняка многим интересно написать свой первый юнит тест.
В мире Java можно воспользоваться JUnit. Тестировать будем результат от сложения 2 + 2. Исходник:
public class LearnUnitTest {
    public static void main(String[] args) {
        int x = 2;
        int y = 2;
        int sum;
        sum = x + y;
        System.out.println(sum);
    }
}
И его тест:



import org.junit.Test;
import static org.junit.Assert.assertEquals;

public class LearnUnitTestTest extends LearnUnitTest {
    @Test
    public void main() throws Exception {
        assertEquals(4, 2 + 2);
    }
}

Если выставить поменять ожидаемый результат на 5 то тест упадёт. 
