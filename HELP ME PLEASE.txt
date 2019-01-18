#include <stdio.h>
#include <iostream>
using namespace std;
class troad 
{
public:
int Width;
float Length;
troad();
troad(float Length0,int Width0);
};
troad:: troad()
{
Length=50.1;
Width=4;
}
troad:: troad(float Length0,int Width0)
{
if (Length0>0)
Length = Length0;
else Length = 1;
if (Width0>0)
Width = Width0;
else Width = 1;
}
int main()
{
troad road;
std::cout<<"road.Width = "<< road.Width<<"\nroad.Length = "<<road.Length<<std::endl;
troad road1 (50.1,4);
std::cout<<"road.Width = "<< road1.Width<<"\nroad.Length = "<<road1.Length<<std::endl;
return 0;
}