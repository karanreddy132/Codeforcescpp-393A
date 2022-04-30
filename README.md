# Codeforcescpp-393A
#include<bits/stdc++.h>
using namespace std;

int main(){
  string s;
  cin >> s;
  int arr[5] = {0};
  for(int i=0;i<s.size();i++){
    if(s[i]=='n')
      arr[0]++;
    else if(s[i]=='i')
      arr[1]++;
    else if(s[i]=='e')
      arr[2]++;
    else if(s[i]=='t')
      arr[3]++;
  }
  if(arr[0]<=3)
    cout << min(arr[0]/3,min(arr[1],min(arr[2]/3,arr[3])));
  else
    cout << min((arr[0]-1)/2,min(arr[1],min(arr[2]/3,arr[3])));
  return 0;
}
