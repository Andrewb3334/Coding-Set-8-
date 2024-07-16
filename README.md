# Coding-Set-8-
Alg Workbench #3

mystring = "abc123def456ghi789"

count_digits = 0 

for char in mystring:
    if char.isdigit():
        count_digits += 1 

print("Number of digits in the string:", count_digits)

Alg Workbench #2

mystring = "Hi, how are you doing today?"

count_spaces = 0 

for char in mystring:
    if char == ' ':
        count_spaces += 1 
print("Number of space characters in the string:", count_spaces)

Programming Exercise #1

def display_initials(full_name):
    names = full_name.split()

    initials = ""


    for name in names:

        initial = name[0].upper()

        initials += initial + ". "

    initials = initials.strip()

    return initials 

full_name = input("Enter your first, middle, and last name: ")

print("Initials: ", display_initials(full_name))


Programming Exercise #2

def sum_of_digits_in_string(input_string):
    total_sum = 0 

    for char in input_string:

        digit = int (char)

        total_sum += digit 

    return total_sum

user_input = input("Enter a series of single-digit numbers with nothing seperating them: ")

sum_digits = sum_of_digits_in_string(user_input)

print("Sum of digits:", sum_digits)


Programming Exercise #3

from datetime import datetime

def format_date(input_date):
    date_obj = datetime.strptime(input_date, '%m/%d/%y')

    formatted_date = date_obj.strftime('%B %d, %Y')

    return formatted_date


user_input = input("Enter a date in the format mm/dd/yyyy: ")

try:
    formatted_date = format_date(user_input)
    print("Formatted date:", formatted_date)
except ValueError:
    print("Invalid date format. Please enter a date in mm/dd/yyyy format.")








