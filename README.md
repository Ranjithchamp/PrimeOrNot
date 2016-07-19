# PrimeOrNot
import java.util.Scanner;

public class Prime {
	public static void main(String []arg)
	{
		int l=0;
		Scanner get=new Scanner(System.in);
		int input=get.nextInt();
		if(input==1 || input==0)
		{
			System.out.println("It is neither prime nor composite");
		}
		else
		{
			for(int i=2;i<input;i++)
			{
				if(input%i==0)
				{
					l=1;
					break;
				}
			}
		}
		if(l==0){
			System.out.println("It is prime");
		}
		else
		{
			System.out.println("It is not a prime number");
		}
	}

}
