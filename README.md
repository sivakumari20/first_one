# first_one

when the error cannot be resolved to a variable occurs 
initialise it before loops or method 
if it is necesary declare initial values

*factorial of a number*
fact cannot be resolved to a variable
package First_one;
import java.util.Scanner;
public class factorial {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc=new Scanner(System.in);
		System.out.println("enter the number you want to find the factorial");
		int x=sc.nextInt();
		int fact=1;
			
		for(int i=1;i<=x;i++)
		{
		    fact=fact*i;
		}
		System.out.println(fact);
		
		
		

	}

}
2.palindrome number
import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc =new Scanner(System.in);
		try {
		int x,temp,sum=0;
		System.out.println("enter a number you want to find out palindrome for");
		int n=sc.nextInt();
	   // int n=989;
		temp=n;

		while(n>0)
		{
			x=n%10;
			sum=sum*10+x;
			n=n/10;
		}
		if(temp==sum)
		{
			System.out.println("given number is a palindrome number");
		}
		else
		{
			System.out.println("given number is not a palindrome number");
		}
		}
		catch(Exception e) {
			System.out.println("error:invalid input");
			
		}finally 
		{
		  	sc.close();  
		}
		

	}
}

** fibanocci series **
import java.util.Scanner;

public class Main {
//fibanocci series
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc =new Scanner(System.in);
		int a=0,b=1,c;
		System.out.println("enter a number you want to find out series upto for");
		int n=sc.nextInt();
	   // int n=989;
	   int x;
        c=a+b;
		for(int i=0;i<=n;i++)
		{
	
			System.out.print(fibanocci(i)+ " ");
			
		}
	}
	public static int fibanocci(int n)
		{
		    if (n==0)
		    {
		        return 0;
		    }
		    else if(n==1)
		    {
		        return 1;
		        
		    }
		    else{
		        return fibanocci(n-1)+fibanocci(n-2);
		    }
		}
		
	}


