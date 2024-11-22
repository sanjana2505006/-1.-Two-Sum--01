1.Two Sum - 01
def two_sum(nums, target):
    for i in range(len(nums)):
        for j in range(i + 1, len(nums)):  
            if nums[i] + nums[j] == target:
                return [i,j] 
nums = [2,7,11,15]
target = 9
print(two_sum(nums, target))


#len func is essential when iterating through the list because we need to know how many times the loop should run
straightforward approach known as brute force approach.

Why Both i and j Are Necessary

	1.	Finding Pairs:
	•	You need to check all possible pairs of numbers in the list. For this, i represents the first number, and j represents the second number.
	•	Without j, you can’t examine combinations of two numbers.
