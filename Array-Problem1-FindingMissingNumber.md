## Problem : Finding Missing number in array
- Solution : We can use a simple math formula to solve this => N=N*(N+1)//2
- Problem Link : https://leetcode.com/problems/missing-number/
```Python 
class Solution(object):
    def missingNumber(self, nums):
        n = len(nums)
        expectedsum=n*(n+1)//2
        actualsum = sum(nums)
        missingnumber=expectedsum-actualsum
        return missingnumber
```
