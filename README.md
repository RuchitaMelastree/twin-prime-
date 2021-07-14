# twin-prime-
import java.util.*;
public  class twin_prime
{
    static int prime(int num)
    {
        int f=0,i;
        for(i=2;i<=num/2;i++)
        {
            if(num%i==0)
            {
                f=1;
                break;
            }
        }
        return f;
    }
public static void main(String[]args)
{
    int num,num1,i;
    Scanner sc= new Scanner (System.in);
    System.out.println("Enter starting number" );
    num=sc.nextInt();
    System.out.println("Enter last number");
    num1=sc.nextInt();
    System.out.println("twin prime numbers are ...");
    for(i=num;i<=num1;i++)
    {
        if(prime(i)==0&&prime(i+2)==0)
        {
            System.out.println(i+"   "+(i+2));
            }
            
        }
    }
}
