Assignment 1:
LeetCode 1. Two Sum

If you don't have an leetcode account yet, please register one from leetcode.com. For
this class, you don't need to pay the membership fee for this leetcode account as all 
the problems covered in our course will be unlocked problems.

This is our first assignment. It will not be graded. If you submit it on time, you can 
get full credit. The due time is June 2, 23: 59.


You can use your favoriate programming language to solve the problem.
Please include:
1. Your student id (using id instead of name to protect your privacy), 
2. Time complexity and space complexity of your code,
3. Add necessary comments on your code.


A sample submission can be here:
```cpp
/*
Studentd id:     0000
Time complexity: O(n^2)
Space complxity: O(1)
*/

class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        const int n = nums.size();
        vector<int> ret;
        for (int i = 0; i < n - 1; ++i)
            for (int j = i + 1; j < n; ++j)
            {
                if (nums[i] + nums[j] == target) 
                {
                    return {i, j};
                }
            }
        return ret;
    }
};
```
