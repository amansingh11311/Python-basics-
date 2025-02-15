#Write a Python program to print "Hello, World!"
print("Hello, World!")
# Write a Python program that displays your name and age
print("Name = Aman kumar")
print("Age= 20")
# Write code to print all the pre-defined keywords in Python using the keyword library
# Get the list of all Python keywords
keywords = keyword.kwlist

# Print the list of keywords
print("Python Keywords:")
for kw in keywords:
    print(kw)

# Write a program that checks if a given word is a Python keyword
import keyword

word = input("Enter a word: ")
print(f"'{word}' is a keyword" if keyword.iskeyword(word) else f"'{word}' is not a keyword")

# Create a list and tuple in Python, and demonstrate how attempting to change an element works differently for each
# List (Mutable)
my_list = [1, 2, 3]
my_list[0] = 5  # Allowed
print(my_list)

# Tuple (Immutable)
my_tuple = (1, 2, 3)
my_tuple[0] = 5

#. Write a function to demonstrate the behavior of mutable and immutable arguments
def modify_values(immutable, mutable):
    immutable += 1  # Creates a new integer object
    mutable.append(4)  # Modifies the existing list

num = 10
lst = [1, 2, 3]

modify_values(num, lst)

print(num)  # Output: 10 (unchanged, immutable)
print(lst)  # Output: [1, 2, 3, 4] (modified, mutable)

# Write a program that performs basic arithmetic operations on two user-input numbers.
a=int(input("enter a="))
b=int(input("enter b="))
print({a+b}, {a-b}, {a*b},{a%b}, {a/b})
# Write a program to demonstrate the use of logical operators.
a, b = True, False

print(a and b)  # False (Both must be True)
print(a or b)   # True (At least one is True)
print(not a)    # False (Negates True to False)

# Write a Python program to convert user input from string to integer, float, and boolean types
user_input = input("Enter a value: ")

int_value = int(user_input)
float_value = float(user_input)
bool_value = bool(user_input)

print({int_value}, {float_value}, {bool_value})

#. Write code to demonstrate type casting with list elements.
# List of string numbers
str_list = ["10", "20", "30.5", "40"]

# Convert to integers (ignoring float values)
int_list = [int(float(num)) for num in str_list]

# Convert to floats
float_list = [float(num) for num in str_list]

# Convert to booleans
bool_list = [bool(num) for num in str_list]

print(f"Original List: {str_list}")
print(f"Integer List: {int_list}")
print(f"Float List: {float_list}")
print(f"Boolean List: {bool_list}")

#. Write a program that checks if a number is positive, negative, or zero.
num = float(input("Enter a number: "))

if num > 0:
    print("Positive")
elif num < 0:
    print("Negative")
else:
    print("Zero")

# Write a for loop to print numbers from 1 to 10
for i in range(1, 11):
    print(i)

#. Write a Python program to find the sum of all even numbers between 1 and 50.
print(sum(range(2, 51,2)))

# Write a program to reverse a string using a while loop
s = input("Enter a string: ")
rev, i = "", len(s) - 1

while i >= 0:
    rev += s[i]
    i -= 1

print(rev)


# Write a Python program to calculate the factorial of a number provided by the user using a while loop
num = int(input("Enter a number: "))
fact, i = 1, num

while i > 1:
    fact *= i
    i -= 1

print("Factorial:", fact)
# Python-basics-
assignment
