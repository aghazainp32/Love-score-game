# Love-score-game

#You are going to write a program that tests the compatibility between two people.

#To work out the love score between two people:

#Take both people's names and check for the number of times the letters in the word TRUE occurs. Then check for the number of times the letters in the word LOVE occurs. Then combine these numbers to make a 2 digit number.

#For Love Scores less than 10 or greater than 90, the message should be:

#"Your score is **x**, you go together like coke and mentos."

#For Love Scores between 40 and 50, the message should be:

#"Your score is **y**, you are alright together."

#Otherwise, the message will just be their score. e.g.:

#"Your score is **z**."
 
 #START PROGRAM
 
print("Welcome to the Love Calculator!")
name1 = input("What is your name? \n")
name2 = input("What is their name? \n")
lover_name=name1+name2
lower_case=lover_name.lower()
t=lower_case.count("t")
r=lower_case.count("r")
u=lower_case.count("u")
e=lower_case.count("e")
true=t+r+u+e

l=lower_case.count("l")
o=lower_case.count("o")
v=lower_case.count("v")
e=lower_case.count("e")
love=l+o+v+e

lover_score=int(str(true)+str(love))
if (lover_score<10) or (lover_score>90):
  print(f"Your score is {lover_score}, you go together like coke and mentos.")
elif (lover_score>40) or (lover_score<50):
  print(f"Your score is {lover_score}, you are alright together.")
else:
  print(f"Your score is {lover_score}.")
