# Experiment 5
## Aim
To learn the execution and use of if statements & switch in c++.

## Software Used
VS Code

## Problem Statements
1. Leap Year Checker: Create a C++ program to determine if a given year is a leap year.
2. Password Validator: Write a C++ program to validate passwords based on specific criteria.
3. Days of the Week Printer: Implement a C++ program that outputs the days of the week based on user input.
4. Simple Calculator: Develop a C++ program that performs basic arithmetic operations.
5. Grade Evaluator: Build a C++ program to evaluate and display grades based on student scores.

## Theory
If Statement: Executes a block of code if a specified condition evaluates to true.

Else Statement: Executes an alternative block of code if the condition in the if statement is false.

Else if Statement: Tests additional conditions if previous conditions are false.

Switch Statement: Executes different blocks of code based on the value of a given expression. It allows for multiple execution paths and is useful when handling various cases based on a variable's value. The switch expression must be of type int or char.

## Example Usage of switch
The switch statement provides a way to handle multiple possible values for a variable. Each case represents a potential value, and the corresponding block of code executes if the switch expression matches that case value.


## Program Codes
1.
```javascript
//Grade Evaluation
#include <iostream>
using namespace std;
int main()
{
  int s;
  cout<< "Enter your score";
  cin>>s;
  if(s>=90)
  {
    cout<<"Your grade is A"<<endl;
    cout<< "You are passed"<<endl;
  }
  else if(s>=80)
  {
    cout<<"Your grade is B"<<endl;
    cout<< "You are passed"<<endl;
  }
  else if(s>=70)
  {
    cout<<"Your grade is C"<<endl;
    cout<< "You are passed"<<endl;
  }
  else if(s>=60)
  {
    cout<<"Your grade is D"<<endl;
    cout<< "You are passed"<<endl;
  }
  else if( s>=50)
  {
    cout<<"Your grade is E"<<endl;
    cout<< "You are passed"<<endl;
  }
  else
  { cout<< "Failed";
  }
  return 0;
}
```
2.
```
//Leap Year
#include<iostream>
using namespace std;
int main()
{
    int year;
    cout<<"enter a year"<<endl;
    cin>>year;
    if(cin.fail())
    {
        cout<<"invalid input";
    }
    else 
    {
        if((year%4==0 && year%100!=0) || (year%400==0))
        {
        cout<<year<<" is a leap year";
        }
        else 
        {
        cout<<year<<" is not a leap year";
        }
    }
    return 0;
}
```
3.
```
//Password Validation
#include<iostream>
using namespace std;
int main()
{
   string password;
   cout << "Enter the password: ";
   cin >> password;
   if (password == "secret")
   {
    cout << "Access Granted ";
   }
   else
   { 
    cout<< "Access Denied";
   }
   return 0;
}
```
4.
```
//Calculator
#include<iostream>
using namespace std;
int main()
{
    float a,b,c ;

    int choice;
    cout << "Calculator"<<endl;
    cout << "1: Addition"<<endl;
    cout << "2: Subtraction"<<endl;
    cout << "3: Multiplication"<<endl;
    cout << "4: Division"<<endl;
    cout<<"Enter operation choice: ";
    cin>>choice;
switch(choice)
{
    case 1 :
    { float c;
    cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a+b;
    cout<<"sum is = "<<c;
    } 
    break;
    case 2 :
    {
        float c;
    cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a-b;
    cout<<"difference is = "<<c;
    }
    break;
case 3 :
{ float c;
    cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a*b;
    cout<<"product is = "<<c;
}
break;
case 4 :

{ float c;
   cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a/b;
    cout<<"quotient is = "<<c;
    }
    break ;
}
return 0;
}
```
5.
```
//Days of Week
#include<iostream>
using namespace std;
int main()
{
    int a,b,c, choice ;
    cout << "DAY"<<endl;
    cout << "1: Monday"<<endl;
    cout << "2: Tuesday"<<endl;
    cout << "3: Wednesday"<<endl;
    cout << "4: Thursday"<<endl;
    cout << "5: Friday"<<endl;
    cout << "6: Saturday"<<endl;
    cout << "7: Sunday"<<endl;
    cout<<"Enter of day: ";
    cin>>choice;
switch(choice)
{
{ case 1 :
cout<< "Day is Monday";
}
break ;
{ case 2 :
cout<< "Day is Tuesday";
}
break ;
{ case 3 :
cout<< "Day is Wednesday";
}
break ;{ case 4 :
cout<< "Day is Thursday";
}
break ;
{ case 5 :
cout<< "Day is Friday";
}
break ;
{
 case 6 :
cout<< "Day is Saturday";
}
break ;
{ case 7 :
cout<< "Day is Sunday";
}
}
}
```

## Output:











    
