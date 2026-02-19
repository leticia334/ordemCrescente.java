import java.util.Scanner;

 public class ordemCrescente{
      public static void main(String [] args){
        Scanner sc = new Scanner(System.in);

        int n1, n2, n3, temp;

        System.out.print("digite o primeiro numero: ");
        n1 = sc.nextInt();

        System.out.print("digite o segundo numero: ");
        n2 = sc.nextInt();

        System.out.print("digite o terceiro numero: ");
        n3 = sc.nextInt();

        if (n1 > n2){
            temp = n1;
            n1 = n2;
            n2 = temp;
        }

        if (n1 > n3){
            temp = n1;
            n1 =n3;
            n3 = temp;
        }

        if (n2 > n3){
            temp = n2;
            n2 = n3;
            n3 =temp;
        }

        System.out.println("ordem crescente: " + n1 + " " + n2+ " " +n3);
        sc.close();
    }
}
