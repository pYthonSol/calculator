# calculator
This is an exponent calculator
def add(x, y):
   return x + y
def subtract(x, y):
    return x -  y
def multiply(x, y):
    return x * y
def divide(x, y):
    return x / y
def exponent(x, y):
    return x**y
print("Select Operation.")
print("Add")
print("Subtract")
print("Multiply")
print("Divide")
print("Multiply by an Exponent")

while True:
    choice = input("Enter a Choice:(1/2/3/4/5): ")
    if choice in ('1', '2', '3', '4', '5'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))


        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))
        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))
        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))
        elif choice == '4':
            print(num1, "/", num2, "=", divide(num1, num2))
        elif choice == '5':
            print(num1, "**", num2, "=", exponent(num1, num2))

            next_calculation = input("do you want to do another calculation? (yes/no): ")
            if next_calculation == "no":
                break
        else:
            print("invalid input")





