public class Main {
    public static int generateRandomAge() {
        return (int)(Math.random() * 70); // age 0–69
    }

    public static String permission(int age, int temperature) {
        if (age >= 20 && age <= 45 && temperature >= -20 && temperature <= 30) {
            return "You can go for a walk";
        } else if (age < 20 && temperature >= 0 && temperature <= 28) {
            return "You can go for a walk";
        } else if (age > 45 && temperature >= -10 && temperature <= 25) {
            return "You can go for a walk";
        } else {
            return "Stay home";
        }
    }

    public static void main(String[] args) {
        int age1 = generateRandomAge();
        System.out.println("Age: " + age1 + ", Temperature: 10 " + permission(age1, 10));

        int age2 = generateRandomAge();
        System.out.println("Age: " + age2 + ", Temperature: -15  " + permission(age2, -15));

        int age3 = generateRandomAge();
        System.out.println("Age: " + age3 + ", Temperature: 25  " + permission(age3, 25));

        int age4 = generateRandomAge();
        System.out.println("Age: " + age4 + ", Temperature: 5  " + permission(age4, 5));

        int age5 = generateRandomAge();
        System.out.println("Age: " + age5 + ", Temperature: 30  " + permission(age5, 30));
    }
}
