# java-switch-tasks
A java program using switch case for number analysis.
The below mentioned code takes user generated inputs and perfoms tasks accordingly.



import java.util.*;

public class Main
{
	public static void main(String[] args)
	{
	    int n, m;
	    char c;
	    Scanner sc = new Scanner(System.in);
	    System.out.println("Enter an integer within 100");
	    n=sc.nextInt();
	    System.out.println("Enter a character in Upper Case");
	    c=sc.next().charAt(0);
	    System.out.println("Enter an integer m");
	    m=sc.nextInt();
	    switch(c)
	{
	          case 'A':
	          int count=0,res;
	          for(int i=1;i<=n/2;i++)
	          {
	              if(n%i==0) ?//to count the factors
	              count++;
	          }  
	              if(count==1) // n is prime
	              res=n*m;

	              else
	              res=n+m;

	              System.out.println("Result=" + res);
	              break;
	              

	                 case 'B':
	                 if(n%2==0) 
	                 System.out.println(n + " is an even number");
	                 else
	                 System.out.println(n + " is not an even number");
	                 break;
	               
	                   case 'C':
	                   int gcd=1;
	                   for(int i=1; i<=n && i<=m; i++) 
	                   {
	                       if(n%i==0 && m%i==0) // calculates the greatest divisor
	                       gcd=i;
	                   }
	                   System.out.println("Result= " + gcd);
	                   break;
	                   
	                   default:
	                   System.out.println("Invalid choice");
	                   break;        
	      }     
        
	    }

	}


	                 
	                 
