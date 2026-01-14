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
total=0
m1=int(input("Enter marks of first subject:"))
m2=int(input("Enter marks of second subject:"))
m3=int(input("Enter marks of third subject:"))
total=m1+m2+m3
percentage=(total/300)*100
print(f"Total : {total}")
print(f"Percentage: {percentage}")

tasks=[]
while True:
	print("1.Add")
	print("2.View")
	print("3.Remove")
	print("4.Exit")
	choice=input("Enter choice:")
	if choice=="1":
		task=input("Enter tasks:")
		tasks.append(task)
		print("Added")
	elif choice=="2":
		  
		  if not tasks:
		  	print("No tasks")
		  else:
		  	    for i,task in enumerate(tasks,1):
		  	    	print(f"{i}.{task}")
	elif choice=="3":
		  num=int(input("Number to be remove:"))
		  if 1 <= num <= len(tasks):
		       tasks.pop(num-1)
		       print("Removed")
		  else:
		 	     print("No tasks to remove")
	elif choice=="4":
	       print("Complete your tasks")
	       break
	else:
	         print("Invalid option")

while True:
    print("\n--- Main Menu ---")
    print("1. Quiz")
    print("2. Banking")
    print("3. Marks Calculator")
    print("4. Task Manager")
    print("5. Exit")

    choice = input("Choose an option: ")

    if choice == "1":
        import quiz
        quiz.run()  # assuming you define a run() function in quiz.py

    elif choice == "2":
        import mini_banking
        mini_banking.run()

    elif choice == "3":
        import marks_calculator
        marks_calculator.run()

    elif choice == "4":
        import task_manager
        task_manager.run()

    elif choice == "5":
        print("Exiting program")
        break

    else:
        print("Invalid option")
      


