# Program-to-calculate-length-of-the-string-using-recursion-in-CPP

Length of the String using Recursion in C++
 

Here, in this page we will discuss the program to find the length of the string using recursion in C++ programming language. We are given with a string and need to print its length. Besides the recursive approach to solve this problem we will also discuss the iterative and using inbuilt function to find the length of the given input string.

Example :

Input : String : PrepInsta
Output : 9
Length of the String using Recursion in C++
Method 1 (Using Recursion) :
In this method we will discuss the recursive approach to find the length of the string.

Create a recursive function say Len(char* str), that return integer value.
Inside that function if *str == ‘\0’ , then return 0.
Otherwise, return (1+ Len(str+1)).
Length of the string
Code to find Length of the string using Recursion in C++
Run
#include <bits/stdc++.h>
using namespace std;

//Recursive function to calculate the length of the string
int Len(char* str) 
{
   if (*str == '\0')
      return 0;
   else
      return 1 + Len(str + 1);
}

/* Driver code */
int main()
{
   char str[] = "PrepInsta";
   cout << Len(str);
   return 0;
}
Output :

9
Method 2 (Using Loop) :
In this method we will discuss the iterative approach to find the length of the string, we can use while or for loop to count the length of the given string. Here, we will use while loop to find the length of the given string.

Create a function say Len(char* str), that return integer value.
Inside that function,
Create a variable say count and initialize it with 0,
Run a while loop that will terminate when, *str == ‘\0’ ,
Increment count by 1 and str by 1, i.e, count++ and str++
After execution of that loop return the value of count.
Code to find Length of the string using Loop in C++
Run
#include <bits/stdc++.h>
using namespace std;

//Function to calculate the length of the string
int Len(char* str) 
{  
   int count = 0;
   while (*str != '\0'){
      count++;
      str++;
   }
   return count;
}

/* Driver code */
int main()
{
   char str[] = "PrepInsta";
   cout << Len(str);
   return 0;
}
Output :

9
Method 3 (Using In-built Function) :
In this method we will use length() function to return of the given input string

Create a function say Len(string  str), that return integer value.
Inside that function,
return str.length();
Code to find Length of the string using Inbuilt Function in C++
Run
#include <bits/stdc++.h>
using namespace std;

//Function to calculate the length of the string
int Len(string str) 
{  
   return str.length();
}

/* Driver code */
int main()
{
   string str = "PrepInsta";
   cout << Len(str);
   return 0;
}
Output :

9
