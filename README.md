

# Interactive Personal Data Collector

 ## 📌 Description

 The **Interactive Personal Data Collector** is a simple Python program that collects basic information from the user, including:

 - Name
- Age
- Height
- Favorite number

 The program then displays the collected information along with the **data type** and **memory address** of each value. It also calculates an approximate birth year based on the user's age.

## Video Demo
https://drive.google.com/file/d/1yJlBZjvA_UPfDNv18-r-aHIIH0nsSvgZ/view?usp=sharing

 ## 🛠️ Technologies Used

 - **Python 3**
- `datetime` module
- Built-in functions such as `input()`, `print()`, `type()`, and `id()`

 ## 🚀 How to Run

 1. Make sure Python 3 is installed on your computer.
2. Save the program as a Python file, for example:

```
personal_data_collector.py
```

 3. Open a terminal or command prompt.
4. Run the program using:

```
python personal_data_collector.py
```

 ## 💻 How It Works

 The program asks the user to enter four pieces of information:

```
Enter your name
Enter your age
Enter your height
Enter your fav num
```

 The values are stored in variables:

```
a = input("enter your name")
b = int(input("enter your age"))
c = float(input("enter your height"))
d = int(input("enter your fav num"))
```

 The program uses different Python data types:

 | Variable | Information | Data Type |
| --- | --- | --- |
| `a` | Name | `str` |
| `b` | Age | `int` |
| `c` | Height | `float` |
| `d` | Favorite number | `int` |

## 🧮 Birth Year Calculation

 The program gets the current year using the `datetime` module:

```
import datetime

year = datetime.datetime.now().year
birth = year - b
```

 The approximate birth year is calculated by subtracting the user's age from the current year.

 > **Note:** The result is approximate because the program does not check whether the user's birthday has already occurred this year.

 ## 🔍 Data Types and Memory Addresses

 The program uses:

```
type()
```

 to display the type of each value and:

```
id()
```

 to display the object's identity/memory-related identifier.

 For example:

```
print("name", a, "(type is:)", type(a), "memory address:", id(a))
```

 ## 📋 Example Output

```
welcome to the interactive personal data collector

enter your name Alex
enter your age 20
enter your height 175.5
enter your fav num 7

thank you! here is the information we collected

name Alex (type is:) <class 'str'> memory address: 140123456789
name 20 (type is:) <class 'int'> memory address: 140123456790
name 175.5 (type is:) <class 'float'> memory address: 140123456791
name 7 (type is:) <class 'int'> memory address: 140123456792

your birth year is approximately 2006 (based on your age)

thank you for using personal data collector goodbye!
```

 The exact `id()` values will be different each time the program runs.

 ## 📚 Concepts Demonstrated

 This beginner-friendly project demonstrates:

 - User input with `input()`
- Type conversion with `int()` and `float()`
- Variables
- Strings, integers, and floating-point numbers
- `print()` statements
- The `type()` function
- The `id()` function
- Basic arithmetic
- Importing and using the `datetime` module

 ## ⚠️ Current Code Note

 In the current version, the birth-year line is:

```
print("your birth year is approximetely","year","(based on ypur age)")
```

 This prints the word **`year`** rather than the calculated value.

 To display the calculated birth year, use:

```
print("your birth year is approximately", birth, "(based on your age)")
```

 ## 🎯 Future Improvements

 Possible improvements include:

 - Add input validation for invalid ages and numbers.
- Improve the formatting of the output.
- Correct spelling and grammar in messages.
- Ask for the user's birthday for a more accurate birth year.
- Use descriptive variable names such as `name`, `age`, `height`, and `favorite_number`.
- Add error handling using `try` and `except`.

 ## 📄 License

 This project is intended for **learning and educational purposes**.

 This README is ready to save directly as **`README.md`** in the same folder as your Python program.
