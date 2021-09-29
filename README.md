# 1.

All right! Let’s get started.

Remember how an even number is a number that is divisible by 2?
Instructions

# Exercise:
Define a function is_even that will take a number x as input.

If x is even, then return True.

Otherwise, return False.




def if_even(x):
  if x % 2 == 0:
    return True
  else:
     return False

print if_even(4)
print if_even(5) 

# --------------------------- #

# 2. is_int

An integer is just a number without a decimal part (for instance, -17, 0, and 42 are all integers, but 98.6 is not).

For the purpose of this lesson, we’ll also say that a number with a decimal part that is all 0s is also an integer, such as 7.0.

This means that, for this lesson, you can’t just test the input to see if it’s of type int.

If the difference between a number and that same number rounded is greater than zero, what does that say about that particular number?


# Exercise:
Define a function is_int that takes a number x as an input.

Have it return True if the number is an integer (as defined above) and False otherwise.

For example:
is_int(7.0) # True
is_int(7.5)  # False
is_int(-1) # True

def is_int(x):
  absolute = abs(x)
  rounded = round(absolute)
  return absolute - rounded == 0 

print is_int(15)
print is_int(7.5)
print is_int (0)
 

# -----------# 

# 3. digit_sum

Awesome! Now let’s try something a little trickier. Try summing the digits of a number.

# Excercise:
Write a function called digit_sum that takes a positive integer n as input and returns the sum of all that number’s digits. For example: digit_sum(1234) should return 10 which is 1 + 2 + 3 + 4. (Assume that the number you are given will always be positive.)

Check the hint if you need help!


def digit_sum(n):
  total = 0 
  string_n = str(n)
  for char in string_n:
   total += int(char)
  return total 


def digit_sum(n):
  total = 0
  while n > 0:
    total += n % 10
    n = n // 10
  return total 

# --------------- #


# 4. Factorial 
 
 # All right! Now we’re cooking. Let’s try a factorial problem.

To calculate the factorial of a non-negative integer x, just multiply all the integers from 1 through x. For example:

    - factorial(4) would equal 4 * 3 * 2 * 1, which is 24.
    - factorial(1) would equal 1.
    - factorial(3) would equal 3 * 2 * 1, which is 6.













