# Loop
Using loops 

#While:
count = 0

if count < 5:
  print "Hello, I am an if statement and count is", count
#will meet condition if it is true


while count < 5:
  print "Hello, I am a while and count is", count
  count += 1
  #will continue to loop until it reaches condition. 


#Excercise, make count to 9, can either be set to <10 or <=9


while count <= 9:
  print "Hello, I am a while and count is", count
  count += 1
  #will print "" statement 9 times with the count included.
  #-------------#
  
#Condition:


loop_condition = True

while loop_condition:
  print "I am a loop"
  loop_condition = False

#The loop_condition is set to true, when it is it will it print statement, it is not the second time, so process terminates.



num = 1

while num <= 10:   # Fill in the condition
  # Print num squared
  print num**2
  # Increment num (make sure to do this!) #This will limit the number of times the code will loop 
  num += 1
  
  
  #1.
Fill in the loop condition so the user will be prompted for a choice over and over while choice does not equal 'y' and choice does not equal 'n'.

  choice = raw_input('Enjoying the course? (y/n)')

while ________:  # Fill in the condition (before the colon)
  choice = raw_input("Sorry, I didn't catch that. Enter again: ")

  
  
  choice = raw_input('Enjoying the course? (y/n)')

while choice != "y" and choice != "n" :  # Fill in the condition (before the colon)   #!= mean does not equal 
  choice = raw_input("Sorry, I didn't catch that. Enter again: ")

  

