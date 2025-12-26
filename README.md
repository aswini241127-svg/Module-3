# List Operations in Python: Sum of List Items

## 🎯 Aim
To write a Python program that calculates the **sum of all elements** in a list.

## 🧠 Algorithm
1. Define a list of numbers.
2. Use Python’s built-in `sum()` function to calculate the total.
3. Print the result.

## 🧾 Program
```
items=[153,147,124,102]
print(sum(items))
```

## Output
<img width="1185" height="233" alt="image" src="https://github.com/user-attachments/assets/ec4480e0-3a6d-4909-9805-8d45f41220c5" />

## Result
executed successfully
# Regex in Python: Filter Words Without the Letter 'e'

## 🎯 Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program
```
import re
words = ['apple', 'banana', 'cherry', 'date', 'fig', 'grape']
pattern = re.compile(r'^[^e]*$')
filtered_words = [word for word in words if pattern.match(word)]
print("Words without the letter 'e':", filtered_words)
```
## Output

<img width="612" height="55" alt="exp1" src="https://github.com/user-attachments/assets/ef05c847-2aae-4f13-ace7-c6bd08e51ef5" />

## Result
The program successfully filters and returns all elements from the list that do not contain 'e',using regex
# Module-3
# 🧹 Strings-Remove Nth Index Character from a String

## 🎯 Aim
To write a Python program that accepts a string and removes the character at a specified index.

## 🧠 Algorithm
1. Define a function named `remove` that takes the input string as an argument.
2. Read the index `n` from the user input.
3. Initialize an empty string `a` to store the new string.
4. Iterate over each index of the string using a `for` loop.
5. Check if the current index `i` is not equal to `n`.
6. If `i != n`, append the character at index `i` to string `a`.
7. After the loop, return the modified string `a`.
8. Print the final result.

## 💻 Program
```
# Function to remove character at index n
def remove(string, n):
    a = ""  # Initialize an empty string
    for i in range(len(string)):
        if i != n:  # Skip the character at index n
            a = a + string[i]
    return a

# Get input string from user
string = input("Enter a string: ")

# Get index to remove
n = int(input("Enter the index to remove: "))

# Display result
print("Modified string:", remove(string, n))
```
## Output

<img width="997" height="130" alt="exp1" src="https://github.com/user-attachments/assets/5f17b8db-fd42-440d-912f-27934b5c1580" />

## Result
The program successfully takes a string and an index number from the user, removes the character at the specified index, and prints the modified string without that character.
