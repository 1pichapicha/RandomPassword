import java.util.Random;

public class RandomPasswordGenerator {
    public static void main(String[] args) {
        int length = 10;
        String password = generateRandomPassword(length);
        System.out.println("Сгенерированный пароль: " + password);
    }
