# CODE_100
### STARTED ON 17 DEC, 2021

21 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt(); // LENGTH OF CANDY --> 3
		   int k = sc.nextInt(); // UNIT TO BE EATEN --> 1
		   int r = 0, m = 0;
		   r = n % k;
		   if(r == 0)
		   {
		      m = n / k;
		      System.out.println(m);
		   }
		   else 
		      System.out.println("-1");
		 }
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int g1 = sc.nextInt();
		   int s1 = sc.nextInt();
		   int b1 = sc.nextInt();
		   int g2 = sc.nextInt();
		   int s2 = sc.nextInt();
		   int b2 = sc.nextInt();
		   int t1 = g1 + s1 + b1;
		   int t2 = g2 + s2 + b2;
		   if(t1 > t2)
		   System.out.println("1");
		   else
		   System.out.println("2");
		}
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		// CHEF --> X MIN --> P WRONG SUBMISSION
      // CHEFINA --> Y MIN --> Q WRONG SUBMISSION
      // WRONG SUBMISSION --> 10 MIN PENALTY
      for(int i=0; i<t; i++)
      {
         int x = sc.nextInt();
         int y = sc.nextInt();
         int p = sc.nextInt();
         int q = sc.nextInt();
         int m = 0, f = 0;
         m = x + (10*p); // CHEF
         f = y + (10*q); // CHEFINA
         if(m>f)
         System.out.println("CHEFINA");
         else if(f>m)
         System.out.println("CHEF");
         else
         System.out.println("DRAW");
      }
  }
}


import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int j=0; j<t; j++)
		{
		   // A min --> each inter-district e-pass --> 0
		   // B min --> each inter-state e-pass --> 1
		   int n = sc.nextInt();
		   int a = sc.nextInt();
		   int b = sc.nextInt();
		   int A = 0, B = 0;
		   int tt = 0;
		   sc.nextLine();
		   String s = sc.nextLine();
		   for(int i=0; i<n; i++)
		   {
		      char ch;
		      ch = s.charAt(i);
		      if(ch == '0')
		      A++;
		      else
		      B++;
		   }
		   tt = (a*A) + (b*B);
		   System.out.println(tt);
		}
	}
}


import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int a = sc.nextInt();
		   int b = sc.nextInt();
		   int a1 = sc.nextInt();
		   int b1 = sc.nextInt();
		   int a2 = sc.nextInt();
		   int b2 = sc.nextInt();
		   if((a == a1 || a == b1) && (b == a1 || b == b1))
		   System.out.println("1");
		   else if((a == a2 || a == b2) && (b == a2 || b == b2))
		   System.out.println("2");
		   else
		   System.out.println("0");
		 }
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
	   for(int i=0; i<t; i++)
	   {
	      int d = sc.nextInt();
	      int x = sc.nextInt(); // x unit of work everyday
	      int y = sc.nextInt(); // y unit of work for first d day
	      int z = sc.nextInt(); // z unit of work for 7-d day
	      int f = 0;
	      f = x * 7;
	      int s = 0;
	      s = (y * d) + z * (7 - d);
	      int max = 0;
	      max=Math.max(f,s);
	      System.out.println(max);
	   }
      }
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int j=0; j<t; j++)
		{
		   int a[] = new int[5];
		   int e = 0, b=0, d=0;
		   for(int i=0; i<5; i++)
		   {
		      a[i] = sc.nextInt();
		      if(a[i] == 0)
		      d++; // DRAW
		      else if(a[i] == 1)
		      b++; // INDIA
		      else 
		      e++;
		   }
		   if(b>e)
		   System.out.println("INDIA");
		   else if(e>b)
		   System.out.println("ENGLAND");
		   else if(e==b)
		   System.out.println("DRAW");
		}
	}
}

20 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int g = 0, b = 0;
		   int a[] = new int[7];
		   for(int j=0; j<7; j++)
		   {
		      a[j] = sc.nextInt();
		      if(a[j] == 1)
		      g++;
		      else if(a[j] == 0)
		      b++;
		   }
		   if(g>b)
		   System.out.println("YES");
		   else
		   System.out.println("NO");
		}
	}
}


import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int count = 0;
		   long e = sc.nextLong();
		   long k = sc.nextLong();
		   double x = 0;
		   while(e != 0)
		   {
		      e = e/k;
		      count ++;
		   }
		   System.out.println(count);
	       }
	}
}


19 JAN, 2022

import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		int t = sc.nextInt();
		for(int j=0; j<t; j++)
		{
	      int n = sc.nextInt();
		   int i;
		   if(n == 1)
		   {
		      System.out.println("no");
		      continue;
		   }
		   boolean isPrime = true;
		   for(i=2; i<n; i++)
		   {
		      if(n%i == 0)
		      {
		      isPrime = false;
		      break;
		   }
		   }
		   if(isPrime)
		   System.out.println("yes");
		   else
		   System.out.println("no");
		}
	}
}

import java.util.Scanner;
class Main
{ 
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int count = 0;
		   long k = sc.nextLong();
		   if(k%2 != 0)
		   System.out.println("0");
		   else
		   {
		      while(k%2 == 0)
		      {
		         count ++;
		         k = k/2;
		      }
		      if(count > 0)
		      System.out.println(count);
		      else
		      System.out.println("0");
		   }
		}
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
	   // a --> x votes
	   // b --> y votes
	   // c --> z votes
	   // strictly greater than 50 votes --> clear majority
	   for(int i=0; i<t; i++)
	   {
	      int a = sc.nextInt();
	      int b = sc.nextInt();
	      int c = sc.nextInt();
	      if(a>50)
	      System.out.println("A");
	      else if(b>50)
	      System.out.println("B");
	      else if(c>50)
	      System.out.println("C");
	      else
	      System.out.println("NOTA");
	   }
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		// 52 CARDS IN TOTAL
      // K-1 FRNDS
      // TOTAL K PEOPLE WILL PLAY THE GAME --> K-1 FRNDS + ALICE HERSELF 
      // EACH PERSON SHOULD HAVE EQUAL NO. OF CARDS
      for(int i=0; i<t; i++)
      {
         int k = sc.nextInt();
         // 03 --> 1
         // 50 --> 2
         // 02 --> 0
         // 14 --> 10
         int r = 0;
         r = 52 % k;
         System.out.println(r);
      }
      
	}
}

18 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt(); 
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt(); //12
		   sc.nextLine();
		   String s = sc.nextLine(); //111111111111
		   char ch[] = {'a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p'};
		   String a,l="";
		   int b=0, r=0,w=1, ans=0;
		   int m,c=0; 
		   for(int j=0; j<=n-4; j=j+4) //j--> 4 8
		   {
		       c++;
		       a = s.substring(j,j+4); //(0,4) (4,8)
		       m = Integer.parseInt(a); //1111
		       while(m!=0)
		       {
		          r = m % 10; 
		          m = m / 10; 
		          ans = ans + r*w; 
		          w = w * 2; 
		       }
		       l = l + ch[ans]; 
		       ans = 0;
		       w = 1;
		    }
		    System.out.println(l);
   	}
	}
}


17 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt();
		   sc.nextLine();
		   String s = sc.nextLine();
		   String K;
		   int d=n/4;
		   for(int j=0; j<d; j++)
		   {
		       K = s.substring(0,4);
		       s = s.substring(4);
                if (K.equals("0000"))
                    System.out.print("a");

                else if (K.equals("0001"))
                    System.out.print("b");

                else if (K.equals("0010"))
                    System.out.print("c");

                else if (K.equals("0011"))
                    System.out.print("d");

                else if (K.equals("0100"))
                    System.out.print("e");

                else if (K.equals("0101"))
                    System.out.print("f");

                else if (K.equals("0110"))
                    System.out.print("g");

                else if (K.equals("0111"))
                    System.out.print("h");

                else if (K.equals("1000"))
                    System.out.print("i");

                else if (K.equals("1001"))
                    System.out.print("j");

                else if (K.equals("1010"))
                    System.out.print("k");

                else if (K.equals("1011"))
                    System.out.print("l");

                else if (K.equals("1100"))
                    System.out.print("m");

                else if (K.equals("1101"))
                    System.out.print("n");

                else if (K.equals("1110"))
                    System.out.print("o");

                else if (K.equals("1111"))
                    System.out.print("p");	       
		   }
		 System.out.println();  
		}
	}
}


import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt(); // n is the number of balls
		   int r[] = new int[3];
		   int g[] = new int[3];
		   int b[] = new int[3];
		   for(int j=0; j<3; j++)
		   {
		      r[j] = sc.nextInt();
		   }
		   for(int j=0; j<3; j++)
		   {
		      g[j] = sc.nextInt();
		   }
		   for(int j=0; j<3; j++)
		   {
		      b[j] = sc.nextInt();
		   }
		   int lt = 0;
		   lt = g[0] + b[0] + b[1];
		   int ut = 0;
		   ut = r[1] + r[2] + g[2];
		   int max = 0;
		   max = Math.max(lt,ut);
		   System.out.println(max);
		   
		}
	}
}


import java.util.Scanner;
import java.util.Arrays;
class Main
{
   public static void main(String[] args)
   {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt(); 
        for (int i = 0; i < t; i++)
        {
            int n = sc.nextInt(); 
            int x = sc.nextInt(); 
            int a[] = new int[n];
            int sum = 0, in = 0, temp = 0;
            boolean flag = true;

            for (int j = 0; j < n; j++)
            {
                a[j] = sc.nextInt(); 
                sum = sum + a[j];  
            }
            
            if (sum < x) 
            {
               System.out.println("-1");
               flag = false;
            }
            
            else
            {
            Arrays.sort(a); 
            
            for (int j = 0; j < n / 2; j++)  // ARRAY REVERSE
            {
               temp = a[j];
               a[j] = a[n - j - 1];
               a[n - j - 1] = temp;
            }
         
            int count = 0;
            
            int sum2 = 0;
            for (int j = 0; j < n; j++)
            {
               sum2 = sum2 + a[j]; 
               count ++; 
               if (sum2 >= x)
               {
                  flag = true;
                  break;
               }
            }
            
            if(flag)
            {
               System.out.println(count);
               count = 0;
            }
         }
    }
      
   }
}

15 JAN, 2022

9 GFG QUES

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int j=0; j<t; j++)
		{
		   int n = sc.nextInt(); // SETTERS
		   long k = sc.nextLong(); // PROBLEMS IN A CONTEST
		   long d = sc.nextLong(); // NO. OF DAYS
		   long a[] = new long [n];
		   long sum = 0;
		   for(int i=0; i<n; i++)
		   {
		      a[i] = sc.nextInt();
		      sum = sum + a[i];
		   }
		   if(sum < k)
		   System.out.println("0");
		   else if(sum == k)
		   System.out.println("1");
		   else
		   {
		      long g = 0;
            g = sum / k;
            if(g <= d)
            System.out.println(g);
            else
            System.out.println(d);
		   }
		}
	}
}


14 JAN, 2022

{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int d1 = sc.nextInt(); //DSA
		   int d2 = sc.nextInt();
		   int d3 = sc.nextInt();
		   int s1 = sc.nextInt();
		   int s2 = sc.nextInt();
		   int s3 = sc.nextInt();
		   int sumd = d1 + d2 + d3;
		   int sums = s1 + s2 + s3;
		   if(sumd == sums && d1 == s1 && d2 == s2)
		   System.out.println("TIE");
		   else
		   {
		   if(sumd > sums)
		   System.out.println("DRAGON");
		   else if(sums > sumd)
		   System.out.println("SLOTH");
		   else
		   {
		      if(d1 > s1)
		      System.out.println("DRAGON");
		      else if(s1 > d1)
		      System.out.println("SLOTH");
		      else
		      {
		         if(d2 > s2)
		         System.out.println("DRAGON");
		         else if(s2 > d2)
		         System.out.println("SLOTH");
		      }
		    }  
	    }
	}
   }
}

13 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt(); // no. of friends
		   int x = sc.nextInt(); // amount of gold in the mine
		   int y = sc.nextInt(); // atmost y kg capacity of each person
		   int r = 0;
		   r = (n+1)*y;
		   if(r>=x)
		   System.out.println("YES");
		   else
		   System.out.println("NO");
		}
	}
}


12 JAN, 2022

1 gfg ques

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		// A, B, C --> COMBOS
		for(int i=0; i<t; i++)
		{
		   int a1 = sc.nextInt(); // COMBO A POPCORN
		   int a2 = sc.nextInt(); // COMBO A COKE
		   int b1 = sc.nextInt(); // COMBO B POPCORN
		   int b2 = sc.nextInt(); // COMBO B COKE
		   int c1 = sc.nextInt(); // COMBO C POPCORN
		   int c2 = sc.nextInt(); // COMBO C COKE
		   int a = a1 + a2;
		   int b = b1 + b2;
		   int c = c1 + c2;
		   double max = 0.0;
		   max = Math.max(a,Math.max(b,c));
		   int maxi;
		   maxi = (int) max;
		   System.out.println(maxi);
		}
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		// n --> total no. of slippers
		// l --> no. of left slippers
		// x --> the price of a pair of slippers in rupees
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt();
		   int l = sc.nextInt();
		   int x = sc.nextInt();
		   int p = 0;
		   int r = 0;
		   //System.out.println(l);
		   r = n - l;
		   //System.out.println(r);
		   if(l >= r)
		   {
		     p = r * x;
		     System.out.println(p);
		   }
		   else if(r > l)
		   {
		     p = l * x;
		     System.out.println(p);
		   }
		   p = 0;
		}
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
      for(int i=0; i<t; i++)
      {
         int r = sc.nextInt();
         if(r >= 2000)
         System.out.println("1");
         else if(r >= 1600 && r < 2000)
         System.out.println("2");
         else if(r < 1600)
         System.out.println("3");
      }
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt();
		   // N -> E -> S -> W 
		   if(n % 4 == 0)
		   System.out.println("NORTH");
		   else if(n % 4 == 1)
		   System.out.println("EAST");
		   else if(n % 4 == 2)
		   System.out.println("SOUTH");
		   else
		   System.out.println("WEST");
		}
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int time = 0;
	   // n --> no. of people in queue
	   // p --> position from front at which chef is standing
	   // x --> child vaccine min
      // y --> elder vaccine min
      for(int i=0; i<t; i++)
      {
         int n = sc.nextInt();
         int p = sc.nextInt();
         int x = sc.nextInt();
         int y = sc.nextInt();
         int a[] = new int[n];
         for(int j = 0; j < n; j++)
         {
            a[j] = sc.nextInt();
         }
         n = p;
         int b[] = new int[n];
         for(int j = 0; j < n; j++)
         {
            b[j] = a[j]; 
         }
         for(int j = 0; j < n; j++)
         {
            if(a[j] == 0)
            time = time + x;
            else if(a[j] == 1)
            time = time + y;
         }
         System.out.println(time);
         time = 0;
      }
	}
}


11 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		int a = sc.nextInt();
		int b = sc.nextInt();
		int c = sc.nextInt();
		int d = sc.nextInt();
		int sum1 = 0;
		int sum2 = 0;
		sum1 = a + c;
		sum2 = b + d;
		if(sum1 == 180 && sum2 == 180)
		System.out.println("YES");
		else
		System.out.println("NO");
	}
}
}

import java.util.Arrays;
import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int a[] = new int[t];
		for(int i=0; i<t; i++)
		{
		   a[i] = sc.nextInt();
		}
		Arrays.sort(a);
		for(int i=0; i<t; i++)
		{
		   System.out.println(a[i]);
		}
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		
		// FUEL ECONOMY --> DIS TRAVEL IN 1L OF FUEL
		// BASE FUEL ECONOMY --> FE WHEN THERE IS ONLY ONE PERSON (M KM/L)
		// EVERY EXTRA PASSENGER DEC THE FE BY 1 KM/L
		// P --> NO. OF PEOPLE
		// V --> L OF FUEL
		
		// MAX DIS TRAVELLED UNDER GIVEN CONDITION
		
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int p = sc.nextInt(); // no. of people (5)
		   int m = sc.nextInt(); // base fuel economy (10)
		   int v = sc.nextInt(); // amount of fuel
		   int d = 0;
		   d = p - 1; // extra passenger (4)
		   int e = 0; // effective fuel economy
		   e = m - d; // (6)
		   int max = 0;
		   max = e * v;
		   System.out.println(max);
		   
		}
	}
}

NEW STREAK START

***

8 JAN, 2022

3 GFG QUES

// WRONG
import java.util.Scanner;
public class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int k = 0;
		sc.nextLine(); 
		for(int i=0; i<t; i++)
		{
		   String s = sc.nextLine();
		   int l = 0;
		   l = s.length();
		   if(l == 1)
		   System.out.println("NO"); 
		   else
		   {
		      for(int j=0; j<l-2; j++)
		      {
		         String x;
		         x = s.substring(j,j+2);
		         if(x.equals("10") || x.equals("11"))
		         {
		             k++;
		             System.out.println("YES");
		             break;
		         }
		         else
		         {
		             String y;
		             y = s.substring(l-2);
		             if(y.equals("10") || y.equals("11"))
		             System.out.println("YES");
		         }
		      }
		   }
		}
	}
}

7 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		for(int i = 0; i < n; i++)
		{
		   double t1, t2, r1, r2;
		   t1 = sc.nextDouble();
		   t2 = sc.nextDouble();
		   r1 = sc.nextDouble();
		   r2 = sc.nextDouble();
		   double d1;
		   double d2;
		     d1 = (t1 * t1)/(r1 * r1 * r1);
           d2 = (t2 * t2)/(r2 * r2 * r2);
           if(d1 == d2)
           System.out.println("YES");
           else
           System.out.println("NO");
           d1 = 0.0;
           d2 = 0.0;
      }
	}
}

import java.util.Scanner;
import java.lang.Math;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
	   int r = 0;
	   int v = 0;
	   
	   // DAY 0 --> 1 PERSON IS INFECTED
      // NEXT 10 DAYS --> INFECTED PEOPLE DOUBLES EACH DAY 
      // FROM 11 DAY ONWARDS --> INFECTED PEOPLE TRIPLES EACH DAY 
      // N --> POPULATION
      // D --> DAY
      
      for(int i = 0; i < t; i++)
      {
         int n = sc.nextInt();
         int d = sc.nextInt();
         double f = 0.0; // INFECTED
         if(d<=10)
         {
            {
               f = Math.pow(2,d); 
            }
            v = (int)f;
            if(f < n)
            System.out.println(v);
            else
            System.out.println(n);
         }
         if(d>=11)
         {
            f = Math.pow(2,10);
            r = d - 10;
            double f2 = 0.0;
            f2 = f * Math.pow(3,r);
            v = (int)f2;
            if(v < n)
            System.out.println(v);
            else
            System.out.println(n);
         }
      }
 	}
}

6 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		int k = 1;
		int t = 0;
		for(int i = 1; i <= n; i++)
		{
		   if(i % 2 != 0)
		   {
		      for(int j = 1; j <= 5; j++)
		      {
		        System.out.print(k + " ");
		        k = k + 1;
		      }
		      System.out.println();
		      t = k;
		   }
		   else
		   {
		      t = t + 4;
		      for(int j = 1; j <= 5; j++)
		      {
		         System.out.print(t + " ");
		         t = t - 1;
		      }
		      System.out.println();
		      k = t + 6;
		   }
	  }
	}
}


import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
      int a = sc.nextInt();
	   int b = sc.nextInt();
   	int c = sc.nextInt();
      if((a + b + c == 180) && (a > 0) && (a <= 178) && 
         (b > 0) && (b <= 178) && (c > 0) && (c <= 178)) 
      System.out.println("YES");
      else
      System.out.println("NO");
   }
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
      int a = sc.nextInt();
	   int b = sc.nextInt();
   	int c = sc.nextInt();
      if((a + b > c) && (b + c >a) && (c + a > b))
      {
         if (a == b && b == c)
         System.out.println("1");
         else if (a == b || b == c || c == a)
         System.out.println("2");
         else if (a != b && b != c && c != a)
         System.out.println("3");
      }
      else
      System.out.println("-1");
   }
}

import java.util.Scanner;
import java.util.Arrays;
class Main 
{ 
   public static void main(String[] args) 
   { 
      Scanner sc = new Scanner(System.in); 
      int n = sc.nextInt(); 
      int k = sc.nextInt(); 
      int t = 0;
      int a[] = new int[n]; 
      for(int i = 0; i<n; i++)
      {
         a[i] = sc.nextInt(); 
      }
      Arrays.sort(a);
      t = Arrays.binarySearch(a,k);
      if(t >= 0)
      System.out.println("1");
      else 
      System.out.println("-1");
   }
}

import java.util.Scanner;
import java.util.Arrays;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
      int a = sc.nextInt();
	   int b = sc.nextInt();
   	int c = sc.nextInt();
      if((a + b > c) && (b + c >a) && (c + a > b))
      System.out.println("YES");
      else
      System.out.println("NO");
   }
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		long n = sc.nextLong();
	   long odd = 0;
	   long even = 0;
	   odd = n * n;
	   even = n * (n + 1);
	   System.out.println(odd + " " + even);
	}
}


5 JAN, 2022

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		if(n % 5 == 0 || n % 6 == 0)
		System.out.println("YES");
		else
		System.out.println("NO");
	}
}

import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int l = sc.nextInt();
		int r = sc.nextInt();
		for(int i = l; i <= r; i++)
		{
		   if(i % 2 != 0)
		   System.out.print(i + " ");
		}
	}
}

import java.util.Scanner;
import java.util.Arrays;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
      int a = sc.nextInt();
	   int b = sc.nextInt();
   	int c = sc.nextInt();
   	int arr[] = new int[3];
   	arr[0] = a;
   	arr[1] = b;
   	arr[2] = c;
   	Arrays.sort(arr);
      System.out.println(arr[1]);
   }
}


import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int z = sc.nextInt();
		   int y = sc.nextInt();
		   int a = sc.nextInt();
		   int b = sc.nextInt();
		   int c = sc.nextInt();
		   int d = 0;
		   d = z - y;
		   int sum = 0;
		   sum = a + b + c;
		   if(d >= sum)
		   System.out.println("YES");
		   else
		   System.out.println("NO");
		   
		}
	}
}


import java.util.Scanner;
class Main
{
	public static void main (String[] args) 
	{
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		for(int i=0; i<t; i++)
		{
		   int n = sc.nextInt(); // NUMBER OF ROWS
		   int m = sc.nextInt(); // NUMBER OF SEATS IN EACH ROW
         if (n == 1 || n == 2)
         {
            int r = 0;
            r = m % 2;
            if (r == 0)
            System.out.println(m/2);
            else
            {
               m = m + 1;
               System.out.println(m/2);
            }
         }
         
         if(n > 2)
         {
            int s = 0;
            s = n % 2;
            if(s == 0)
            {
               n = n/2;
               int r = 0;
               r = m % 2;
               if (r == 0)
               System.out.println((n*m)/2);
               else
               {
                  m = m + 1;
                  System.out.println((n*m)/2);
               }
            }
            else
            {
               n = n + 1;
               n = n/2;
               int r = 0;
               r = m % 2;
               if (r == 0)
               System.out.println((n*m)/2);
               else
               {
                  m = m + 1;
                  System.out.println((n*m)/2);
               }
            }
		   }
	  }
	}
}

4 JAN, 2022

NO QUESTION


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
