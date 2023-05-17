# RandomPassword
RandomPassword
import java.util.Random;

public class RandomPasswordGenerator {
    public static void main(String[] args) {
        int length = 10;
        String password = generateRandomPassword(length);
        System.out.println("Сгенерированный пароль: " + password);
    }

    public static String generateRandomPassword(int length) {
        String characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*";
        StringBuilder password = new StringBuilder();

        Random random = new Random();
        for (int i = 0; i < length; i++) {
            int index = random.nextInt(characters.length());
            password.append(characters.charAt(index));
        }

        return password.toString();
    }
}
