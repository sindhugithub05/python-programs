# python-programs
# Python program for simple calculator

# Function to add two numbers
def add(num1, num2):
	return num1 + num2

# Function to subtract two numbers
def subtract(num1, num2):
	return num1 - num2

# Function to multiply two numbers
def multiply(num1, num2):
	return num1 * num2

# Function to divide two numbers
def divide(num1, num2):
	return num1 / num2
 
# Function to do float division of two numbers
def floatdivision(num1,num2):
    return num1%num2

print("Please select operation -\n" \
		"1. Add\n" \
		"2. Subtract\n" \
		"3. Multiply\n" \
		"4. Divide\n"\
		"5.Float Division\n")


# Take input from the user
select = int(input("Select operations form 1, 2, 3, 4,5 :"))

number_1 = int(input("Enter first number: "))
number_2 = int(input("Enter second number: "))

if select == 1:
	print(number_1, "+", number_2, "=",
					add(number_1, number_2))

elif select == 2:
	print(number_1, "-", number_2, "=",
					subtract(number_1, number_2))

elif select == 3:
	print(number_1, "*", number_2, "=",
					multiply(number_1, number_2))

elif select == 4:
	print(number_1, "/", number_2, "=",
					divide(number_1, number_2))
elif select==5:
	print(number_1,"%",number_2,"=",floatdivision(number_1,number_2))
else:
    print(" invalid input")
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# profit and loss code
a=int(input("Enter the cost price\n"))
b=int(input("Enter the selling price\n"))
if(b>a):
    x=((b-a)/a)*100
    print(f"Profit {x:.1f}")
elif(b<a):
    y=((a-b)/a)*100
    print(f"Loss {y:.1f}")
else:
    print(f"No Profit No Loss")
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# luggage chech in code
weight=int(input("Enter the weight of luggage\n" ))
w=weight-15
if weight<=0:
    print("Invalid Input")
    exit()
if(w<=30 and w>0):
    pay=w*50
    print(f"Need to pay extra amount of Rs.{pay}")
elif(w>30 and w<=60):
    pay=w*150
    print(f"Need to pay extra amount of Rs.{pay}")
elif(w>60):
    pay=w*250
    print(f"Need to pay extra amount of Rs.{pay}")
else:
    print(f"No need to pay extra amount")
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# check no of seats available code 
a=int(input("Enter the number of students in the class\n" ))
b=int(input("Enter number of rows\n"))
c=int(input("Enter the number of students can sit in each row\n"))
d=c*b
e=a-d
if(d<a):
    print(f"{e} has to attend lecture standing")
else:
       print("Everyone can sit")
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# default function code
def greet(name,message="Welcome to Python Programming"):
    print(f"Hello {name}, {message}")
def main():
    print("Menu")
    print("1.Name and Message")
    print("2.Name")
    choice=input("")
    
    if choice=="1":
        name=input("Enter the name\n")
        message=input("Enter the message\n")
        greet(name,message)
    elif choice=="2":
       name=input("Enter the name")
       greet(name)
    else:
        print("Invalid choice")

if __name__=="__main__":
    main()
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# multiplication of two numbers using functions
def multiply(arg1,arg2=10):
    return arg1*arg2
a=int(input())
b=int(input())
result1=multiply(a)
result2=multiply(a,b)
result3=multiply(a,arg2=9)
print(f"The result is {result1}")
print(f"The result is {result2}")
print(f"The result is {result3}")
