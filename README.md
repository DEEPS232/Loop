choice = raw_input('Enjoying the course? (y/n)')

while choice != "y" and choice != "n":  # Fill in the condition (before the colon)
  choice = raw_input("Sorry, I didn't catch that. Enter again: ")

if choice == "n":
  print "We're sorry to hear that."
else:
  if choice == "y":
    print "I know right, this coding stuff ain't half bad!"
