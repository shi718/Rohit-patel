
1 / 2
              ASSIGNMENT NUMBER - 3

Here’s a Python program that finds the index of the first and last occurrence of an element in a single iteration over the array without using extra space.


def find_first_and_last_occurrence(arr, target): first_index = -1 last_index = -1
for i in range(len(arr)):
   if arr[i] == target:
       if first_index == -1:
           first_index = i  # First occurrence
       last_index = i  # Last occurrence (will keep updating)

return first_index, last_index
 
2 / 2
Example usage
arr = [1, 2, 3, 2, 4, 2, 5] target = 2 first, last = find_first_and_last_occurrence(arr, target)
print("First occurrence:", first) print("Last occurrence:", last)
