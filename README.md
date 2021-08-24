# codechef-august-cook-off
 EQDIFFER 
#include <bits/stdc++.h>
using namespace std;

int main() {
	int t;
	cin>>t;      
	while(t--){
	    long long n; cin>>n; int a[n];
	    for (int i=0;i<n; i++)  { 
	        cin>>a[i];}
	        unordered_map<long long, long long>mp; 
	        for(int i=0; i<n;i++) { 
	            mp[a[i]]++;
	        
	       
	        } 
	       
	       long long maxi=0;
	       for(auto i:mp){
	           maxi=max(maxi,i.second); 
	       }  
	       if(n<=2)  cout<<0<<endl;
	       else if (maxi==1) {  cout<<n-2<<endl;} 
	       else{   cout<< n- maxi <<endl ;  } 
	}  

}

WHICHDIV
#include <iostream>
using namespace std;

int main() {
	int t; cin>>t;  
	while(t--)
	{long long r;
	    cin>>r; 
	    if(r>=2000) 
	    cout<<1<<endl; 
	    else if (r<2000 and r>=1600)
	    cout<<2<<endl; 
	    else if (r<1600) 
	    cout<<3<<endl;
	}
	
	return 0;
}
