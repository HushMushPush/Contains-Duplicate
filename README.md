# Contains-Duplicate
class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
        s = {}
        for i in nums:
            if i not in s.keys():
                s[i] = 1
            else:
                s[i] = s[i] + 1
                return True
        return False

# https://neetcode.io/problems/duplicate-integer/question
