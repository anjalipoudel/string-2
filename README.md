# string-2
#include <iostream>
#include<conio.h>
#include <string.h>
 using namespace std;
 class AddString 
 {
 public:
    char s1[30], s2[30];
    AddString(char str1[], char str2[])
    {
        strcpy(this->s1, str1);
        strcpy(this->s2, str2);
    }
    void operator+()
    {
        cout << "\nConcatenation: " << strcat(s1, s2);
    }
};
int main()
{
    char str1[] = "This program is written by Anjali.";
    char str2[] = "Anjali aka sister.";
    AddString a1(str1, str2);
    +a1;
    return 0;
}
