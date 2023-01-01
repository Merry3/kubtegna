# kubtegna





import java.util.Arrays;
import java.util.Random;
import java.util.Scanner;

public class luckky {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("please insert the number of members ");
        int memberSize = scanner.nextInt();
        System.out.println("how many person will be nominated?");
        int choosen = scanner.nextInt();

        String[] membersList = new String[memberSize];

        int index = 0;
        while (membersList.length > index) {
            System.out.println("please insert your name ");
            membersList[index] = scanner.next();
            index++;
        }
        System.out.println(Arrays.toString(membersList));
        for (int i = 0; i < 3; i++) {
            Random random = new Random();
            int luckyNumber = random.nextInt(0, memberSize);
            System.out.println(membersList[luckyNumber]);


            /**for(int i = 0; i < 5; i++) {
             System.out.println("*");
             for (int j = 0; j <= i; j++)
             System.out.print("*");

             }
             System.out.print(" ");*/


        }
    }
}
