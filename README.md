#include <iostream>
using namespace std;
int main(){

    char text[100];
    cout << "Enter your sentence:";
    cin.getline(text,100);
    for(int i=0; text[i]!='\0';i++){
    char ch = text[i];
        if(ch >= 'A'&& ch<='Z')
            cout<<(ch-'A'+1)<<"";
        else if(ch >='a'&& ch<= 'z')
            cout<<(ch-'a'+1)<<"";
        else if(ch==' ')
            cout<<"27";
        else if(ch==',')
            cout<<"28";
        else if(ch=='.')
            cout<<"29";
        else if(ch=='?')
            cout<<"30";
        else
            cout<<"unknown input";
    }
    return 0;
}
