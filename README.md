import math
import os
import random
import re
import sys

def miniMaxSum(arr):
    # Calculate the total sum of the array
    total_sum = sum(arr)
    # Calculate the minimum sum (exclude the maximum element)
    min_sum = total_sum - max(arr)
    # Calculate the maximum sum (exclude the minimum element)
    max_sum = total_sum - min(arr)
    # Print the results
    print(min_sum, max_sum)

if __name__ == '__main__':
    arr = list(map(int, input().rstrip().split()))
    miniMaxSum(arr)

