package com.company;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("Введите велиичины полуосей a и b");
        System.out.println("a =");
        double a = scan.nextDouble();
        System.out.println("b =");
        double b = scan.nextDouble();

        double array[] = new double[]{0.1, 0.1, 0.2, 0.3, 0.2, 0.1, 0.3, 0.4, 5, 6};
        for (int k = 0; k < 5; k++) {
            int i = k * 2;
            int j = i + 1;
            if ((array[i]*array[i])/(a*a)+(array[j]*array[j]/(b*b)) < 1) {
                System.out.println(k+1);
            }
        }
    }

}
