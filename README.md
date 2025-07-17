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
//SUM 0F  DIGITHS.

import java.util.Scanner;

public class Main {
    static int SOD(int n) {
        if (n >0&&n<=9) {
            return n;
        }
        return SOD(n/10)+(n%10);
    }

    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
    int n = sc.nextInt();
        System.out.println(SOD(n));
    }
}

//PRINT POWER.

import java.util.Scanner;

public class Recorsion {
 static int power(int p,int q){
     if(q==0){
         return 1;
     }
     int power=power(p,q-1);
     return p*power;
 }
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int p= sc.nextInt();
       int q= sc.nextInt();
       System.out.println(power(p,q));
       }
    }
    //SECOND METHODE.

    import java.util.Scanner;

public class Recorsion {
 static int power(int p,int q){
     if(q==0){
         return 1;
     }
     //if q is even
     if(q%2==0){
         return power(p,q/2)*power(p,q/2);
     }
     //if q is odd.
     return  power(p,q/2)*power(p,q/2)*p;
 }
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int p= sc.nextInt();
       int q= sc.nextInt();
       System.out.println(power(p,q));
       }
    }
//print k multiple of nth number.

import java.util.Scanner;

public class Recorsion {
 static void multiple(int p,int q){
     //base case
     if(q==1){
         System.out.println(p);
         return ;
     }
     //recursive work
     multiple(p,q-1);
     //self work
     System.out.println(p*q);

 }
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int p= sc.nextInt();
       int q= sc.nextInt();
       multiple(p,q);
       }
    }
    //print decreasing order.
import java.util.Scanner;

public class Recorsion {
 static void multiple(int p,int q){
     //base case
     if(q==1){
         System.out.println(p);
         return ;
     }
     //self work
     System.out.println(p*q);
     //recursive work
     multiple(p,q-1);
    

 }
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int p= sc.nextInt();
       int q= sc.nextInt();
       multiple(p,q);
       }
    }

  //PRINT SUM OF N NATURAL NUMBER BUT ALTERNATE SINGH.
  import java.util.Scanner;

public class Recorsion {
 static int SUM(int q){
     //base case
     if(q==0){
         return 0;
     }
     //recursive work
     //IF Q IS EVEN
     if(q%2==0){
         return SUM(q-1)-q;
     }
     //IF Q IS ODD
     return SUM(q-1)+q;
        }
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int p= sc.nextInt();
       System.out.println(SUM(p));
       }
    }
    //SUM OF TWO DIGIT.

    import java.util.Scanner;

public class Main {
    static int dif(int n,int m) {
        if(m==0){
            return n;
        }
        return dif(n+1,m-1);
    }
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int n = sc.nextInt();
       int k = sc.nextInt();
       System.out.println(dif(n,k));
    }
}
//DIFFRENTS OF TWO NUMBER.

import java.util.Scanner;

public class Main {
    static int dif(int n,int m) {
        if(m==0){
            return n;
        }
        return dif(n-1,m-1);
    }
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int n = sc.nextInt();
       int k = sc.nextInt();
       System.out.println(dif(n,k));
    }
}
// PRINT LCM.

import java.util.Scanner;

public class Recursion {
    static int GCD(int n, int m) {
       if(m==0){
           return n;
       }
        return GCD(m,n%m);
    }
    static int LCM(int n, int m) {
        return (n*m)/GCD(n,m);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int m = sc.nextInt();
        int result = LCM(n, m);
        System.out.println(result);

    }
}
//PRINT ARRAY USING RECURSION.

import java.util.Scanner;

public class Recursion {
   static void printArray(int[] arr, int idx) {
       if (idx == arr.length) {
           return;
       }
       System.out.print(arr[idx] + " ");
       printArray(arr, idx + 1);

   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
       printArray(arr, 0);

    }
}
//PRINT REVERSE ORDER IN ARRAY.
import java.util.Scanner;

public class Recursion {
   static void printArray(int[] arr, int idx) {
       if (idx == arr.length) {
           return;
       }
    
       printArray(arr, idx + 1);
       System.out.print(arr[idx] + " ");

   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
       printArray(arr, 0);

    }
}
//PRINT MAX NUM IN ARR.

import java.util.Scanner;

public class Recursion {
   static int printArray(int[] arr, int idx) {
       if (idx == arr.length-1) {
           return arr[idx];
       }
      int smalAns=printArray(arr, idx+1);
       return Math.max(smalAns, arr[idx]);

   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
           int max= printArray(arr, 0);
        System.out.println(max);

    }
}
//SUM OF  ALL ELEMENT.

import java.util.Scanner;

public class Recursion {
   static int printArray(int[] arr, int idx) {
       if (idx == arr.length) {
           return 0;
       }
      int sum=printArray(arr, idx+1);
       return sum+arr[idx];

   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
           int sum= printArray(arr, 0);
        System.out.println(sum);

    }
}
//fiind target is present or not.

import java.util.Scanner;

public class Recursion {
   static boolean printArray(int[] arr,int n,int target, int idx) {
       if (idx >= n) {
           return false;
       }
       if (arr[idx] == target)return true;
       return printArray(arr,n,target, idx+1);

   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int target=sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        if(printArray(arr,target,arr.length,0)){
            System.out.println("YES");
        }else{
            System.out.println("NO");
        }
    }
}
//FING TARGET INDEX IN ARR.

import java.util.Scanner;

public class Recursion {
   static int printArray(int[] arr,int n,int target, int idx) {
       if (idx >= n) {
           return -1;
       }
       if (arr[idx] == target)return idx ;
       return printArray(arr,n,target, idx+1);

   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int target=sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        int res = printArray(arr,n,target,0);
       System.out.println(res);
    }
}
//find target in arrayList.

import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

public class Recursion {
   static List<Integer> printArray(int[] arr, int n, int target, int idx) {
       if (idx >= n) {
           return new ArrayList<>();
       }
       List<Integer> list = printArray(arr, n, target, idx + 1);
       if (arr[idx] == target)list.add(arr[idx]) ;
       return list;

   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int target=sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        List<Integer> list = printArray(arr,n,target,0);
      if(list.isEmpty()){
          System.out.println("target not found");
      }else{
          for (Integer integer : list) {
              System.out.print(integer + " ");
          }
      }
    }
}
//FIND ALL INDISES.

import java.util.Scanner;

public class Recursion {
  static void findAllIndises(int[]arr,int n,int target,int idx){
      if(idx>=n){
          return;
      }
      if(arr[idx]==target) {
          System.out.print(idx+" ");
      }
          findAllIndises(arr,n,target,idx+1);

  }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int target = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0;i<n;i++){
            arr[i] = sc.nextInt();
        }
       findAllIndises(arr,n,target,0);
    }
}
//RETURN  ALL INDISES IN ARRAYLIST.

import java.util.ArrayList;
import java.util.Scanner;

public class Recursion {
  static ArrayList<Integer> findAllIndises(int[]arr,int n,int target,int idx){
      if(idx>=n){
          return  new ArrayList<>();
      }
      ArrayList<Integer> res = new ArrayList<>();
      if(arr[idx]==target) {
          res.add(idx);
      }
      ArrayList<Integer> tmp = findAllIndises(arr,n,target,idx+1);
      res.addAll(tmp);
      return res;

  }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int target = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0;i<n;i++){
            arr[i] = sc.nextInt();
        }
       ArrayList<Integer> res = findAllIndises(arr,n,target,0);
        System.out.println(res);
    }
}
