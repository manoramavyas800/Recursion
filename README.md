# Recursion
//PRINT N NATURAL NUMBER IN INCRESING ORDER.

public class TestClass {
    static void nNaturalNumbers(int n, int current) {
        if(current > n){
            return;
        }
       System.out.print(current+" ");
        nNaturalNumbers(n, current + 1);
    }
    public static void main(String[] args) {
        nNaturalNumbers(5, 1);

    }
}

//PRINT N NATURAL NUMBER IN DECRESING ORDER.

public class TestClass {
    static void nNaturalNumbers(int n, int current) {
        if(current < n){
            return;
        }
       System.out.print(current+" ");
        nNaturalNumbers(n, current - 1);
    }
    public static void main(String[] args) {
        nNaturalNumbers(1, 10);

    }
}
//PRINT FECTORAIL
import java.util.Scanner;

public class TestClass {
    static int fectotial (int n){
        if(n==0){
            return 1;
        }
       return n*fectotial(n-1);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
       System.out.println(fectotial(n));

    }
}
//PRINT FIBONACCI NUMBER.

import java.util.Scanner;

public class TestClass {
    static int fibonacci (int n){
        if(n==0||n==1){
            return n;
        }
            return fibonacci(n - 1) + fibonacci(n - 2);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
            System.out.println(fibonacci(n));
    }
}
//PRINT FIBONACCI SERICE.

import java.util.Scanner;

public class TestClass {
    static int fibonacci (int n){
        if(n==0||n==1){
            return n;
        }
            return fibonacci(n - 1) + fibonacci(n - 2);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        for(int i=1;i<=n;i++){
            System.out.print(fibonacci(i)+" ");
        }

    }
}
//SUM OF N NATURA NUMBER.
import java.util.Scanner;

public class TestClass {
    static int fibonacci (int n){
        if(n==0||n==1){
            return n;
        }
            return n + fibonacci(n - 1);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.println(fibonacci(n));

    }
}
