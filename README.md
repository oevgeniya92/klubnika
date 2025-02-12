# klubnika

import java.util.ArrayList;
import java.util.Collections;
import java.util.List;

public class SortExample {
    public static void main(String[] args) {
        // Создаем список строк
        List<String> names = new ArrayList<>();
        names.add("Иван");
        names.add("Анна");
        names.add("Сергей");
        names.add("Елена");
        names.add("Максим");
        
        System.out.println("Исходный список:");
        printNames(names);
        
        // Сортируем список по алфавиту
        Collections.sort(names);
        
        System.out.println("\nОтсортированный список:");
        printNames(names);
        
        // Сортируем список в обратном порядке
        Collections.reverse(names);
        
        System.out.println("\nСписок в обратном порядке:");
        printNames(names);
    }
    
    private static void printNames(List<String> names) {
        for (String name : names) {
            System.out.println(name);
        }
    }
}
