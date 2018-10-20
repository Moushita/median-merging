# median-merging
A code that finds the median of two arrays after merging them
#include<iostream.h>
#include<constream.h>
void main()
{
int n,m,mid,mid1;
int a[50],b[50];
float med;
cout<<"Enter n";
cin>>n;
m=(2*n);
cout<<"Enter array a";
for(int i=0;i<n;i++)
{
cin>>a[i];
}
for(int j=0;j<n;j++)
{
cin>>b[j];
}
for(int k=0;k<n;k++)
{
cout<<a[k];
}
for(int l=0;l<n;l++)
{
cout<<b[l];
}
for(int g=n;;g<=m;g++)
{
b[g]=a[g-n];
}
if(m%2==0)
{
mid=m/2;
cout<<"Median= "<<b[mid];
}
else
{
mid=n/2;
mid1=((n+1)/2);
med=((b[mid]+b[mid1])/2);
cout<<"Median"<<med;
}
getch();
}

