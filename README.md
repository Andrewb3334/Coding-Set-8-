# Coding-Set-8-
Alg Workbench #3

mystring = "abc123def456ghi789"

count_digits = 0 

for char in mystring:
    if char.isdigit():
        count_digits += 1 

print("Number of digits in the string:", count_digits)

Alg Workbench #2

my string = "Hi, how are you doing today?"

count_spaces = 0 

for char in mystring:
    if char == ' ':
        count_spaces += 1 
print("Number of space characters in the string:", count_spaces)
