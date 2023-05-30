class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:

        d = {}
        for i, j in enumerate(nums):
            rem = target - j

            if rem in d : return [d[rem], i]
            d[j] = i
            
        
