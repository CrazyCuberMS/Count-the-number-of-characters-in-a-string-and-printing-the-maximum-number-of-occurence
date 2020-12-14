# Count-the-number-of-characters-in-a-string-and-printing-the-maximum-number-of-occurence


#include <iostream>
#include <string>
using namespace std;

// Function that return count of the given
// character in the string
int count(string s, char c)
{
    // Count variable
    int res = 0;

    for (int i=0;i<s.length();i++)

        // checking character in string
        if (s[i] == c)
            res++;

    return res;
}

// Driver code
int main()
{
    long int a;
    cin >> a;
    string str;
    cin >> str;
    char c = 'c';
    char o = 'o';
    char d = 'd';
    char e = 'e';
    long int p,q,r,s;
    p = count(str, c);
    q = count(str, o);
    r= count(str, d);
    s= count(str, e);
    cout <<( (p<=q ? p : q) <= (r<=s ? r : s) ? (p<=q? p : q) : (r<=s ? r : s)  ) << endl;
    return 0;
}
