# CODE_100

3 JAN, 2O22

import java.util.Scanner;
public class Solution 
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int n;
        n = sc.nextInt();
        int a[] = new int[n];
        for(int i = 0; i<n; i++)
            a[i] = sc.nextInt();
        for(int i = n-1; i>=0; i--)
            System.out.print(a[i] + " ");
    }
}


import java.util.Scanner;
class Main 
{ 
   public static void main(String[] args) 
   { 
      Scanner sc = new Scanner(System.in); 
      int n; 
      n = sc.nextInt(); 
      int a[] = new int[n]; 
      for(int i = 0; i<n; i++)
      a[i] = sc.nextInt(); 
      for(int i = n-1; i>=0; i--) 
      System.out.print(a[i] + " "); 
   } 
}


import java.util.Scanner;
public class Main
{
public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();
        for (int i = 0; i < t; i++)
        {
            int a = sc.nextInt();
            int b = sc.nextInt();
            int r = 0, m = 0;
            int sum = 0;
            sum = a + b;
            int k = 0;
            while (sum != 0)
            {
                r = sum % 10;
                if (r == 0)
                    m = 6;
                else if (r == 1)
                    m = 2;
                else if (r == 2)
                    m = 5;
                else if (r == 3)
                    m = 5;
                else if (r == 4)
                    m = 4;
                else if (r == 5)
                    m = 5;
                else if (r == 6)
                    m = 6;
                else if (r == 7)
                    m = 3;
                else if (r == 8)
                    m = 7;
                else if (r == 9)
                    m = 6;
                k = k + m; 
                sum = sum / 10;
            }
            System.out.println(k);
        }
    }
}

***

17 DEC,2021

Codechef practice problem 01
import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt();
		   if(n<10)
		   System.out.println("Thanks for helping Chef!");
		   else
		   System.out.println("-1");
		}
	}
}


Codechef practice problem 02
import java.util.Scanner;
public class Main
{
	public static void main (String[] args)
	{
		Scanner sc=new Scanner(System.in);
		int n=sc.nextInt();
		int t;
		t=n;
		if(n%4==0)
		t++;
		else
		t--;
		System.out.println(t);
	}
}


Codechef practice problem 03
import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
	   int n=sc.nextInt();
	   System.out.println(n);
	}
}


Codechef practice problem 04
import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
      for(int i=0; i<t; i++)
      {
		  int a = sc.nextInt();
		  int b = sc.nextInt();
        int c=0;
        c=a%b;
        System.out.println(c);
      }
   }
}


18 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   char ch = sc.next().charAt(0);
		   switch(ch)
		   {  //next().charAt(0)
		      case 'B':
		         System.out.println("BattleShip");
		         break;
		      case 'b':
		         System.out.println("BattleShip");
		         break;
		      case 'C':
		         System.out.println("Cruiser");
		         break;
		      case 'c':
		         System.out.println("Cruiser");
		         break;
		      case 'D':
		         System.out.println("Destroyer");
		         break;
		      case 'd':
		         System.out.println("Destroyer");
		         break;
		      case 'F':
		         System.out.println("Frigate");
		         break;
		      case 'f':
		         System.out.println("Frigate");
		         break;
		   }
	   }
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		char ch = sc.next().charAt(0);
	   if(ch=='A'|| ch=='E' || ch=='I' || ch=='O' || ch=='U')
		   {
		       System.out.println("Vowel");
		   }
		   else
		   {
		         System.out.println("Consonants");
		   }
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int l = sc.nextInt();
		int b = sc.nextInt();
		int area = 0;
		area = l*b;
		int peri = 0;
		peri = l+l+b+b;
		if(area > peri)
		{
	   	System.out.println("Area");
	   	System.out.println(area);
		}
		if(peri>area)
		{
		   System.out.println("Peri");
		   System.out.println(peri);
		}
		if(area==peri)
		{
		    System.out.println("Eq");
		    System.out.println(area);
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		  int a = sc.nextInt();
		  int b = sc.nextInt();
		  if(a>b)
		  System.out.println(">");
		  else if(a<b)
		  System.out.println("<");
		  else
		  System.out.println("=");
	   }
   }
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		int mul = 1;
		for(int i=0; i<t; i++)
		{
		   int n=sc.nextInt();
		   for(int j=n;j>1;j--)
		   {
		      mul = mul * j;
		   }
		   System.out.println(mul);
		   mul=1;
		}
	}
}


19 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		int c=0;
		int r=0;
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt();
		   while(n!=0)
		   {
		      r=n%10;
		      if(r==4)
		      {
		         c++;
		      }
		      n=n/10;
		   }
		   System.out.println(c);
		   c=0;
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
	   int t = sc.nextInt();
	   for(int i=0; i<t; i++)
	   {
	      int a = sc.nextInt();
	      int b = sc.nextInt();
	      int sum = 0;
	      sum = a + b;
	      if(sum % 2 == 0)
	      System.out.println("BOB");
	      else
	      System.out.println("ALICE");
	   }
	}
}


20 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int a, b, c;
		   a = sc.nextInt();
		   b = sc.nextInt();
		   c = sc.nextInt();
		   int x=0, y=0, z=0;
		   x=a+b;
		   y=b+c;
		   z=a+c;
		   if(a == y || b == z || c == x)
		   System.out.println("Yes");
		   else
		   System.out.println("No");
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int x1, x2, y1, y2, z1, z2;
		   x1 = sc.nextInt();
		   x2 = sc.nextInt();
		   y1 = sc.nextInt();
		   y2 = sc.nextInt();
		   z1 = sc.nextInt();
		   z2 = sc.nextInt();
		   if(x2>=x1 && y2>=y1 && z2<=z1)
		   System.out.println("Yes");
		   else
		   System.out.println("No");
		 }
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int a = sc.nextInt();
		int b = sc.nextInt();
	  	if(a>b)
		{
		   System.out.println(a-b);
		}
		else
		{
		   System.out.println(a+b);
	   }
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
	   // soldier --> lucky --> Even no. of weapons
	   //	army ready --> lucky > unlucky
	   int n = sc.nextInt(); // NO. OF SOLDIERS
	   int even = 0, odd = 0;
	   int a[] = new int[n];
	   for(int i=0; i<n; i++)
	   {
	      a[i] = sc.nextInt();
	   }
	   for(int i=0; i<n; i++)
	   {
	      int t=0;
	      t=a[i];
	      if(t%2==0)
	      {
	         even++;
	      }
	      else
	      {
	         odd++;
	      }
	   }
	   if(even>odd)
	   System.out.println("READY FOR BATTLE");
	   else
	   System.out.println("NOT READY");
	}
}


21 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int a = sc.nextInt(); // Jitne paise hai
		   int b = sc.nextInt(); // Jitne paise krne hai
		   int x = sc.nextInt(); // Ek saal mei kitne inc ho rhe hai
		   int diff = 0;
		   int k;
		   diff = b - a;
		   k = diff/x;
		   System.out.println(k);
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int a, b, c, d;
		   a = sc.nextInt();
		   b = sc.nextInt();
		   c = sc.nextInt();
		   d = sc.nextInt();
		   int sum = 0;
		   int s = 0;
		   s=c/a;
		   int x = 0;
		   x=d/b;
		   sum = s+x;
		   System.out.println(sum);
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt();
		   int r = 0;
		   r = n%4;
		   if(r>=2)
		   System.out.println("YES");
		   else
		   System.out.println("NO");
		}
	}
}


22 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int x = sc.nextInt();
		   int k = 0, r=0;
		   k=x;
		   r = x%10;
		   if(r == 5)
		   System.out.println("1");
		   else if (r == 0)
		   System.out.println("0");
		   else
		   System.out.println("-1");
		}
	}
}


23 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int m = sc.nextInt(); // exams will start after m minutes
		   int n = sc.nextInt(); // no. of episodes in the show
		   int k = sc.nextInt(); // length of each episodes
		   int duration = 0;
		   duration = n*k;
		   if(duration < m)
		   System.out.println("YES");
		   else
		   System.out.println("NO");
		}
	}
}


24 DEC, 2021

NO QUESTION SOLVED


25 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int n = sc.nextInt();
		int k=0;
		for(int i=0; i<n; i++)
		{
		   int a[] = new int [5];
		   for(int j=0; j<5; j++)
		   {
		      a[j] = sc.nextInt();
		   }
		   for(int j=0; j<5; j++)
		   {
		      if(a[j] == 1)
		      k++;
		   }
		   switch(k)
		   {
		     case 0 : 
		        {
		           System.out.println("Beginner"); 
		           k=0;
		           break;
		        }
		     case 1 : 
		        {
		           System.out.println("Junior Developer"); 
		           k=0;
		           break;
		        }
		     case 2 : 
		        {
		           System.out.println("Middle Developer");
		           k=0; 
		           break;
		        }
		     
		     case 3 : 
		        {
		           System.out.println("Senior Developer"); 
		           k=0; 
		           break;
		        }
		     case 4 : 
		        {
		           System.out.println("Hacker");
		           k=0; 
		           break;
		        }
		     case 5 : 
		        {
		           System.out.println("Jeff Dean"); 
		           k=0;
		           break;
		        }
		    }
	   }
   }
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int n = sc.nextInt();
		int r, k=0;
		while(n!=0)
		{
		   r=n%10;
		   n=n/10;
		   k++;
		}
		if(k==1) 
		System.out.println("1");
		else if(k==2) 
		System.out.println("2");
		else if(k==3) 
		System.out.println("3");
		else
		System.out.println("More than 3 digits");
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		// HOSTED --> 2010, 2015, 2016, 2017 and 2019
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt();
		   if(n == 2010 || n== 2015 || n== 2016 || n== 2017 || n==2019)
		   System.out.println("HOSTED");
		   else
		   System.out.println("NOT HOSTED");
		}
	}
}


26 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
	   int t = sc.nextInt();
	   for(int i=0; i<t; i++)
	   {
	      int n = sc.nextInt(); // N --> TOTAL QUESTIONS
	      int x = sc.nextInt(); // X --> CORRECT QUESTIONS
	      int p = sc.nextInt(); // P --> PASSING MARKS (ATLEAST)
	      int marks = 0;
	      marks = 3*x - (n-x);
	      if(marks >= p)
	      System.out.println("PASS");
	      else
	      System.out.println("FAIL");
	   }
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int m = sc.nextInt(); // DURATION OF THE TRIP
		   int s = sc.nextInt(); // DURATION OF THE SONG
		   int r = 0;
		   r = m/s;
		   if(m>=s)
		   System.out.println(r);
		   else
		   System.out.println("0");
		}
	}
}


27 DEC, 2021

import java.util.Scanner;
public class Main 
{
   public static void main(String[] args) 
   {
      Scanner sc = new Scanner(System.in);
      int t = sc.nextInt();
      int p2 = 0;
      sc.nextLine();
      for(int i = 1; i <= t; i++) 
      {
         String p = sc.nextLine();
         String var = p.substring(0, 2);
         int p1 = Integer.parseInt(var + p.substring(3, 5));
         char ch = p.charAt(6);
         p2 = p1;
         if (ch == 'A')
         {
            if (1200 <= p1 && p1 <= 1259) 
               p2 = p1 - 1200;
         }
         else if (ch == 'P' && p1 <= 1159) 
         {
            p2 = p1 + 1200;
         }
         int n = sc.nextInt();
         sc.nextLine();
         String[] a = new String[n];
         int[] b = new int[n];
         int[] c = new int[n];
         int j;
         for(j = 0; j < n; j++) 
         {
            a[j] = sc.nextLine();
         }
         for(j = 0; j < n; j++)
         {
            String var2 = a[j].substring(0, 2);
            b[j] = Integer.parseInt(var2 + a[j].substring(3, 5));
            var2 = a[j].substring(9, 11);
            c[j] = Integer.parseInt(var2 + a[j].substring(12, 14));
            char x1 = a[j].charAt(6);
            char x2 = a[j].charAt(15);
            if (x1 == 'A')
            {
               if (1200 <= b[j] && b[j] <= 1259)
                  b[j] = b[j] - 1200;
            }
            else if (x1 == 'P' && b[j] <= 1159) 
            {
               b[j] = b[j] + 1200;
            }
            if (x2 == 'A') 
            {
               if (1200 <= c[j] && c[j] <= 1259) 
                  c[j] = c[j] - 1200;
            } 
            else if (x2 == 'P' && c[j] <= 1159)
            {
               c[j] = c[j] + 1200;
            }
         }
         for(int k = 0; k < n; k++)
         {
            if (b[k] <= p2 && p2 <= c[k]) 
            {
               System.out.print("1");
            } 
            else 
            {
               System.out.print("0");
            }
         }
          System.out.println("");
      }
   }
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int h = sc.nextInt(); // HARDNESS
		   double c = sc.nextDouble(); // CARBON CONTENT
		   int s = sc.nextInt(); // TENSILE STRENGTH
		   if(h > 50 && c < 0.7 && s > 5600)
		   System.out.println("10");
		   else if(h > 50 && c < 0.7 && s <= 5600)
		   System.out.println("9");
		   else if (h <= 50 && c < 0.7 && s > 5600)
		   System.out.println("8");
		   else if(h > 50 && c >= 0.7 && s > 5600 )
		   System.out.println("7");
		   else if(h > 50 || c < 0.7 || s > 5600)
		   System.out.println("6");
		   else 
		   System.out.println("5");
		}
	}
}

28 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		double g = 0.0;
		for(int i=0; i<t; i++)
		{
		   /*  salary < 1500 --> HRA = 10% of base salary 
		                         DA = 90% of basic salary.
             salary >= 1500 --> HRA = Rs. 500 
                                DA = 98% of basic salary
             find his gross salary
             Gross Salary = Basic Salary + HRA + DA */
		   int salary = sc.nextInt();
		   double h = 0;
		   double d = 0;
		   if (salary < 1500)
		   {
		      h = 0.1 * salary;
		      d = 0.9 * salary;
		   }
		   if (salary >= 1500)
		   {
		      h = 500;
		      d = 0.98 * salary;
		   }
		   g = salary + h + d;
		   System.out.println(g);
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		sc.nextLine();
		int a = 0, b = 0;
		for(int i=0; i<t; i++)
		{
		   String s;
		   char ch;
		   s = sc.nextLine();
		   int n = s.length();
		   for(int j=0; j<n; j++)
		   {
		      ch = s.charAt(j);
		      if(ch == 'a')
		      a++;
		      else 
		      b++;
		   }
		   if(a==b)
		   System.out.println(a);
		   if (a>b)
		   System.out.println(b);
		   else if(b>a)
		   System.out.println(a);
		   a = 0;
		   b = 0;
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int a = sc.nextInt();
		   int b = sc.nextInt();
         int c = sc.nextInt();
         if(a>c && b>c)
         System.out.println("Alice");
         else if(c>b && a>b)
         System.out.println("Bob");
         else
         System.out.println("Draw");
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		int k=0;
		for(int i=0; i<t; i++)
		{
		   int m = sc.nextInt();
		   int n = sc.nextInt();
		   int p = sc.nextInt();
		   if(m == 7 || n == 7 || p == 7)
		   k++;
		   if(k>0)
		   System.out.println("YES");
		   else
		   System.out.println("NO");
		   k = 0;
		}
	}
}


29 DEC, 2021

NO QUESTIONS SOLVED 


30 DEC, 2021

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		// D DAYS AGO VACCINE TAKEN
		// SECOND DOSE BTW L AND R DAYS
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int d = sc.nextInt();
		   int l = sc.nextInt();
		   int r = sc.nextInt();
		   // L D R
		   if(l<=d && d<=r)
		   System.out.println("Take second dose now");
		   else if(d>r)
		   System.out.println("Too Late");
		   else
		   System.out.println("Too Early");
		}
	}
}


31 DEC, 2021

#include <stdio.h>
int max(int x, int y)
{
    if(x>y)
    return x;
    else 
    return y;
}
int main()
{
    int a, b, c, d;
    int x=0;
    scanf("%d %d %d %d", &a, &b, &c, &d);
    x = max(a, max(b, max(c,d)));
    printf("%d", x);
}


01 JAN, 2022

NO QUESTIONS SOLVED


02 JAN, 2022

>> SWAP PROGRAM
>> SUM OF N NUMBERS
>> LAST DIGIT OF NUMBER
>> HELLO WORLD
>> NEW LINE

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int a, b, x, y, sum = 0;
		a = sc.nextInt();
		b = sc.nextInt();
		x = sc.nextInt();
		y = sc.nextInt();
		sum = a*x + b*y;
		System.out.println(sum);
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int n = sc.nextInt();
		if(n%5 == 0 && n%11 == 0)
		System.out.println("BOTH");
		else if(n%5 == 0 || n%11 == 0)
		System.out.println("ONE");
		else
		System.out.println("NONE");
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int n = sc.nextInt();
		int k = 0;
		for(int i=1; i<=n; i++)
		{
		   if(n%i == 0)
		   k++;
		}
		System.out.println(k);
		for(int i=1; i<=n; i++)
		{
		   if(n%i == 0)
		   System.out.print(i +" ");
		}
	}
}


import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		long n = sc.nextInt();
		long sum = 0;
		sum = (n*(n+1))/2;
		System.out.println(sum);
	}
}
