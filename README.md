# Write-a-Python-program-to-find-the-highest-3-values-in-a-dictionary

import heapq
my_dict = {'a': 20, 'b': 10, 'c': 50, 'd': 40, 'e': 30}
# Find the top 3 values in the dictionary
top_3_values = heapq.nlargest(3, my_dict.values())
# Find the keys corresponding to the top 3 values
top_3_keys = [key for key, value in my_dict.items() if value in top_3_values]
# Print the result
print(f"The top 3 values in the dictionary are: {', '.join(str(val) for val in top_3_values)}")
print(f"The keys corresponding to the top 3 values are: {', '.join(top_3_keys)}")
