# Languages

## Python
- [Python](https://www.python.org/)
- [Python 3 Tutorial](https://docs.python.org/3/tutorial/index.html)
- [Python 3 Documentation](https://docs.python.org/3/)
- [Python 3 Standard Library](https://docs.python.org/3/library/index.html)
- [Python 3 Reference](https://docs.python.org/3/reference/index.html)
- [Python 3 Glossary](https://docs.python.org/3/glossary.html)
- [Python 3 Style Guide](https://www.python.org/dev/peps/pep-0008/)

- Python is a programming language that is easy to learn and use. Jasper literally have never used python before joining the team, and he was able to pick it up within 3 days. It is a very powerful language that is used in many different fields. It is used in web development, machine learning, data science, and many other fields. It is also a very popular language, so there is a lot of documentation and resources available for it.
- Python is the main programming language used by the team. It is easy to learn and has a lot of libraries that can be used to make your life easier. For instance, the ODrive library is written in Python, and it is used to control the ODrive motor controllers (more on this later).
- Though you are welcome to use any language you want, previously we used Rust, C++ and even C# from Unity!
- I don't think covering the basics of python is necessary, as there are many resources available online. However, I will cover some of the basics of python that you will need to know to get started with the team.

### Python Basics
- Python is an interpreted language, which means that you don't need to compile your code before running it. You can just run your code directly from the command line.
- Python is a dynamically typed language, which means that you don't need to specify the type of a variable when you declare it (though I strongly suggest that you do). This means that you can change the type of a variable at any time.
- Python is a whitespace sensitive language, which means that the indentation of your code matters. This is a bit different from other languages like C++ and Java, where the indentation doesn't matter. This is a bit of a controversial topic, but I personally think that it's a good thing. It makes your code more readable, and it makes it easier to spot errors.
- Python is an object oriented language, which means that everything in python is an object. This is a bit different from other languages like C++ and Java, where you have to explicitly declare objects. This is a bit of a controversial topic, but I personally think that it's a good thing. It makes your code more readable, and it makes it easier to spot errors.
- Python is a high level language, which means that it is very easy to learn and use. It is also a very powerful language, which means that you can do a lot of things with it. It is also a very popular language, which means that there is a lot of documentation and resources available for it.

### Python Syntax
- Python uses the `#` symbol to denote a comment. Anything after the `#` symbol will be ignored by the interpreter.
```python
# Your mom's a comment 😱😱😱
```
- Python uses the `print()` function to print text to the console.
```python
print("I hate this team and I wished I quit long ago!")
```
```
Terminal Output:
I hate this team and I wished I quit long ago!
```
- Python uses the `input()` function to get input from the user.
```python
name = input("What is your name? ")
print("Hello, " + name + "!")
```
```
What is your name? Jasper
Hello, Jasper!
```
- Python uses the `if` statement, `elif`, and `else` to execute code if a condition is true/false.
```python
if 1 == 1:
    print("1 is equal to 1!")
```
```python
if 1 == 2:
    print("1 is equal to 2!")
elif 1 == 3:
    print("1 is equal to 3!")
else:
    print("1 is not equal to 2 or 3!")
```
```python
# wtf is this, what happened here?
odrv.config.brake_resistance = 2.0 if powerDC else 0.0
# this is called a ternary operator btw. It's a shorthand for an if statement.
```
- Python uses the `for` and `while` statement to loop through a list.
```python
for i in range(10):
    print(i)
```
```python
for i in range(10):
    if i == 5:
        break
    print(i)
```
```python
while True:
    print("I'm stuck in an infinite loop!")
```
- Python uses the `def` keyword to define a function.
```python
def add(a, b):
    return a + b
```
- You can also define the return type, and variable type, but it's not necessary.
```python
# Is the same as the function above
def add(a: int, b: int) -> int:
    return a + b
```
- Python uses the `class` keyword to define a class.
```python
class Person:
    def __init__(self, name):
        self.name = name

    def say_hello(self):
        print("Hello, my name is " + self.name + "!")
```
- Python uses the `import` keyword to import a library.
```python
import math
```
- Python uses the `from` keyword to import a specific function from a library.
```python
from math import sqrt
```
- Python uses the `as` keyword to rename a library.
```python
import math as m

# Now you can use m instead of writing out math, like this:
print(m.sqrt(4))
```
- Python uses the `try` and `except` keywords to catch errors.
```python
try:
    print(1 / 0)
except ZeroDivisionError:
    print("You can't divide by zero!")
```
- Python uses the `with` keyword to open a file.
```python
with open("file.txt", "r") as file:
    print(file.read())
```
- Python uses the `pass` keyword to do nothing.
```python
if 1 == 1:
    pass
```
- Python uses the `in` keyword to check if a value is in a list.
```python
if 1 in [1, 2, 3]:
    print("1 is in the list!")
```
- Python uses the `is` keyword to check if two variables are the same.
```python
a = 1
b = 1
if a is b:
    print("a and b are the same!")
```
- Python uses the `and` and `or` keywords to check if multiple conditions are true.
```python
if 1 == 1 and 2 == 2:
    print("Both conditions are true!")
```
```python
if 1 == 1 or 2 == 3:
    print("At least one condition is true!")
```

### Python Data Types
- Python has 5 basic data types: `int`, `float`, `bool`, `str`, and `NoneType`.
- `int` is a whole number, like `1`, `2`, `3`, etc.
- `float` is a decimal number, like `1.0`, `2.5`, `3.14159265359`, etc.
- `bool` is a boolean value, which can be either `True` or `False`.
- `str` is a string, which is a sequence of characters.
- `NoneType` is a special type that represents the absence of a value.
- Python also has 3 complex data types: `list`, `tuple`, and `dict`.
- `list` is a list of values, which can be of any type.
    + You can access a specific value in a list by using the index of that value.
    + You can also use negative indices to access values from the end of the list.
    + You can also use the `len()` function to get the length of a list.
    + You can also use the `append()` function to add a value to the end of a list.
    + You can also use the `insert()` function to add a value to a specific index in a list.
    + You can also use the `remove()` function to remove a value from a list.
    + You can also use the `pop()` function to remove a value from a specific index in a list.
    + You can also use the `sort()` function to sort a list.
    + You can also use the `reverse()` function to reverse a list.
    + You can also use the `clear()` function to clear a list.
    + etc...
    + Code Example:
    ```python
    list = [1, 2, 3, 4, 5]
    print(list[0])      # 1
    print(list[-1])     # 5
    print(len(list))    # 5
    list.append(6)
    print(list)         # [1, 2, 3, 4, 5, 6]
    list.insert(0, 0)
    print(list)         # [0, 1, 2, 3, 4, 5, 6]
    ```
- `tuple` is a list of values, which can be of any type, but it is immutable.
    + You can access a specific value in a tuple by using the index of that value.
    + You can also use negative indices to access values from the end of the tuple.
    + You can also use the `len()` function to get the length of a tuple.
    + Code Example:
    ```python
    tuple = (1, 2, 3, 4, 5)
    print(tuple[0])     # 1
    print(tuple[-1])    # 5
    print(len(tuple))   # 5
    ```
    ```python
    gp = gmi.getGamepad(0)
    (ls_x, ls_y) = gmi.getLeftStick(gp, AXIS_DEADZONE)  # tuple unpacking, returns more than one value
    ```
- `dict` is a dictionary, which is a list of key-value pairs.
    + You can access a specific value in a dictionary by using the key of that value.
    + You can also use the `len()` function to get the length of a dictionary.
    + You can also use the `keys()` function to get a list of all the keys in a dictionary.
    + You can also use the `values()` function to get a list of all the values in a dictionary.
    + You can also use the `items()` function to get a list of all the key-value pairs in a dictionary.
    + You can also use the `clear()` function to clear a dictionary.
    + You can also use the `get()` function to get a value from a dictionary.
    + You can also use the `pop()` function to remove a value from a dictionary.
    + You can also use the `popitem()` function to remove a random key-value pair from a dictionary.
    + You can also use the `update()` function to update a dictionary with another dictionary.
    + etc...
    + Code Example:
    ```python
    dict = {"a": 1, "b": 2, "c": 3}
    print(dict["a"])    # 1
    print(len(dict))    # 3
    print(dict.keys())  # ["a", "b", "c"]
    print(dict.values())    # [1, 2, 3]
    print(dict.items())     # [("a", 1), ("b", 2), ("c", 3)]
    ```
    + More high level examples:
    ```python
    # ---- Target List ------------------------------------------------
    a = { "motor" : axis.motor, "encoder" : axis.encoder }

    c = {
        "Motor State"   : [AXIS_STATE_MOTOR_CALIBRATION, a["motor"].error],
        "Hall Polarity" : [AXIS_STATE_ENCODER_HALL_POLARITY_CALIBRATION, a["encoder"].error],
        "Hall Phase"    : [AXIS_STATE_ENCODER_HALL_PHASE_CALIBRATION, a["encoder"].error],
        "Hall Offset"   : [AXIS_STATE_ENCODER_OFFSET_CALIBRATION, a["encoder"].error]
    }

    # ---- Calibration Function ---------------------------------------
    def calib(target : str):
        logger.debug("Calibrating {}... 🤞".format(target))
        axis.requested_state = c[target][0]
        log_state()
        if c[target][1] != 0:
            logger.error("Error at {} 😢".format(target))
            print("\t> Error: ", c[target][1])
            sys.exit()

    # ---- Pre-Calibration Function -----------------------------------
    def pre_calib(target : str):
        logger.debug("Setting {} to precalibrated... 😎️".format(target))
        a[target].config.pre_calibrated = True
        log_state()

    # ---- Debugging Function -----------------------------------------
    def log_state():
        print("\t> OdriveSN: ",odrv_num, "-- Axis: ", axis_num, "-- State: ", axis.current_state, " <")
        while axis.current_state != AXIS_STATE_IDLE:
            time.sleep(2)
        print("\t> OdriveSN: ",odrv_num, "-- Axis: ", axis_num, "-- State: ", axis.current_state, " <")
        time.sleep(5)

    calib("Motor State")
    pre_calib("motor")
    calib("Hall Polarity")
    calib("Hall Phase")
    calib("Hall Offset")
    pre_calib("encoder")
    ```

-----------------------------------------

## C++

- Bruh, do you even take CS classes at Saddleback? 😂
- Go back to class and learn C++ first. 😂
- ( I recommend taking Professor Rousseau, Bodhanwala, Nadia and Rainey! )