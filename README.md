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



def factorial(x):
  total = 1 
  while x > 0:
    total *= x
    x -= 1
  return total 

print factorial (5)    








# 5. is_prime

A prime number is a positive integer greater than 1 that has no positive divisors other than 1 and itself. (That’s a mouthful!)

In other words, if you want to test if a number in a variable x is prime, then no other number should go into x evenly besides 1 and x. So 2 and 5 and 11 are all prime, but 4 and 18 and 21 are not.

If there is a number between 1 and x that goes in evenly, then x is not prime.



def is_prime(x):
    if x < 2:
        return False
    else:
        for n in range(2, x-1):
            if x % n == 0:
                return False
        return True

print is_prime(13)
print is_prime(10)




# 6. Reverse:
Define a function called reverse that takes a string textand returns that string in reverse. For example: reverse("abcd") should return "dcba".

You may not use reversed or [::-1] to help you with this.

You may get a string containing special characters (for example, !, @, or #).


def reverse (text):
    word = ""
    l = len(text) - 1
    while l >= 0:
       word = word + text[l]
       l -= 1
    return word 



# 7. Anti- Vowel:

# Excercise:
# 1.Define a function called anti_vowel that takes one string, text, as input and returns the text with all of the vowels removed.

For example: anti_vowel("Hey You!") should return "Hy Y!". Don’t count Y as a vowel. Make sure to remove lowercase and uppercase vowels.


def anti_vowel(text):
    result = ""
    vowels = "ieaouIEAOU"
    for char in text:
          if char not in vowels:
            result += char
    return result
print anti_vowel("hello book")

(My version)

def anit_vowel(text):
  word = ""
  vowels ="aeiouAEIOU"
  for char in text:
     if char not in vowels:
      result += char
  return result
print anti_vowel("The Big Knights") 


# 8. 













