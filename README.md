# FLAMES
Project Name: Flames (C++ implementation)  Purpose: To predict the relationship between two people based on the letters in their names.
#include <bits/stdc++.h>
using namespace std;
int main()
{
  int g,j,k=0;
  char s[20],u[20];
  string v,b;
  cout<<"Enter the name first";
  getline(cin, v);
  cout<<"Enter the name second";
  cin>>b;
  for(int i=0;i<v.length();++i)
  {
      
      
      for(j=0;j<b.length();++j)
      {
         if (v[i]==b[j]) 
         
         {  k++;
             v.erase(i,1);
             b.erase(j,1);
             i--;
             j--;
             break;
         }
         
         
      }
  }
  g=v.length()+b.length();
  if(g>5)
  {
      g=g%6;
  }
   cout<<k;
 
 switch(g)
 {
     case 1: cout<<" this is friend";
      break;
     case 2: cout<<"this is love";
     break;
     case 3: cout<<"this is affection";
     break;
     case 4: cout<<" this is marrage";
     break;
     case 5: cout<<"this is sibilings";
     break;
     default:cout<<"Enter the a character" ;
     
 }
  
}

