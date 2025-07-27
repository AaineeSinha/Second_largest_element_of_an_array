# Second_largest_element_of_an_array
To find the second largest element of an array
class Solution:
    def getSecondLargest(self, arr):
        first = second = -1
        for num in arr:
            if num > first:
                second = first
                first = num
            elif num > second and num != first:
                second = num
        return second
