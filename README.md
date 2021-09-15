## [**Python Tutorial**](https://www.youtube.com/watch?v=rfscVS0vtbw&t=2078s)
____
### **Intro**

* _Python_ is a programing language.
* Need a _text editor_ to write code in (notepad, text edit, etc.)
>Note: There are special text editors for writing python code called IDE's (integrated develepment environments), we will use _PyCharm_.
____
### **Variables**
* A _variable_ is a container where we can store certain data types.
    ```python
    variable_name = "some value"
    ```
____
### **Data Types**

* **Strings** - Store text. Must be written in quotations.
    ```python
    character_name = "Tom"
    ```
* **Numbers** - Store whole or decimal numbers. 
    ```python
    character_age = 50
    ```
* **Boolians** - Store True or False value.
    ```python
    is_male = True
    ```
>Note: Can adjust data types in middle of code.
____
### **Working With Strings**
\
**Example 1:** We can use the print function to print different data types (strings in this case).

```python
print("Giraffe Academy")
```
>_Returns:_ Giraffe Academy

\
**Example 2:** We can store this string value inside of a variable (phrase).

```python
phrase = "Giraffe Academy"
print(phrase)
```
>_Returns:_ Giraffe Academy

\
**Example 3:** Concatination is the process of joining strings together.

```python
phrase = "Giraffe Academy"
print(phrase + "is cool")
```
>_Returns:_ Giraffe Academy is cool

\
**Example 4:** We can also use functions to modify/ get information, about our strings.
```python
phrase = "Giraffe Academy"
print(phrase_______)
```
|phrase(_______)  |Returns         |Description                                           |
| ---             | ---            | ---                                                  |
|.lower()         |giraffe academy |Converts entire string to lower case                  |
|.upper()         |GIRAFFE ACADEMY |Converts entire string to upper case                  |
|.islower()       |False           |Checks if phrase is lower case and returns a T/F value|
|.isupper()       |False           |Checks if phrase is upper case and returns a T/F value|
|[0]              |G               |Returns string value corresponding to its index number|
|.index("G")      |0               |Returns index number corresponding to its string value|
|.replace("G","J")|Jiraffe Academy |Functions as a search and replace                     |
|                 |                |                                                      |
>Note: Index numbers are assigned begining at 0 (i.e. G = 0, i = 1, r = 3, etc.)

\
**Example 5:** Functions can be used in combination with eachother.
```python
phrase = "Giraffe Academy"
print(phrase.upper().isupper())
```

>_Returns:_ True

\
**Example 6:** The length function will return the length of a string.
```python
phrase = "Giraffe Academy"
print(len(phrase))
```
>_Returns:_ 15

\
**Example 7:** Backslashes can be used in various ways to modify the output.

|print("______")  |Returns         |Description                         |
| ---             | ---            | ---                                |
|Giraffe Academy  |Giraffe Academy |Prints string with a space inbetween|
|Giraffe\\"Academy|Giraffe"Academy |Prints quotation mark               |
|Giraffe\\Academy |Giraffe\Academy |Prints string with a backslash      |
|Giraffe\nAcademy |Giraffe         |Prints string on a new line         |
|                 |Academy         |                                    |
|                 |                |                                    |

>Note: A backslash is called the escape character; meaning that whatever character comes after it we want to render literally.
___
### **Working With Numbers**
\
**Example 1:** We can use the print function to cary out various mathematic equations and print the results.
```python
print(10 _ 3)
```
|print(10 _ 3)|Returns|Description                       |
|:---:        |:---:  |---                               |
|+            |13     |Addition                          |
|-            |7      |Subtraction                       |
|/            |3.333  |Division                          |
|*            |30     |Multiplication                    |
|%            |1      |Modulus operator returns remainder|
|             |       |                                  |
>Note: Parentheses can be used to specify order of operations.

>Note: Python can handle whole numbers, decimal numbers and negative numbers.

\
**Example 2:** Common functions using numbers.
```python
num = -5
print(______)
```
|print(______)|Returns|Description                     |
|:---:        |:---:  |---                             |
|num          |-5     |Returns variable in integer form|
|str(num)     |-5     |Returns variable in string form |
|abs(num)     |5      |Returns absolute value          |
|pow(3,2)     |9      |3^2                             |
|max(3,2)     |3      |Returns larger number           |
|min(3,2)     |2      |Returns smaller number          |
|round(3.2)   |3      |Rounds input                    |
|             |       |                                |

>Note: You need to convert numbers into strings in order to print them alongside strings.

\
**Example 3:** In order to access certain functions we need to import python math.
```python
from math import*
print(______)
```
|print(______)|Returns|Description         |
|:---:        |:---:  |---                 |
|floor(3.7)   |3      |Cuts off lower value|
|ceil(3.7)    |4      |Rounds up           |
|sqrt(36)     |6      |Returns square root |
___
### **How to get user input**
\
**Example 1:** Prompts user for name and age and returns input alongside strings.
```python
name = input("Enter your name: ")
age = input("Enter your age: ")
print("Hello " + name + "! You are " + age)
```
>_Returns:_ Hello Ashley! You are 31

\
**Example 2:** Prompts user for two numbers and returns their sum.
```python
num1 = input("Enter a number: ")
num2 = input("Enter another number: ")
result = float(num1) + float(num2)
print(result)
```
>Note: Both num1 and num2 are stored in string form and therefore must be converted into either integer (for whole numbers) or float form(for decimal numbers).
___
### **Dealing with Lists**
\
**Example 1:**
```python
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
print(_______)
```
|print(______)|Description|
|:---:|---|
|friends|Prints entire list|
|friends[0]|Prints name corresponding to index number|
|friends[1:]|Prints index 1 and all elements after|
|friends[1:3]|Prints from index 1 up to index 3|

\
**Example 2:**
```python
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
friends[1] = "Mike"
print(friends[1])
```
>Note: This will modify index 1 (karen) and instead print Mike.