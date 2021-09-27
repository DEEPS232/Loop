# Looping over a dictionary

# You may be wondering how looping over a dictionary would work. Would you get the key or the value?

# The short answer is: you get the key which you can use to get the value: 

  d = { 'x': 9, 'y': 10, 'z':20}
  for key in d:
    if d[key] == 10:
     print "This dictionary has the value of 10!"
 

# 1. First, we create a dictionary with strings as the keys and numbers as the values. 
# 2. Then, we iterate through the dictionary, each time storing the key in key.
# 3 .Next, we check if that key’s value is equal to 10.
# 4. If so, we print "This dictionary has the value 10!"

     
     
 # Excersie:
 
 
 d = {'a': 'apple', 'b': 'berry', 'c': 'cherry'}

for key in d:
  # Your code here!
  print key, d[key]
  
  # prints the following:
  
  a apple 
  c cherry 
  b berry 
