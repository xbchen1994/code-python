### 1. Two Sum

Given an array of integers, return indices of the two numbers such that they add up to a specific target.
You may assume that each input would have exactly one solution.

```
class Solution(object):
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        i = 0;
        a = { };
        length = len(nums);
        for i in range(length):
            if (target-nums[i]) in a:
                return [a[target-nums[i]],i];
            a[nums[i]] = i;
```
