Write C++ code to accomplish the following tasks.
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.

#include <iostream>
#include <string>
using namespace std;
int main() {
int nums[]={2,3,4};
int target=5;
for (int i = 0; i < sizeof(nums); i++)
 {
for (int j = i + 1; j < sizeof(nums); j++) 
{
if (nums[j] == target - nums[i])
 {
cout <<"["<<i<<","<<j<<"]";
}
}
}
}
