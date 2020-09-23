<div align="center">

## User Registration


</div>

### Description

Registration
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Michael](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/michael.md)
**Level**          |Beginner
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Registry](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/registry__3-11.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/michael-user-registration__3-2067/archive/master.zip)





### Source Code

```
/*
 * File:  User Registration
 *
 * Author:  Micahel
 *
 * Description: Requests User For Information And Writes Inputed Information Into
 *    A .eml (E-Mail) File.
 *
 *
 * This File Is Available For Free Distrobution. Please Report Bugs To: Warped46@home.com
 *
 */
#include <iostream.h>
#include <stdio.h>
#include <conio.h>
#include <windows.h>
#include <tcconio.c>
#include <tcconio.h>
#include <time.h>
#include <string.h>
#include <fstream.h>
char FirstName[20];
char LastName[20];
char Address[20];
char Phone[12];
char Time[3];
char Email[20];
char State[15];
char City[15];
char Info_Check[3];
char ReEnter_Check[3];
char Age[3];
char Zip[4];
std::ofstream tfile;
void start();
void check();
int main(int argc, char *argv[])
{
 textcolor(DARKGRAY); cout << "\n\nWelcome To Smart Registration"<<endl;
 cout << "Written By Michael(warped46@home.com)"<<endl;
 cout << "\nPress Enter To Begin...";
 getch();
 start();
}
void start()
 {
 clrscr();
 	time_t ltime;
	time( <ime );
	textcolor(LIGHTBLUE); cout << "\nCurrent Log In Date And Time Is "<<ctime( <ime)<<endl;
 cout << "Is The Time Correct? (y/n): "; textcolor(CYAN);
 gets(Time);
 if ( Time[0] == 'y' || Time[0] == 'Y' )
   {
   clrscr();
   textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
   cout << "1"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your First Name: "; textcolor(CYAN);
   gets(FirstName);
   textcolor(DARKGRAY); cout << "\n\n["; textcolor(WHITE);
   cout << "2"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your Last Name: "; textcolor(CYAN);
   gets(LastName);
   textcolor(DARKGRAY); cout << "\n\n["; textcolor(WHITE);
   cout << "3"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your Home Address: "; textcolor(CYAN);
   gets(Address);
   textcolor(DARKGRAY); cout << "\n\n["; textcolor(WHITE);
   cout << "4"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your Age: "; textcolor(CYAN);
   cin >> Age;
   textcolor(DARKGRAY); cout << "\n\n["; textcolor(WHITE);
   cout << "5"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your Phone Number (With Area Code): "; textcolor(CYAN);
   gets(Phone);
   textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
   cout << "6"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your City: "; textcolor(CYAN);
   gets(City);
   clrscr();
   textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
   cout << "7"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your State: "; textcolor(CYAN);
   gets(State);
   textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
   cout << "8"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your Zip Code: "; textcolor(CYAN);
   gets(Zip);
   textcolor(DARKGRAY); cout << "\n\n["; textcolor(WHITE);
   cout << "9"; textcolor(DARKGRAY);
   cout << "]";
   textcolor(LIGHTBLUE); cout << " Please Enter Your E-Mail Address: "; textcolor(CYAN);
   gets(Email);
   check();
     }
     else
     {
     clrscr();
     textcolor(RED); cout << "\nLog In Error. [Time(1)]"<<endl;
     cout << "Please Try Again And/Or Report This To: warped46@home.com"<<endl;
     cout << "Press 'Enter' To Exit..."<<endl;
     getch();
     }
}
void check()
 {
  clrscr();
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "1"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " First Name:  "; textcolor(CYAN);
  cout << FirstName;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "2"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " Last Name:  "; textcolor(CYAN);
  cout << LastName;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "3"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " Address:  "; textcolor(CYAN);
  cout << Address;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "4"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " Age:   "; textcolor(CYAN);
  cout << Age;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "5"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " Phone Number: "; textcolor(CYAN);
  cout << Phone;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "6"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " City:   "; textcolor(CYAN);
  cout << City;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "7"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " State:   "; textcolor(CYAN);
  cout << State;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "8"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " Zip Code:  "; textcolor(CYAN);
  cout << Zip;
  textcolor(DARKGRAY); cout << "\n["; textcolor(WHITE);
  cout << "9"; textcolor(DARKGRAY);
  cout << "]";
  textcolor(LIGHTBLUE); cout << " E-Mail Address: "; textcolor(CYAN);
  cout << Email;
  textcolor(LIGHTBLUE); cout << "\n\nIs All Of That Information Correct?(y/n): "; textcolor(CYAN);
  gets(Info_Check);
  if ( Info_Check[0] == 'y' || Info_Check[0] == 'Y' )
   {
   clrscr();
   textcolor(LIGHTBLUE); cout << "\nPress Enter To Write .eml File..."<<endl;
   getch();
   cout << "Writing Registration.eml..."<<endl;
   time_t ltime;
   time( <ime );
   tfile.open("Registration.eml");
   tfile << "From: <" << Email << ">"<<endl;
   tfile << "To: warped46@home.com"<<endl;
   tfile << "Subject: Registration (Through Smart Registration)"<<endl;
   tfile << "Date: " << ctime( <ime) <<endl;
   tfile << "First Name: " << FirstName <<endl;
   tfile << "Last Name: " << LastName <<endl;
   tfile << "Address: " << Address <<endl;
   tfile << "Phone: " << Phone <<endl;
   tfile << "Email: " << Email <<endl;
   tfile << "City: " << City <<endl;
   tfile << "Zip Code: " << Zip <<endl;
   tfile << "State: " << State <<endl;
   tfile << "Age: " << Age <<endl;
	  tfile.close();
   clrscr();
   textcolor(LIGHTBLUE); cout << "\nRegistration.eml (E-Mail) Written Successfully..."<<endl;
   cout << "Press Enter To Exit...";
   getch();
   }
   else
    {
    textcolor(LIGHTBLUE); cout << "\n\nWould You Like To Re-Enter Your Information?(y/n)"; textcolor(CYAN);
    gets(ReEnter_Check);
     if ( ReEnter_Check[0] == 'Y' || ReEnter_Check[0] == 'y' )
      {
      textcolor(LIGHTBLUE); cout << "\nRestarting Registration...";
      start();
       }
       else
        {
        clrscr();
        textcolor(RED); cout << "\nRegistration Error [User Fault(2)]"<<endl;
        cout << "Press Enter To Exit...";
        getch();
        }
    }
}
```

