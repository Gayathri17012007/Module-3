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
~~~c
import re
def filter_without_e(words):
    pattern = re.compile(r'^[^eE]*$')
    return [word for word in words if pattern.match(word)]
word_list = ['apple', 'banana', 'cherry', 'fig', 'grape', 'kiwi']
filtered_words = filter_without_e(word_list)
print("Words without the letter 'e':", filtered_words)
~~~

## Output
![Screenshot 2025-05-11 095545](https://github.com/user-attachments/assets/c1020e41-94ce-4e44-b1f5-ef81882001ca)

## Result
Thus , the program has been executed successfully
