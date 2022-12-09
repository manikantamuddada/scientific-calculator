import math

print("***This Scientific Calculator***")
print("Press:   1 for Arithmetic Operations  2 for Square root  3 for Exponent  4 for Trigonometric Function  5 for Degree to Radian  6 for Radian to Degree")
optn = int(input("\nEnter the Number: "))

if optn>0 and optn<=6:
    if optn == 1:
        print("\n__ Arithmetic Operations __")
        
        print("\nOperation Between Two Numbers\n")

        num1 = eval(input("Enter first number: "))
        num2 = eval(input("Enter second number: "))
        operation = input("Enter the Operator: ")
        if operation == "+":
            print("The Addition of {} and {} is {}".format(num1,num2,num1+num2))
        elif operation == "-":
            print("The Substraction of {} and {} is {}".format(num1,num2,num1-num2))
        elif operation == "x" or "*":
            print("The Multiplication of {} and {} is {}".format(num1,num2,num1*num2))
        elif operation == "/":
            print("The Division of {} and {} is {}".format(num1,num2,num1/num2))
        elif operation == "%":
            print("The Modulus of {} and {} is {}".format(num1,num2,num1%num2))
        else:
            print("Invalid Input")
    elif optn == 2:
        print("    ___This is to find Squareroot___")
        root = eval(input("Enter the Number: "))
        print("The Square root of",root,"is","{:.2f}".format(math.sqrt(root)))

    elif optn == 3:
        print("   ___This is to find Exponent___")
        num = int(input("Enter the Number: "))
        pwr = int(input("Enter the Power: "))
        print("The Power {} of {} is {}".format(pwr,num,num**pwr))

    elif optn == 4:
        print("  ___This is to find Trigonometric Function___")
        print("Press: 1 for Cose 2 for Sine 3 for Tangent")
        func = int(input("Enter the Number: "))
        if func == 1:
            value = int(input("Enter: "))
            print("The Sine of {} is {}".format(value,math.sin(value)))
        elif func == 2:
            value = int(input("Enter: "))
            print("The Sine of {} is {}".format(value,math.cos(value)))
        elif func == 3:
            value = int(input("Enter: "))
            print("The Sine of {} is {}".format(value,math.tan(value)))
        else:
            print("x__  Enter value has not alloted to any function   __x")
    elif optn == 5:
        print("___ Degree to Radian ___")
        degree = int(input("Enter Degree: "))
        print("The Radian of {} is {}".format(degree,math.radians(degree)))
    elif optn == 6:
        print("___ Radian to Degree ___")
        Radian = int(input("Enter Radian: "))
        print("The Radian of {} is {}".format(Radian,math.degrees(Radian)))
        

else:
    print("x__   Entered Value is has not alloted to any function  __x")

