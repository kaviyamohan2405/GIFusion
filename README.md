1. # SORTING ARRAY BY INCREASING FREQUENCY

## Explanation:
1.**Counting Frequencies:** The Counter class from the collections module is used to count the frequency of each number in the array.

2.**Sorting the Array:** The sort method is used with a custom key:

3.**key=lambda x: (freq[x], -x):** This sorts the elements first by their frequency (freq[x]) in ascending order.
                  If two elements have the same frequency, they are sorted by their value in descending order (-x).

4.**Returning the Result:** The sorted array is returned directly.


2. # REVERSE INTEGER

## Explanation:

1.**Class Definition:** We define a class Solution with a method reverse which takes an integer x as input and returns an integer.

2.**Handling the 32-bit Limits:** We define INT_MIN and INT_MAX to represent the minimum and maximum values of a 32-bit signed integer.

3.**Sign and Absolute Value:** We determine the sign of x and work with its absolute value for the reversal process.

4.**Reversal Logic:** Inside a loop, we pop the last digit of x and append it to result. Before updating result, we check if the new value would overflow. If it would, we return 0 immediately.

5.**Return Result with Sign:** Finally, we return result multiplied by the original sign to ensure the correct sign of the reversed integer.
