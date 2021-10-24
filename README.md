# Lecture-9
While loop 

    #include <iostream>
    using namespace std;

    int main() {
        int count = 1;
        while (count <= 1000) {
            cout << count << endl;
            count++;
        }
    }
Do While loop

    #include <iostream>
    #include <string>
    using namespace std;

    int main()
    {
        string password = "1234password";
        string userInput;
        do {
            cout << "Enter your Password" << endl;
            cin >> userInput;
        } while (password != userInput);
        cout << "Welcome to the super secure banking area" << endl;
    }
 Login Alter

    #include <iostream>
    #include <string>
    using namespace std;

    //Login Alternative 
    int main()
    {
        string password = "1234password";
        string userInput;

        cout << "Enter your password" << endl;
        cin >> userInput;

        while (password != userInput) {
            cout << "Enter your password" << endl;
            cin >> userInput;
        }
        cout << "Welcome to the super secure banking area" << endl;
    }

Remain Positive

    #include <iostream>
    using namespace std;

    int main() {

        float mynum = 20;

        while (mynum > 0) {
            cout << mynum << endl;
            mynum -= 0.5;
        }

        return 0;
    }
 Age
    
    #include <iostream>
    using namespace std; 

    int main()
    {
        cout << "Enter your age" << endl; 
        int age;
        cin >> age;

        while (cin.fail()) {
            cout << "Invalid input.\nPlease enter a valid age" << endl;
            cin.clear();
            cin.ignore(1000, '\n');
            cin >> age;
        }
        cout << "your age is:" << age;
    }
  Break Example
  
      #include <iostream>
    using namespace std;

    int main()
    {
        cout << "Enter a whole number: " <<
            endl; int userNum;
        cin >> userNum;

        int count = 1;
        while (true) {
            cout << count << endl;
            if (count == userNum) {
                break;
            }
            count++;
        }
    }
Break Alter

    #include <iostream>
    using namespace std;

    int main()
    {
        cout << "Enter a whole number: " << endl;
        int userNum;
        cin >> userNum;

        int count = 1;
        while (count <= userNum) {
            cout << count << endl;
            count++;
        }

    }

    
