from typing import List


class Solution:
    def removeElement(self, nums: List[int], val: int) -> int:
        self.val = val
        
        for i in nums:
            if i == val:
                nums.remove(i)

        return len(nums)

r1 = Solution()

print(r1.removeElement([0,1,2,2,3,0,4,2]), 2)



#ERROR Traceback (most recent call last):
#  File "C:/Users/CrazyPants/PycharmProjects/DummiesProject/pages/views.py", line 15, in <module>
#    print(r1.removeElement([0,1,2,2,3,0,4,2]))
#TypeError: removeElement() missing 1 required positional argument: 'val'
