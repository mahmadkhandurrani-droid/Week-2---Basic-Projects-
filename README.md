# Week-2---Basic-Projects-
This repository contains small Python projects I created as a beginner to practice coding and showcase my skills.

score=0
q1=input("What is 2+2?:")
if q1.strip()=="4":
   score += 1
q2=input("Do you jump?:")
if q2=="Yes":
   score += 1
print(f"Score is {score}/2")

balance=1000
print("Mini Banking System")
print("1.Deposit")
print("2.Withdraw")
print("3.Check Balance")
print("Exit")
choice=input("Enter choice:")
if choice=="1":
   amount=int(input("Amount:"))
   balance += amount
   print(f"New Balance:{balance}")
elif choice=="2":
	  amount=int(input("Amount:"))
	  if amount <= balance:
	  	balance -= amount
	  	print("Money Withdrawn")
	  else:
	 	    print("Insufficent Balance")
elif choice=="3":
	  print(f"Balance :{balance}")
elif choice=="4":
	  print("Thanks for using Mini Bank")
else:
	    print("Invalid option")
      


