Array Quiz Style

(Source Code):-

import java.util.Random;
import java.util.Scanner;
import java.util.Arrays;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("*****WELCOME TO QUIZ GAME*****");
        String qst[] = {"1) Who Did the Beer Hall pusch ?", "2) In which year the French Revolution happened ?", "3) Who invented Java?"};
        String opts[][] = {{"a) Hitler b) Waffen SS c) Khalid"}, {"a) 1234 b) 1771 c) 1781 d) 1787"}, {"a) James Gosling b) Eminem c) Marshaal d) Mozart"}};
        int ans[] = {1, 4, 1};
        int point = 0;
        for (int i = 0; i < qst.length; i++) {
            System.out.println(qst[i]);
            for (int j = 0; j < opts[i].length; j++) {
                System.out.println(opts[i][j]);
            }
            System.out.println("Enter your choice");
            int choice = sc.nextInt();
            if (choice == ans[i]) {
                point++;
            }
        }
        System.out.println("Total Score :- "+" "+point);
    }
}
