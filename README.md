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
