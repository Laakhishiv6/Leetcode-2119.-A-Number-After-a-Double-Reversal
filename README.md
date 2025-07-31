# Leetcode-2119.-A-Number-After-a-Double-Reversal
# Description
Reversing an integer means to reverse all its digits.

For example, reversing 2021 gives 1202. Reversing 12300 gives 321 as the leading zeros are not retained.
Given an integer num, reverse num to get reversed1, then reverse reversed1 to get reversed2. Return true if reversed2 equals num. Otherwise return false.
# Solution
The following question :

if the number is 0 its reverse will be 0 , hence this is the base case and the answer will be true.

If the number if 1800 , its reverse will be 81 and again if we reverse it wont be the same it will be 18 . So what we can infer from this example is that if the numbers end with 0 its reverse reverse wont be the same.
Hence if the number is divisible by 10 simply return false.

Else for all the numbers double reverse will give the same number .

# Algorithm
1. The base case is if the number is 0 , return True.
2. If the number is divisible by 10 then return false.
3. Else return True.
# Code
class Solution:

    def isSameAfterReversals(self, num: int) -> bool:
        if num==0:
            return True
        elif num%10==0:
            return False
        else:
            return True
 # Time complexity
 All the if else statments take constant time 

 Hence time complexity : O(1)
