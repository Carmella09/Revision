# Revision

EXERCISE 

Write a code 10 min
Write a code that asks the user to input 5 subject marks (0-100) and
Calculates the sum and average 

    #include<iostream>
    #include<string>
    using namespace std;
    int main()
    {
        cout << "Enter 5 of your Grade (between 0 - 100): " << endl;

        cout << "First: ";
        double grade1;
        cin >> grade1;

        cout << "Second: ";
        double grade2;
        cin >> grade2;

        cout << "Third: ";
        double grade3;
        cin >> grade3;

        cout << "Fourth: ";
        double grade4;
        cin >> grade4;

        cout << "Fifth: ";
        double grade5;
        cin >> grade5;

        double x,d;
        x = grade1 + grade2 + grade3 + grade4 + grade5;
        d = x / 5;

        cout << x << " is the sum of your grade. \n";
        cout << d << " is your average grade. ";

    }
  
Rewrite a code 15 min
Write the code that asks the user to input 5 subject marks (0-100) and
Calculates the sum and average making sure that program handles the fail
command
  
    #include<iostream>
    #include<string>
    using namespace std;
    int main()
    {
        cout << "Enter 5 of your Grade (between 0 - 100): " << endl;

        double grade1, grade2, grade3, grade4, grade5;
        double x, d;

        cin >> grade1;
        cin >> grade2;
        cin >> grade3;
        cin >> grade4;
        cin >> grade5;

        if (!cin.fail())
        {
            grade1 >= 100 && grade2 >= 100 && grade3 >= 100 && grade4 >= 100 && grade5 >= 100;

            x = grade1 + grade2 + grade3 + grade4 + grade5;
            d = x / 5;

            cout << x << " is the sum of your grade. \n";
            cout << d << " is your average grade. ";
        }
        else if (cin.fail())
        {
            cin.clear();
            cin.ignore(1000, '\n');
            cout << "Invalid output" << endl;
        }
    }
  

  
Write a code 15min

Write a code that asks the user their age (>=10), and
according to that give them a message.

Age 10-12: preteen age

Age 13-19: teen-age

Age 20-29: twenties

Age 30-39: thirties

Age 40-49: forties

Age 50-59: fifties

Age 60 or above: sixties or above

Make sure that the age is from 10, age before that should
not be accepted

The code should be able to handle the incorrect input
  
      #include<iostream>
    using namespace std;
    int main()
    {
      int age;
      cout << "Age please (not below 10): " << endl;
      cin >> age;

       if (age < 10)
      {
      cout << "What? Please try again" << endl;
      }
      else if (age >= 10 && age <= 12)
      {
        cout << age <<" is Preteen age" << endl;
      }
      else if (age >= 13 && age <= 19)
      {
        cout << age << " is teen-age" << endl;
      }
      else if (age >= 20 && age <= 29)
      {
        cout << age << " is twenties" << endl;
      }
      else if (age >= 30 && age <= 39)
      {
        cout << age << " is thirties" << endl;
      }
      else if (age >= 40 && age <= 49)
      {
        cout << age << " is fourthies" << endl;
      }
      else if (age >= 50 && age <= 59)
      {
        cout << age << " is fifthies" << endl;
      }
      else if (age >= 60)
      {
        cout << age << " is sixties or above" << endl;
      }
      else
       {
         cout << "Invalid Output" << endl;
       }
    }

  
  
  
  
