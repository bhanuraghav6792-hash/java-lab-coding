
//check prime or not in java
import java.util.Scanner;
public class MyClass {
  public static void main(String args[]) {
      Scanner sc = new Scanner(System.in);
      int n = sc.nextInt();
      int flag = 0;
      for(int i=2;i<=n/2;i++){
          if(n%i==0){
              flag = 1;
              break;
          }
      }
      if(flag==1){
          System.out.println("not a prime");
      }else{
          System.out.println("prime");
      }
  }
}

// with two classes connect first is boolean and second to add this prime class to second void maindatory
import java.util.Scanner;

public class ControlFlow {
    public static boolean prime(int n){
        for(int i =2;i<=Math.sqrt(n);i++){
            if(n%i==0){
                return false;
            }
        }
        return true;
    }
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        // Call the prime method and print result
        System.out.println(prime(n) ? "prime" : "not prime");
        // Close scanner to prevent resource leak
        sc.close();
    }
}

// find factorial with two classes first is fact(n) and second is void mandotory normal to take a input and print the fact(n)
import java.util.Scanner;

public class ControlFlow {
    public static int fact(int n){
        int f = 1;
        for(int i =1;i<=n;i++){
            f*=i;
        }
        return f;
    }   
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        System.out.println(fact(n));
    }
}

// count the digits with two classes first is countdigit(n) with this change in while loop and second is void mandotory normal to take a input and print the countdigit(n)

import java.util.Scanner;

public class ControlFlow {
    public static int countdigit(int n){
        int c = 0;
        while(n!=0){
            c++;
            n = n/10;
        }
        return c;
    }    
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        System.out.println(countdigit(n));
    }
}
 
// sum of digits

import java.util.Scanner;

public class ControlFlow {
    public static int sumofdigits(int n){
        int sum = 0;
        while(n!=0){
            int d = n%10;
            sum = sum + d;
            n = n/10;
        }
        return sum;
    }    
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        System.out.println(sumofdigits(n));
    }
}

// product of digits

import java.util.Scanner;

public class ControlFlow {
    public static int productofdigits(int n){
        int prod = 1;
        while(n!=0){
            int d = n%10;
            prod = prod * d;
            n = n/10;
        }
        return prod;
    }    
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        System.out.println(productofdigits(n));
    }
}

// reverse of digits

import java.util.Scanner;

public class ControlFlow {
    public static int reverseofdigits(int n){
        int rev = 0;
        while(n!=0){
            int d = n%10;
            rev = rev*10 + d;
            n = n/10;
        }
        return rev;
    }    
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        System.out.println(reverseofdigits(n));
    }
}


//check palindrome

import java.util.Scanner;

public class ControlFlow {
    public static boolean palindrome(int n){
        int m=n;
        int rev = 0;
        while(n!=0){
            int d = n%10;
            rev = rev*10 + d;
            n = n/10;
        }
        return rev==m;
    }    
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        System.out.println(palindrome(n)?"palindrome":"not palindrome");
    }
}

//perfect number

import java.util.Scanner;

public class ControlFlow {
    public static boolean perfect(int n){
        int sum=0;
        for(int i=1;i<=n/2;i++){
            if(n%i==0){
                sum = sum + i;
            }
        }
        return sum==n;
    }    
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        System.out.println(perfect(n)?"perfect":"not perfect");
    }
}

//armstrong number

import java.util.Scanner;

// public class ControlFlow {
//     public static boolean palindrome(int n){
//         int m=n;
//         int rev = 0;
//         while(n!=0){
//             int d = n%10;
//             rev = rev*10 + d;
//             n = n/10;
//         }
//         return rev==m;
        
//     }    
//     public static void main(String args[]) {
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter a number: ");
//         int n = sc.nextInt();
//         System.out.println(palindrome(n)?"palindrome":"not palindrome");
//     }
// }

//ARRAYS
module 5 arrays college

1.
// import java.util.Scanner;
// public class ControlFlow {
//     public static void main(String args[]) {
//         int n = 30;
//         boolean arr[] = new boolean[n];
//         Scanner sc = new Scanner(System.in);
//         for(int i=0;i<n;i++){
//             arr[i] = sc.next().equals("p")?true:false;
//         }
//         int countP = 0;
//         for(boolean b : arr){
//             if(b){
//                 countP++;
//             }
            
//         }
//         System.out.println("present" +countP);
//         System.out.println("present" +(n-countP));
//         System.out.println("present" +((float)countP/n*100));
        
       
//     }
// }

2.
// import java.util.Scanner;
// public class ControlFlow {
//     public static void main(String args[]) {
//         int n = 30;
//         float ar[] = new float[n];
//         Scanner sc = new Scanner(System.in);
//         for(int i=0;i<n;i++){
//             ar[i] = sc.nextFloat();
//         }
//         float max = ar[0];
//         float min = ar[0];
//         float sum = 0;
        
//         for(float p : ar){
//             if(p>max){
//                 max = p;
//             }
//             if(p<min){
//                 min = p;
//                 sum = sum + p;
//             }
//         }
//         System.out.println("totalbill" +sum);
//         System.out.println(" highprice" +max);
//         System.out.println("lowest price" +min);
//         System.out.println("average price" +sum/n);
        
       
//     }
// }


3.
// import java.util.Scanner;
// public class ControlFlow {
//     public static void main(String args[]) {
//         int n = 30;
//         float ar[] = new float[n];
//         Scanner sc = new Scanner(System.in);
//         for(int i=0;i<n;i++){
//             ar[i] = sc.nextFloat();
//         }
//         float max = ar[0];
//         float min = ar[0];
//         float sum = 0;
        
//         for(float p : ar){
//             if(p>max){
//                 max = p;
//             }
//             if(p<min){
//                 min = p;
//                 sum = sum + p;
//             }
//         }
//         float avg = sum/n;
//         int countAboveAvg = 0;
//         for(float t:ar){
//             if(t>avg){
//                 countAboveAvg++;
//             }
//         }
//         System.out.println("totalbill" +max);
//         System.out.println(" highprice" +min);
//         System.out.println("lowest price" +avg);
//         System.out.println("average price" +countAboveAvg);
        
       
//     }
// }
