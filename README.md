# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
```
import math
class cse:
    def mech(self,r):
        print("Area of circle:",round(math.pi*r**2,2))

r = int(input()) 
a = cse()
a.mech(r)
```


## Output
<img width="663" height="201" alt="image" src="https://github.com/user-attachments/assets/d40dbcb9-6e8e-48bc-887e-4259d65064e5" />

## Result
Thus , the program has been executed successfully.

## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
```
dict1 = eval(input())
dict2 = eval(input())
def merge(d1, d2):
    merged_dict = {**d1, **d2}
    return merged_dict
result = merge(dict1, dict2)
print(result)

```

## Output
<img width="1050" height="251" alt="image" src="https://github.com/user-attachments/assets/a232f47d-b6fc-4f3b-9581-0675085964d6" />


## Result
Thus , the program has been executed successfully.

# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
```
my_dict = {2: 56, 1: 2, 5: 12, 4: 24, 6: 18, 3: 323}

sorted_by_keys = dict(sorted(my_dict.items()))
sorted_by_values = dict(sorted(my_dict.items(), key=lambda item: item[1]))
print("Original dictionary:", my_dict)
print("Dictionary sorted by keys:", sorted_by_keys)
print("Dictionary sorted by values:", sorted_by_values)
```

## Sample Output
<img width="758" height="166" alt="image" src="https://github.com/user-attachments/assets/d188b2d8-8658-4c46-a2fb-8087b27d0e6b" />

## Result
Thus , the program has been executed successfully.
# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
```
list1 = [5, 10, 20,]

try:
    print(list1[5])
except IndexError:
    print("You're out of list range")
```

## Output
<img width="1052" height="141" alt="image" src="https://github.com/user-attachments/assets/f999fd15-96ac-4225-b610-840c481913bd" />

## Result
Thus , the program has been executed successfully.
# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
def count_lines_not_starting_with_T(filename):
    count = 0  
    with open(filename, "r") as file:
        for line in file:
            if not line.startswith('T'):
                count += 1
    return count

result = count_lines_not_starting_with_T("story.txt")
print("Number of lines that not starting with 'T':", result)

```
## Output

<img width="809" height="193" alt="image" src="https://github.com/user-attachments/assets/2701fb81-bba2-404d-877c-519b750117ff" />

## Result
Thus , the program has been executed successfully.
