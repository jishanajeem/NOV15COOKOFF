#include<iostream>
using namespace std;
unsigned int gcd(unsigned long m,unsigned long n)
 
{ 
  unsigned long r;
  while(n)
 {
   r=m%n;
   m=n;
   n=r;
 }
 return m;
}
int main()
 {
  long long t,i,a,b,G;
 
  unsigned long num;
   cin>>t;
  for(i=0;i<t;i++)
   {
	cin>>a>>b;
 
	if(a>b)
	{
	  G=gcd(a,b);
	}
	if(G!=1)
	{
 	   num=(a/G);
 	   cout<<"No "<<num;
	}
	else
	{
	  cout<<"Yes";
