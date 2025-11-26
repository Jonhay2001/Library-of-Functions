# Library-of-Functions
Returns the sum of two numbers and gives sum as greater than or less than
# Library of functions
# Name: Jonathan Haynes
# Date: 11/25/2025
# Description: Program that demonstrates calling functions,
# returning values, and passing parameters.
# -------------------------------------------------------------

# Function One – prints Student ID
def functionOne():
    print("My Student ID is jonhay2001")   

# Function Two – asks user for 2 numbers, prints sum, returns sum
def functionTwo():
    n1 = float(input("Enter the first number: "))
    n2 = float(input("Enter the second number: "))
    total = n1 + n2
    print(f"The sum of {n1} and {n2} is {total}")
    return total


# Function Three – accepts the sum, prints result, returns numeric part of ID
def functionThree(theSum):
    if theSum > 5:
        print("The sum is greater than 5.")
    else:
        print("The sum is 5 or less.")

    # Return numeric portion of the student ID
    return 1234   # <-- Replace with numeric part of your Student ID


# -------------------------------------------------------------
# main function
# -------------------------------------------------------------
def main():
    functionOne()                     # Calls functionOne() to print Student ID
    sumResult = functionTwo()         # Calls functionTwo(), stores its return value
    studentNumber = functionThree(sumResult)  # Passes the sum to functionThree()
    print(f"functionThree returned the value of {studentNumber}") 
    # Prints the numeric part returned from functionThree()


# Call main
main()
