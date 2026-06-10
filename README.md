# PY-PRACTICE

# 🐍 Python Roadmap — Week 1
## Complete Beginner's Study Guide
### "From Zero to Python — Your First Step Towards DSA, LeetCode & Backend Development"

---

> **Who is this guide for?**
> You have ZERO programming experience. That's perfect. This guide is written like a teacher sitting next to you, explaining every single thing — step by step, with zero assumptions. By the end of Week 1, you will be able to write real Python programs.

---

# CHAPTER 1: Introduction to Programming

---

## 1.1 What is Programming?

### WHY does programming exist?

Imagine you want a robot to make tea for you every morning. The robot is very obedient — it will do EXACTLY what you tell it. But it cannot think on its own. You have to give it clear, step-by-step instructions:

1. Go to the kitchen
2. Pick up the kettle
3. Fill it with 500ml of water
4. Turn on the stove
5. Wait until water boils
6. Pour water into a cup
7. Add a tea bag
8. Wait 3 minutes
9. Remove tea bag
10. Bring the cup to me

This list of instructions is called a **PROGRAM**.

A computer is like that robot. It is extremely fast and obedient, but it cannot think. It needs YOU to write the instructions. Programming is the skill of writing those instructions for a computer.

### What is Programming? (Simple Definition)

> **Programming = Writing step-by-step instructions for a computer to follow.**

Computers understand only electricity — ON (1) and OFF (0). But humans think in words and logic. Programming languages (like Python) act as a translator between human thinking and computer understanding.

### Why Does Programming Exist?

Before computers, everything was manual:
- Banks counted money by hand
- Doctors kept paper records
- Communication happened by letter

Today, computers handle ALL of that — because programmers wrote instructions telling them how. Every app on your phone, every website, every video game, every ATM machine — all of it runs because of programs that a programmer wrote.

**Programming exists because:**
- Computers are fast but dumb — they need instructions
- Humans are smart but slow — we can write those instructions once, and the computer runs them a million times per second

---

## 1.2 What is Python?

Python is a **programming language** — a tool humans use to write instructions for computers.

Just like humans speak different languages (Hindi, English, Telugu), computers understand programs written in different programming languages. Python is one such language.

### Why is Python Beginner-Friendly?

Look at these two examples that do the SAME thing (print "Hello World"):

**In C++ (hard for beginners):**
```cpp
#include 
using namespace std;
int main() {
    cout << "Hello World" << endl;
    return 0;
}
```

**In Python (easy!):**
```python
print("Hello World")
```

Python reads almost like English. That's why it's perfect for beginners.

### Why Python for DSA, LeetCode & Backend?

|
 Goal 
|
 Why Python Works 
|
|
------
|
-----------------
|
|
 DSA & LeetCode 
|
 Clean syntax lets you focus on logic, not language complexity 
|
|
 Competitive Programming 
|
 Fast to write, huge standard library 
|
|
 Backend Development 
|
 Django, Flask, FastAPI — world-class frameworks 
|
|
 Jobs 
|
#
1 most in-demand language worldwide 
|

### Memory Tip 🧠
> **Python = Simple English for computers.** Guido van Rossum created Python in 1991, naming it after the comedy show "Monty Python's Flying Circus" — not the snake!

---

## 1.3 Interpreter vs Compiler

### WHY do we need to understand this?

When you write Python code, the computer doesn't magically understand it. Your code needs to be "translated" into machine language (0s and 1s) that the CPU can understand. There are two ways this translation can happen.

### The Analogy

Imagine you write a speech in Hindi, but your audience only understands English.

**Compiler = Book Translator**
- Takes your entire Hindi book
- Translates the WHOLE thing into English first
- Then gives the English book to the audience
- Once translated, the audience reads the English version directly (very fast)
- Languages: C, C++, Java (partially)

**Interpreter = Live Interpreter**
- Reads one sentence of your Hindi speech at a time
- Translates it to English line by line, RIGHT NOW, as you speak
- Languages: **Python**, JavaScript, Ruby

### Python is an Interpreted Language

```
Your Python Code (.py file)
         ↓
    Python Interpreter
         ↓
   Machine Language (0s and 1s)
         ↓
      CPU executes it
         ↓
       Output appears
```

**What this means for you:**
- You write code → you run it → you see output IMMEDIATELY
- No separate "compile" step needed
- Errors show up line by line (easier to debug)

---

## 1.4 Source Code

**Source code** is the code YOU write — the human-readable instructions.

When you type:
```python
print("Hello World")
```

That text is your **source code**. It's stored in a file with a `.py` extension (like `hello.py`).

The Python interpreter reads your source code and executes it.

---

## 1.5 Program Execution Flow

Here's exactly what happens when you run a Python program:

```
Step 1: You write code in a .py file
           ↓
Step 2: You run the file (python hello.py)
           ↓
Step 3: Python Interpreter reads your code
           ↓
Step 4: Interpreter converts code to bytecode (.pyc)
           ↓
Step 5: Python Virtual Machine (PVM) runs the bytecode
           ↓
Step 6: CPU executes the instructions
           ↓
Step 7: Output appears on your screen
```

Don't worry about memorising all of this. Just know: **you write → python runs it → you see output.**

---

## 1.6 CPU and RAM Basics

You don't need to be a hardware engineer. But understanding this helps you think like a programmer.

### CPU (Central Processing Unit) — The Brain

- The CPU is the "thinker" of the computer
- It executes instructions — billions per second
- When your Python code runs, the CPU is doing the actual work
- Think of it as a super-fast calculator that never gets tired

### RAM (Random Access Memory) — The Workspace

- RAM is your computer's "working memory"
- When you run a Python program, the program loads into RAM
- Variables you create are stored in RAM
- RAM is TEMPORARY — when you close the program, RAM is cleared
- Think of RAM as a whiteboard — you write on it while working, erase it when done

### Why Does This Matter for Programming?

```
Your .py file (stored on Hard Drive)
         ↓  (when you run it)
  Loaded into RAM (temporary workspace)
         ↓  (CPU processes it)
  CPU reads from RAM, executes instructions
         ↓
  Output goes to Screen
```

When you create a variable like `x = 5`, Python stores the value `5` in RAM. This is why variables disappear when your program ends — RAM gets cleared!

---

# CHAPTER 2: Python Setup

---

## 2.1 Installing Python

### Step-by-Step Installation (Windows)

1. Go to **https://www.python.org/downloads/**
2. Click the big yellow button: **"Download Python 3.x.x"**
3. Run the downloaded `.exe` file
4. ⚠️ **VERY IMPORTANT:** Check the box that says **"Add Python to PATH"** before clicking Install
5. Click **"Install Now"**
6. Wait for installation to complete
7. Click **"Close"**

### Verify Installation

Open **Command Prompt** (press `Windows + R`, type `cmd`, press Enter) and type:

```
python --version
```

You should see something like:
```
Python 3.12.0
```

If you see this — Python is installed! 🎉

### For Mac Users
1. Go to **https://www.python.org/downloads/**
2. Download the macOS installer
3. Run the `.pkg` file and follow instructions
4. Open Terminal and type `python3 --version`

---

## 2.2 Installing VS Code

VS Code (Visual Studio Code) is a free code editor made by Microsoft. It's where you'll write your Python code.

### Installation Steps

1. Go to **https://code.visualstudio.com/**
2. Click **"Download for Windows"** (or your OS)
3. Run the installer and follow the steps
4. Open VS Code after installation

### Install Python Extension in VS Code

1. Open VS Code
2. Click the **Extensions icon** on the left sidebar (looks like 4 squares)
3. Search for **"Python"**
4. Click **"Install"** on the extension by Microsoft
5. Done!

---

## 2.3 Running Python Files

### Method 1: Using VS Code

1. Open VS Code
2. Click **File → New File**
3. Save it as `hello.py` (the `.py` extension is important!)
4. Type your code
5. Press **Ctrl + F5** to run

### Method 2: Using Terminal

1. Open Terminal / Command Prompt
2. Navigate to your file's folder:
   ```
   cd Desktop
   ```
3. Run your file:
   ```
   python hello.py
   ```

---

## 2.4 Terminal Basics

The terminal (also called Command Prompt on Windows, Terminal on Mac/Linux) is a text-based way to talk to your computer.

### Essential Commands

|
 Command 
|
 What it Does 
|
 Example 
|
|
---------
|
-------------
|
---------
|
|
`cd foldername`
|
 Enter a folder 
|
`cd Desktop`
|
|
`cd ..`
|
 Go back one folder 
|
`cd ..`
|
|
`dir`
 (Windows) / 
`ls`
 (Mac) 
|
 List files in current folder 
|
`dir`
|
|
`python filename.py`
|
 Run a Python file 
|
`python hello.py`
|
|
`cls`
 (Windows) / 
`clear`
 (Mac) 
|
 Clear the screen 
|
`cls`
|

### Practice This!

Create a folder called `python_practice` on your Desktop. Put your `.py` files there. Then navigate to it in terminal:

```
cd Desktop
cd python_practice
python hello.py
```

---

# CHAPTER 3: The print() Function

---

## WHY do we learn print() first?

A program that produces no output is useless — you can't see what it did! `print()` is how your program communicates with you. It displays text on the screen. It's the most fundamental output tool in Python.

Think of `print()` as your program saying: **"Hey! Look at this!"**

---

## 3.1 Basic print()

### Syntax

```python
print(value)
```

### Examples

```python
print("Hello, World!")
print("I am learning Python")
print("This is my first program")
```

### Output
```
Hello, World!
I am learning Python
This is my first program
```

### Key Rules
- Everything inside the parentheses `()` gets displayed
- Text (words, sentences) must be wrapped in **quotes** — either single `'hello'` or double `"hello"`
- Numbers don't need quotes: `print(42)` works fine
- Each `print()` automatically goes to a new line

### More Examples

```python
print("My name is Arjun")
print(2024)
print(3.14)
print(True)
```

Output:
```
My name is Arjun
2024
3.14
True
```

---

## 3.2 Multiple Arguments in print()

You can pass multiple values to `print()` separated by commas.

```python
print("My name is", "Arjun")
print("I am", 20, "years old")
print("Pi is approximately", 3.14)
```

Output:
```
My name is Arjun
I am 20 years old
Pi is approximately 3.14
```

> **Notice:** Python automatically puts a SPACE between each value. That's the default separator.

---

## 3.3 The sep Parameter

`sep` controls what goes BETWEEN multiple values. By default it's a space `" "`.

### Syntax

```python
print(value1, value2, value3, sep="separator")
```

### Examples

```python
# Default separator (space)
print("apple", "banana", "cherry")

# Custom separator
print("apple", "banana", "cherry", sep=", ")
print("2024", "01", "15", sep="-")
print("www", "google", "com", sep=".")
print("a", "b", "c", sep="---")
```

Output:
```
apple banana cherry
apple, banana, cherry
2024-01-15
www.google.com
a---b---c
```

### Real-World Use Case

```python
# Building a date format
day = 15
month = 8
year = 2024
print(day, month, year, sep="/")
```

Output:
```
15/8/2024
```

---

## 3.4 The end Parameter

By default, every `print()` adds a **newline** (`\n`) at the end — that's why each print goes to a new line. The `end` parameter lets you change that.

### Syntax

```python
print(value, end="something")
```

### Examples

```python
# Default behavior (end="\n")
print("Hello")
print("World")

# Change end to space
print("Hello", end=" ")
print("World")

# Change end to nothing
print("Hello", end="")
print("World")

# Change end to custom string
print("Loading", end="...")
print("Done!")
```

Output:
```
Hello
World
Hello World
HelloWorld
Loading...Done!
```

---

## 3.5 Escape Sequences

Escape sequences are special characters that start with a backslash `\`. They represent characters that are hard to type directly.

|
 Escape Sequence 
|
 What it Does 
|
 Example 
|
|
----------------
|
-------------
|
---------
|
|
`\n`
|
 New line 
|
`"Hello\nWorld"`
|
|
`\t`
|
 Tab (horizontal space) 
|
`"Name:\tArjun"`
|
|
`\\`
|
 Backslash itself 
|
`"C:\\Users\\file"`
|
|
`\'`
|
 Single quote inside single quotes 
|
`'I\'m learning'`
|
|
`\"`
|
 Double quote inside double quotes 
|
`"He said \"hi\""`
|

### Examples

```python
print("Line 1\nLine 2\nLine 3")
print("Name:\tArjun")
print("Score:\t95")
print("File path: C:\\Users\\Arjun\\file.txt")
print("She said, \"Hello!\"")
```

Output:
```
Line 1
Line 2
Line 3
Name:   Arjun
Score:  95
File path: C:\Users\Arjun\file.txt
She said, "Hello!"
```

### Practical Example — Making a Table

```python
print("Name\t\tScore\tGrade")
print("Arjun\t\t95\tA")
print("Priya\t\t87\tB")
print("Rahul\t\t76\tC")
```

Output:
```
Name            Score   Grade
Arjun           95      A
Priya           87      B
Rahul           76      C
```

---

## 3.6 Comments

### WHY use comments?

Imagine writing 500 lines of code, then coming back to it 3 months later. Without explanations, you won't understand your own code! Comments are notes you leave in your code — for yourself and for others. **Python completely ignores comments when running the program.**

### Single-Line Comments

```python
# This is a comment - Python ignores this line
print("Hello")  # This prints Hello

# Calculating area of a rectangle
length = 10  # length in meters
width = 5    # width in meters
```

### Multi-Line Comments (Docstrings)

```python
"""
This is a multi-line comment.
It can span multiple lines.
Useful for explaining what a whole section does.
"""
print("This line runs")
```

### Best Practice: WHEN to comment

```python
# GOOD comment - explains WHY
# Using integer division because we need whole number of groups
groups = students // 5

# BAD comment - just repeats what code already says
# Add 1 to x
x = x + 1
```

---

## Common Mistakes — print()

```python
# MISTAKE 1: Missing quotes around text
print(Hello)        # ❌ Error!
print("Hello")      # ✅ Correct

# MISTAKE 2: Wrong bracket type
print["Hello"]      # ❌ Error! Square brackets are wrong
print("Hello")      # ✅ Correct

# MISTAKE 3: Mixing quote types
print("Hello')      # ❌ Error! Open with ", close with "
print("Hello")      # ✅ Correct

# MISTAKE 4: Forgetting parentheses
print "Hello"       # ❌ This is Python 2 syntax, won't work in Python 3
print("Hello")      # ✅ Correct
```

---

## Practice Exercises — print()

1. Print your full name
2. Print your city and country on separate lines using ONE print statement with `\n`
3. Print the numbers 1, 2, 3 on the SAME line with dashes between them (like `1-2-3`)
4. Print a simple address card:
   ```
   Name:    Your Name
   Age:     Your Age
   City:    Your City
   ```
5. Print "Hello" 5 times on the same line using only 2 print statements

---

# CHAPTER 4: Variables

---

## WHY do we need variables?

Imagine you're building a program that calculates a student's final grade. The program needs to remember the student's name, marks in 5 subjects, and attendance. Without variables, where would those values go?

A **variable** is like a labelled box in RAM. You put a value inside it, give it a name, and then use that name whenever you need the value.

```
BOX ANALOGY:

  +----------+       +----------+       +----------+
  |          |       |          |       |          |
  |    25    |       |  "Arjun" |       |   True   |
  |          |       |          |       |          |
  +----------+       +----------+       +----------+
   label: age        label: name       label: is_student
```

---

## 4.1 Creating a Variable (Assignment)

### Syntax

```python
variable_name = value
```

The `=` sign means **"store this value into this variable"** — NOT "equals" like in math!

### Examples

```python
name = "Arjun"
age = 20
height = 5.9
is_student = True
```

### Using Variables

```python
name = "Arjun"
age = 20

print("Name:", name)
print("Age:", age)
print(name, "is", age, "years old")
```

Output:
```
Name: Arjun
Age: 20
Arjun is 20 years old
```

---

## 4.2 Variable Naming Rules

### MUST Follow (Syntax Rules — Python will give error if violated)

|
 Rule 
|
 Wrong ❌ 
|
 Right ✅ 
|
|
------
|
---------
|
---------
|
|
 Only letters, digits, underscores 
|
`my-name`
|
`my_name`
|
|
 Cannot start with a digit 
|
`2name`
|
`name2`
|
|
 No spaces allowed 
|
`my name`
|
`my_name`
|
|
 No special characters 
|
`name@1`
|
`name_1`
|
|
 Case-sensitive 
|
`Age`
 ≠ 
`age`
|
 (both are different vars) 
|

### SHOULD Follow (Best Practices — Python won't error, but bad habit)

```python
# BAD names (meaningless)
x = "Arjun"
a = 20
b = True

# GOOD names (descriptive)
student_name = "Arjun"
student_age = 20
is_enrolled = True
```

### Reserved Words (Keywords)

These words are reserved by Python — you CANNOT use them as variable names:

```
if    else   elif   while   for    in
not   and    or     True    False  None
def   class  return import  from   try
```

```python
# WRONG - 'if' is a keyword
if = 10      # ❌ SyntaxError

# RIGHT
condition = 10   # ✅
```

---

## 4.3 Reassignment

You can change a variable's value at any time. The new value replaces the old one.

```python
score = 0
print("Initial score:", score)

score = 50
print("After round 1:", score)

score = 95
print("Final score:", score)
```

Output:
```
Initial score: 0
After round 1: 50
Final score: 95
```

**Memory Tip 🧠:** Think of a variable like a whiteboard. You write something, then erase it and write something new. The whiteboard itself doesn't change — only what's written on it.

---

## 4.4 Multiple Assignment

### Assign same value to multiple variables

```python
x = y = z = 0
print(x, y, z)
```

Output:
```
0 0 0
```

### Assign multiple variables in one line

```python
name, age, city = "Arjun", 20, "Hyderabad"
print(name)
print(age)
print(city)
```

Output:
```
Arjun
20
Hyderabad
```

---

## 4.5 Swapping Variables

Swapping means exchanging the values of two variables. This is a CLASSIC programming problem and appears in DSA.

### Method 1: Using a Temporary Variable (Classic Method)

```python
a = 10
b = 20

print("Before swap: a =", a, ", b =", b)

# Swap
temp = a    # temp = 10
a = b       # a = 20
b = temp    # b = 10

print("After swap: a =", a, ", b =", b)
```

Output:
```
Before swap: a = 10 , b = 20
After swap: a = 20 , b = 10
```

### Method 2: Python's One-Line Swap (Pythonic Way) ⭐

```python
a = 10
b = 20

a, b = b, a    # Magic one-liner!

print("a =", a, ", b =", b)
```

Output:
```
a = 20 , b = 10
```

> This is called **tuple unpacking** — unique to Python. Use this in interviews!

---

## Common Mistakes — Variables

```python
# MISTAKE 1: Using a variable before assigning it
print(score)     # ❌ NameError: name 'score' is not defined
score = 10
print(score)     # ✅

# MISTAKE 2: Confusing = and ==
x = 5            # = means "assign"
x == 5           # == means "is equal to?" (comparison) — used in conditions

# MISTAKE 3: Case confusion
Name = "Arjun"
print(name)      # ❌ NameError! 'name' is different from 'Name'

# MISTAKE 4: Starting with a number
1st_score = 95   # ❌ SyntaxError
first_score = 95 # ✅
```

---

## Practice Exercises — Variables

1. Create variables for your name, age, and favourite subject. Print them in a sentence.
2. Create a variable `temperature = 37`. Change it to 38.5, then print both "before" and "after" values.
3. Create two variables `first_name = "Ravi"` and `last_name = "Kumar"`. Print the full name using both variables.
4. Swap two variables `x = 100` and `y = 200` using both methods (temp variable and one-liner).
5. What happens if you name a variable `for`? Try it and note the error.

---

# CHAPTER 5: Data Types

---

## WHY do data types exist?

Think about real life. A "name" and an "age" are completely different kinds of information. You wouldn't do math on a name, and you wouldn't use an age as a title. Computers need to know WHAT TYPE of data they're dealing with so they know how to store it and what operations make sense.

For example:
- `10 + 20 = 30` (makes sense — adding numbers)
- `"Arjun" + "Kumar" = "ArjunKumar"` (makes sense — joining words)
- `"Arjun" + 20 = ???` (makes NO sense — can't add name and number)

Data types are Python's way of categorizing data so it knows what operations are allowed.

---

## 5.1 int (Integer)

Whole numbers — no decimal point. Can be positive, negative, or zero.

```python
age = 20
temperature = -5
students = 45
year = 2024
big_number = 1000000

print(age)
print(temperature)
print(big_number)
```

Output:
```
20
-5
1000000
```

**Range:** In Python 3, integers can be INFINITELY large (unlike other languages). Python handles big numbers automatically!

```python
huge = 99999999999999999999999999999999
print(huge)    # Python handles this perfectly!
```

---

## 5.2 float (Floating Point Number)

Numbers WITH a decimal point.

```python
height = 5.9
price = 299.99
pi = 3.14159
temperature = -3.5
zero_point = 0.0

print(height)
print(price)
print(pi)
```

Output:
```
5.9
299.99
3.14159
```

### Important Float Quirk ⚠️

```python
print(0.1 + 0.2)
```

Output:
```
0.30000000000000004
```

This looks wrong! It's actually a computer science issue — computers store decimal numbers in binary (0s and 1s), and 0.1 can't be represented exactly. This is called **floating point imprecision** and affects ALL programming languages, not just Python. Keep this in mind for financial calculations.

---

## 5.3 str (String)

Text data — any sequence of characters (letters, numbers, symbols) enclosed in quotes.

```python
name = "Arjun Kumar"
city = 'Hyderabad'
message = "Hello, World!"
digits_as_text = "12345"     # This is text, NOT a number!
empty = ""                    # Empty string

print(name)
print(city)
print(digits_as_text)
```

Output:
```
Arjun Kumar
Hyderabad
12345
```

### String Concatenation (Joining Strings)

```python
first_name = "Arjun"
last_name = "Kumar"
full_name = first_name + " " + last_name
print(full_name)
```

Output:
```
Arjun Kumar
```

### String Repetition

```python
line = "-" * 20
print(line)
print("ha" * 3)
```

Output:
```
--------------------
hahaha
```

### Multi-line Strings

```python
message = """Dear Arjun,
Welcome to Python!
Let's learn together.
"""
print(message)
```

Output:
```
Dear Arjun,
Welcome to Python!
Let's learn together.
```

---

## 5.4 bool (Boolean)

Only TWO possible values: `True` or `False`. That's it. Extremely important for decision-making in programs.

```python
is_raining = True
is_hungry = False
has_passed = True
is_logged_in = False

print(is_raining)
print(is_hungry)
```

Output:
```
True
False
```

### Where Booleans Come From

```python
print(10 > 5)     # True (yes, 10 IS greater than 5)
print(10 < 5)     # False (no, 10 is NOT less than 5)
print(10 == 10)   # True (yes, they are equal)
print(10 == 11)   # False (no, they are not equal)
```

Output:
```
True
False
True
False
```

**Memory Tip 🧠:** `True` and `False` MUST start with a capital letter in Python. `true` and `false` will cause errors!

---

## 5.5 None

`None` means "nothing", "empty", "no value". It's Python's way of saying "this variable exists but has no data yet."

```python
result = None
winner = None

print(result)
print(winner)
```

Output:
```
None
None
```

**When do you use None?**
- When a function finds nothing to return
- As a placeholder before you have a real value
- To reset a variable

```python
# Placeholder until we know the winner
race_winner = None

# Later in the program...
race_winner = "Arjun"
print(race_winner)
```

---

## 5.6 type() Function

`type()` tells you what data type a variable is.

```python
age = 25
height = 5.9
name = "Arjun"
active = True
nothing = None

print(type(age))
print(type(height))
print(type(name))
print(type(active))
print(type(nothing))
```

Output:
```
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
<class 'NoneType'>
```

### Checking Types in Real Code

```python
score = 95
print("Score:", score, "| Type:", type(score))

price = 99.99
print("Price:", price, "| Type:", type(price))

product = "Laptop"
print("Product:", product, "| Type:", type(product))
```

Output:
```
Score: 95 | Type: <class 'int'>
Price: 99.99 | Type: <class 'float'>
Product: Laptop | Type: <class 'str'>
```

---

## Data Types Summary Table

|
 Type 
|
 Example 
|
 Used For 
|
|
------
|
---------
|
---------
|
|
 int 
|
`42`
, 
`-7`
, 
`0`
|
 Counting, ages, years 
|
|
 float 
|
`3.14`
, 
`-0.5`
|
 Measurements, prices 
|
|
 str 
|
`"Hello"`
, 
`'abc'`
|
 Names, messages, text 
|
|
 bool 
|
`True`
, 
`False`
|
 On/off, yes/no decisions 
|
|
 None 
|
`None`
|
 Empty/missing values 
|

---

## Common Mistakes — Data Types

```python
# MISTAKE 1: Confusing string numbers with actual numbers
age = "20"      # This is TEXT, not a number!
age + 5         # ❌ TypeError: can't add string and int

# MISTAKE 2: Lowercase true/false
active = true   # ❌ NameError
active = True   # ✅

# MISTAKE 3: Confusing None with "None"
result = None   # ✅ The actual None value
result = "None" # This is a string containing the word None

# MISTAKE 4: Using = instead of == for comparison
if x = 5:       # ❌ SyntaxError (= is assignment, not comparison)
if x == 5:      # ✅
```

---

## Practice Exercises — Data Types

1. Create one variable of each type (int, float, str, bool, None). Print each with its type.
2. What is `type(3.0)`? Is it int or float? Test and explain.
3. What is `type("123")`? Test it.
4. Create a variable `is_sunny = True`. Print it. Then reassign it to `False`. Print again.
5. Try `print("Hello" * 3)`. What happens? What about `print("Hello" + 3)`? Note the error.

---

# CHAPTER 6: Type Conversion

---

## WHY do we need type conversion?

The user enters their age in the terminal. Python receives ALL input as TEXT (string). But you need to DO MATH with the age (calculate birth year, for example). You can't do math on text! You need to CONVERT it from string to integer first.

Type conversion (also called type casting) is changing data from one type to another.

---

## 6.1 int() — Convert to Integer

```python
# String to int
age_text = "25"
age_number = int(age_text)
print(age_number + 5)    # Now we can do math!

# Float to int (truncates decimal — doesn't round!)
price = 9.99
whole_price = int(price)
print(whole_price)       # 9 (not 10!)

# Bool to int
print(int(True))         # 1
print(int(False))        # 0
```

Output:
```
30
9
1
0
```

### What int() CANNOT do

```python
int("hello")     # ❌ ValueError — "hello" is not a number
int("3.14")      # ❌ ValueError — int() can't convert decimal strings
int(None)        # ❌ TypeError
```

---

## 6.2 float() — Convert to Float

```python
# String to float
price_text = "29.99"
price = float(price_text)
print(price + 10)        # 39.99

# Int to float
age = 25
age_float = float(age)
print(age_float)         # 25.0

# String int to float
num = float("100")
print(num)               # 100.0

# Bool to float
print(float(True))       # 1.0
print(float(False))      # 0.0
```

Output:
```
39.99
25.0
100.0
1.0
0.0
```

---

## 6.3 str() — Convert to String

```python
# Int to string
age = 25
age_text = str(age)
print("I am " + age_text + " years old")

# Float to string
pi = 3.14
print("Pi is " + str(pi))

# Bool to string
flag = True
print("Status: " + str(flag))

# None to string
nothing = None
print("Value: " + str(nothing))
```

Output:
```
I am 25 years old
Pi is 3.14
Status: True
Value: None
```

---

## 6.4 bool() — Convert to Boolean

This is very important! Python has rules about what counts as "truthy" and "falsy":

**Falsy values (convert to False):**
- `0` (zero integer)
- `0.0` (zero float)
- `""` (empty string)
- `None`

**Everything else is Truthy (converts to True)**

```python
print(bool(0))        # False
print(bool(1))        # True
print(bool(-5))       # True (any non-zero number)
print(bool(""))       # False (empty string)
print(bool("hello"))  # True (non-empty string)
print(bool(None))     # False
print(bool(0.0))      # False
print(bool(0.1))      # True
```

Output:
```
False
True
True
False
True
False
False
True
```

---

## Type Conversion Summary Table

|
 From\To 
|
 int() 
|
 float() 
|
 str() 
|
 bool() 
|
|
---------
|
-------
|
---------
|
-------
|
--------
|
|
 int 5 
|
 — 
|
 5.0 
|
 "5" 
|
 True 
|
|
 float 3.7 
|
 3 (truncates!) 
|
 — 
|
 "3.7" 
|
 True 
|
|
 str "10" 
|
 10 
|
 10.0 
|
 — 
|
 True 
|
|
 str "" 
|
 ❌ Error 
|
 ❌ Error 
|
 — 
|
 False 
|
|
 bool True 
|
 1 
|
 1.0 
|
 "True" 
|
 — 
|
|
 None 
|
 ❌ Error 
|
 ❌ Error 
|
 "None" 
|
 False 
|

---

## Common Mistakes — Type Conversion

```python
# MISTAKE 1: Expecting int() to round
print(int(9.9))    # ❌ Gives 9, NOT 10! int() truncates (cuts off decimal)
                   # Use round() if you want rounding

# MISTAKE 2: Converting a decimal string with int()
int("3.14")        # ❌ ValueError! Must do: int(float("3.14"))

# MISTAKE 3: Thinking "0" is False
bool("0")          # ✅ This is TRUE! "0" is a non-empty string!
bool(0)            # This is FALSE (the actual number zero)
```

---

## Practice Exercises — Type Conversion

1. Convert `"2024"` to an integer and add 1 to it. Print the result.
2. Convert `42` to a string. Print it with a sentence: `"The answer is 42"`.
3. Convert `"3.99"` to float and multiply by 2.
4. What is `bool("False")`? (Be careful — test it and explain!)
5. Try converting `"hello"` to int. What error do you get?

---

# CHAPTER 7: Input

---

## WHY do we need input?

Until now, all your programs have had values already written in the code. But real programs need to respond to the USER. A calculator needs to know what numbers YOU want to calculate. A login system needs YOUR username and password. `input()` is how Python asks the user for information.

---

## 7.1 The input() Function

`input()` pauses your program, shows a message to the user, waits for them to type something and press Enter, then returns what they typed AS A STRING.

### Syntax

```python
variable = input("Message to show user: ")
```

### Examples

```python
name = input("What is your name? ")
print("Hello,", name)
```

When you run this:
```
What is your name? Arjun
Hello, Arjun
```

```python
city = input("Which city are you from? ")
print(city, "is a great city!")
```

```
Which city are you from? Hyderabad
Hyderabad is a great city!
```

---

## 7.2 CRITICAL: input() ALWAYS Returns a String

This is the most important thing to remember about `input()`.

```python
age = input("Enter your age: ")
print(type(age))
```

If user types `20`:
```
Enter your age: 20
<class 'str'>
```

Even though the user typed a number, Python gives you the string `"20"`, NOT the integer `20`.

### Problem this causes:

```python
age = input("Enter age: ")
next_year = age + 1    # ❌ TypeError! Can't add string and int
```

### Solution: Convert immediately!

```python
age = int(input("Enter age: "))
next_year = age + 1
print("Next year you'll be:", next_year)
```

Output:
```
Enter age: 20
Next year you'll be: 21
```

---

## 7.3 Converting Input — Real Examples

### Integer Input

```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
total = num1 + num2
print("Sum:", total)
```

```
Enter first number: 15
Enter second number: 25
Sum: 40
```

### Float Input

```python
price = float(input("Enter item price: "))
quantity = int(input("How many items? "))
total = price * quantity
print("Total cost:", total)
```

```
Enter item price: 29.99
How many items? 3
Total cost: 89.97
```

### String Input (no conversion needed)

```python
name = input("Enter your name: ")
favourite_color = input("Favourite color: ")
print(name + "'s favourite color is " + favourite_color)
```

```
Enter your name: Arjun
Favourite color: blue
Arjun's favourite color is blue
```

---

## 7.4 Multiple Inputs

### Method 1: Separate input() calls

```python
print("Enter your details:")
name = input("Name: ")
age = int(input("Age: "))
city = input("City: ")

print("\n--- Your Profile ---")
print("Name:", name)
print("Age:", age)
print("City:", city)
```

Output:
```
Enter your details:
Name: Arjun
Age: 20
City: Hyderabad

--- Your Profile ---
Name: Arjun
Age: 20
City: Hyderabad
```

### Method 2: Multiple values on one line (split)

```python
# User types: 10 20 30 (space-separated)
a, b, c = input("Enter 3 numbers: ").split()
print(a, b, c)
```

```
Enter 3 numbers: 10 20 30
10 20 30
```

With conversion:
```python
a, b = map(int, input("Enter two numbers: ").split())
print("Sum:", a + b)
```

```
Enter two numbers: 15 25
Sum: 40
```

> **Note:** `map()` and `split()` are functions you'll learn in more detail later. For now, just know this pattern exists — it's extremely common in competitive programming!

---

## Common Mistakes — Input

```python
# MISTAKE 1: Not converting input to int for math
age = input("Age: ")
print(age + 1)       # ❌ TypeError

age = int(input("Age: "))
print(age + 1)       # ✅

# MISTAKE 2: User enters non-number when int() expected
age = int(input("Enter age: "))
# User types "twenty" → ❌ ValueError: invalid literal for int()

# MISTAKE 3: Wrong conversion type
price = int(input("Price: "))
# User types "29.99" → ❌ ValueError (int() can't handle decimal strings)
price = float(input("Price: "))  # ✅
```

---

## Practice Exercises — Input

1. Ask the user for their name and age. Print: `"Hi [name], you were born in [birth year]!"` (calculate birth year by subtracting age from 2024)
2. Ask for length and width. Calculate and print the area of a rectangle.
3. Ask for a temperature in Celsius. Convert to Fahrenheit: `F = (C × 9/5) + 32`. Print the result.
4. Ask for two numbers and print their sum, difference, and product.
5. Ask for the user's name and print it 3 times using `*` repetition.

---

# CHAPTER 8: Arithmetic Operators

---

## WHY learn arithmetic operators?

Operators are the heart of ALL computation. Without them, your program can't calculate anything. DSA problems almost always involve some calculation — finding averages, checking if a number is divisible, computing power — all of that uses arithmetic operators. Master these completely.

---

## The Operators Overview

|
 Operator 
|
 Name 
|
 Example 
|
 Result 
|
|
----------
|
------
|
---------
|
--------
|
|
`+`
|
 Addition 
|
`10 + 3`
|
`13`
|
|
`-`
|
 Subtraction 
|
`10 - 3`
|
`7`
|
|
`*`
|
 Multiplication 
|
`10 * 3`
|
`30`
|
|
`/`
|
 Division 
|
`10 / 3`
|
`3.333...`
|
|
`//`
|
 Floor Division 
|
`10 // 3`
|
`3`
|
|
`%`
|
 Modulus 
|
`10 % 3`
|
`1`
|
|
`**`
|
 Exponentiation 
|
`10 ** 3`
|
`1000`
|

---

## 8.1 Addition (+)

```python
a = 15
b = 7

result = a + b
print("Sum:", result)

print(100 + 200)
print(-5 + 3)
print(1.5 + 2.5)
```

Output:
```
Sum: 22
300
-2
4.0
```

### String Concatenation with +

```python
first = "Hello"
second = " World"
print(first + second)    # Hello World
```

---

## 8.2 Subtraction (-)

```python
marks_total = 500
marks_lost = 75
final_marks = marks_total - marks_lost
print("Final marks:", final_marks)

print(100 - 30)
print(-10 - 5)
```

Output:
```
Final marks: 425
70
-15
```

---

## 8.3 Multiplication (*)

```python
price = 49.99
quantity = 5
total = price * quantity
print("Total:", total)

print(6 * 7)
print(2 * -3)
print(1.5 * 4)
```

Output:
```
Total: 249.95
42
-6
6.0
```

---

## 8.4 Division (/)

Regular division. **ALWAYS returns a float** — even if the answer is a whole number!

```python
print(10 / 2)     # 5.0 (not 5!)
print(10 / 3)     # 3.3333333333333335
print(7 / 2)      # 3.5
print(1 / 4)      # 0.25
```

Output:
```
5.0
3.3333333333333335
3.5
0.25
```

---

## 8.5 Floor Division (//)

Divides and then FLOORS (rounds DOWN to nearest whole number). Returns an int if both operands are ints.

```python
print(10 // 3)     # 3 (not 3.33)
print(7 // 2)      # 3 (not 3.5)
print(9 // 3)      # 3
print(-7 // 2)     # -4 (floors towards negative infinity!)
```

Output:
```
3
3
3
-4
```

### Real-World Use Cases

```python
# How many full teams of 5 can we make from 23 students?
students = 23
team_size = 5
full_teams = students // team_size
print("Full teams:", full_teams)   # 4

# How many pages? (200 items, 10 per page)
total_items = 200
per_page = 10
pages = total_items // per_page
print("Pages:", pages)             # 20
```

---

## 8.6 Modulus (%)

Returns the **REMAINDER** after division. This is extremely important in DSA!

```python
print(10 % 3)    # 1  (10 = 3*3 + 1, remainder is 1)
print(7 % 2)     # 1  (7 = 2*3 + 1)
print(9 % 3)     # 0  (9 = 3*3 + 0, no remainder)
print(5 % 10)    # 5  (5 = 10*0 + 5)
```

Output:
```
1
1
0
5
```

### 🌟 DSA Gold Mine: Uses of Modulus

```python
# CHECK if a number is even or odd
number = 42
if number % 2 == 0:
    print(number, "is Even")
else:
    print(number, "is Odd")
```

```
42 is Even
```

```python
# Extract last digit of any number
number = 12345
last_digit = number % 10
print("Last digit:", last_digit)   # 5
```

```python
# Check divisibility
year = 2024
if year % 4 == 0:
    print(year, "is a leap year (could be)")
```

```python
# Wrap around (useful in circular arrays, clock problems)
hour = 23
next_hour = (hour + 1) % 24
print("Next hour:", next_hour)    # 0 (midnight)
```

**Memory Tip 🧠:** `%` = "what's left over?" If `a % b == 0`, then `b` divides `a` perfectly.

---

## 8.7 Exponentiation (**)

Raises a number to a power.

```python
print(2 ** 3)      # 8  (2 × 2 × 2)
print(5 ** 2)      # 25 (5 × 5)
print(10 ** 6)     # 1000000
print(2 ** 10)     # 1024
print(4 ** 0.5)    # 2.0 (square root!)
print(27 ** (1/3)) # 3.0 (cube root!)
```

Output:
```
8
25
1000000
1024
2.0
3.0
```

### 🌟 DSA Use: Powers of 2

```python
# These numbers are EVERYWHERE in computer science
for i in range(11):
    print(f"2^{i} = {2 ** i}")
```

Output:
```
2^0 = 1
2^1 = 2
2^2 = 4
2^3 = 8
2^4 = 16
2^5 = 32
2^6 = 64
2^7 = 128
2^8 = 256
2^9 = 512
2^10 = 1024
```

---

## Operator Precedence (BODMAS / PEMDAS)

When multiple operators are in one expression, Python follows this order:

```
1. ()   → Parentheses first
2. **   → Exponentiation
3. * / // %  → Multiplication, Division, Floor Division, Modulus (left to right)
4. + -  → Addition and Subtraction (left to right)
```

### Examples

```python
result = 2 + 3 * 4
print(result)    # 14 (not 20! Multiplication first)

result = (2 + 3) * 4
print(result)    # 20 (parentheses first)

result = 2 ** 3 + 1
print(result)    # 9 (2³ = 8, then 8 + 1 = 9)

result = 10 - 3 + 2
print(result)    # 9 (left to right: 10-3=7, 7+2=9)
```

Output:
```
14
20
9
9
```

**Memory Tip 🧠:** When in doubt, use parentheses! `(2 + 3) * 4` is clearer than relying on precedence rules.

---

## Augmented Assignment Operators

Shorthand for common patterns:

|
 Shorthand 
|
 Equivalent 
|
|
-----------
|
-----------
|
|
`x += 5`
|
`x = x + 5`
|
|
`x -= 3`
|
`x = x - 3`
|
|
`x *= 2`
|
`x = x * 2`
|
|
`x /= 4`
|
`x = x / 4`
|
|
`x //= 3`
|
`x = x // 3`
|
|
`x %= 7`
|
`x = x % 7`
|
|
`x **= 2`
|
`x = x ** 2`
|

```python
score = 100
score += 50    # score is now 150
print(score)

score -= 20    # score is now 130
print(score)

score *= 2     # score is now 260
print(score)
```

Output:
```
150
130
260
```

---

## Practical Program — Simple Calculator

```python
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print("\n--- Results ---")
print("Addition:       ", num1 + num2)
print("Subtraction:    ", num1 - num2)
print("Multiplication: ", num1 * num2)
print("Division:       ", num1 / num2)
print("Floor Division: ", num1 // num2)
print("Modulus:        ", num1 % num2)
print("Power:          ", num1 ** num2)
```

Output (for inputs 10 and 3):
```
Enter first number: 10
Enter second number: 3

--- Results ---
Addition:        13.0
Subtraction:     7.0
Multiplication:  30.0
Division:        3.3333333333333335
Floor Division:  3.0
Modulus:         1.0
Power:           1000.0
```

---

## Common Mistakes — Arithmetic Operators

```python
# MISTAKE 1: Expecting / to return int
print(10 / 2)    # Gives 5.0, not 5!
print(10 // 2)   # Gives 5 (use // for integer division)

# MISTAKE 2: Division by zero
print(10 / 0)    # ❌ ZeroDivisionError!

# MISTAKE 3: Operator precedence confusion
print(2 + 3 * 4)    # 14, not 20
print((2 + 3) * 4)  # 20 — use parentheses to be safe

# MISTAKE 4: Using ^ for power (^ is XOR in Python, not power!)
print(2 ^ 3)     # ❌ Gives 1 (bitwise XOR), NOT 8
print(2 ** 3)    # ✅ Gives 8 (use ** for power)

# MISTAKE 5: Negative modulus confusion
print(-7 % 3)    # 2 in Python (might be -1 in other languages!)
```

---

## Practice Exercises — Arithmetic Operators

1. Calculate: `(5 + 3) * 2 - 4 / 2 + 1`. First predict the answer, then verify with Python.
2. A cinema has 350 seats. If a ticket costs ₹250, calculate total revenue for a full show.
3. Write a program that takes a number from the user and checks whether it's even or odd (hint: use `%`).
4. Calculate the area and perimeter of a circle given radius (use pi = 3.14159). Area = πr², Perimeter = 2πr
5. You have 500 chocolates to distribute equally among 23 students. How many does each student get? How many are left over? (Use `//` and `%`)
6. A bank offers 7% simple interest per year. User enters principal and years. Calculate the final amount.
7. What is `3 ** 3 ** 2`? Is it `(3**3)**2 = 729` or `3**(3**2) = 19683`? Test and explain.

---

# WEEK 1 — REVISION SHEET

---

## Quick Reference — All Topics

### 1. Core Concepts
```
Programming   = Instructions for computers
Python        = Beginner-friendly interpreted language
Interpreter   = Translates code line-by-line (Python's method)
Source Code   = The .py file you write
RAM           = Temporary memory for running programs
```

### 2. print()
```python
print("text")                    # Basic
print("a", "b", sep="-")         # Custom separator → a-b
print("hi", end=" ")             # Custom line ending
print("Line1\nLine2")            # Newline with \n
print("Tab\there")               # Tab with \t
# This is a comment
```

### 3. Variables
```python
name = "Arjun"        # String
age = 20              # Integer
height = 5.9          # Float
active = True         # Boolean
nothing = None        # None

a, b = b, a           # Swap (Pythonic one-liner)
x = y = z = 0         # Multiple assignment
```

### 4. Data Types
```python
type(42)       → 
type(3.14)     → 
type("hi")     → 
type(True)     → 
type(None)     → 
```

### 5. Type Conversion
```python
int("25")      → 25
int(9.9)       → 9      # Truncates! Not rounds
float("3.14")  → 3.14
str(42)        → "42"
bool(0)        → False
bool("")       → False
bool(1)        → True
bool("hello")  → True
```

### 6. Input
```python
name = input("Name: ")              # Always returns string
age = int(input("Age: "))           # Convert to int
price = float(input("Price: "))     # Convert to float
a, b = map(int, input().split())    # Two ints on one line
```

### 7. Arithmetic Operators
```python
+   → Addition         10 + 3  = 13
-   → Subtraction      10 - 3  = 7
*   → Multiplication   10 * 3  = 30
/   → Division         10 / 3  = 3.333...
//  → Floor Division   10 // 3 = 3
%   → Modulus          10 % 3  = 1
**  → Exponentiation   10 ** 3 = 1000
```

---

## Key Things to Remember

1. `input()` ALWAYS returns a string — convert it!
2. `/` always returns float; use `//` for integer division
3. `**` is power, NOT `^` (which is XOR!)
4. `=` is assignment; `==` is comparison
5. `True` and `False` are capitalized
6. `int()` truncates, it does NOT round
7. `bool(0)`, `bool("")`, `bool(None)` are all `False`
8. Variable names are case-sensitive: `Age` ≠ `age`

---

# WEEK 1 — 25 PRACTICE QUESTIONS

---

## Beginner Level (Questions 1-10)

**Q1.** Write a program that prints the following pattern using escape sequences:
```
Name:   Arjun Kumar
Age:    20
City:   Hyderabad
```

**Q2.** Create variables for: your name (str), favourite number (int), your GPA (float), are you a student (bool). Print all of them with their types using `type()`.

**Q3.** Ask the user for their first name and last name separately. Print their full name combined.

**Q4.** What will this print? Predict FIRST, then run it:
```python
x = 5
x = x + 3
x = x * 2
print(x)
```

**Q5.** What is the output?
```python
print("Go" * 3, end="! ")
print("You", "can", "do", "it", sep="-")
```

**Q6.** A movie ticket costs ₹180. Popcorn costs ₹60. A couple goes to the movies. Write a program to calculate the total cost.

**Q7.** Convert `"3.14"` to a float. Multiply it by 2. Print the result.

**Q8.** Ask the user for a number. Print whether it is even or odd. (Hint: use `%`)

**Q9.** What is the difference between `/` and `//`? Show with an example using 17 and 5.

**Q10.** Swap these two variables WITHOUT a third variable: `p = "apple"` and `q = "orange"`.

---

## Intermediate Level (Questions 11-20)

**Q11.** Write a program: Ask the user for marks in 5 subjects (each out of 100). Calculate and print the total and percentage.

**Q12.** Ask for a temperature in Fahrenheit. Convert to Celsius: `C = (F - 32) × 5/9`. Print with 2 decimal format using round().

**Q13.** What is `bool("0")`? What is `bool(0)`? Why are they different?

**Q14.** Write a program to find the area of a triangle given base and height. `Area = 0.5 × base × height`

**Q15.** What will this output? Predict first:
```python
print(2 ** 3 ** 2)
```
Is it `(2**3)**2 = 64` or `2**(3**2) = 512`? Explain why.

**Q16.** A shop offers 15% discount on total purchase. Ask for original price. Calculate and print discounted price.

**Q17.** Write a program to check if a year is a potential leap year (divisible by 4). (Full leap year logic is more complex, but use `% 4 == 0` for now)

**Q18.** Ask for a 3-digit number. Extract and print its hundreds, tens, and units digits.
> Hint: For 347 → hundreds = 347 // 100 = 3, tens = (347 // 10) % 10 = 4, units = 347 % 10 = 7

**Q19.** Predict the output, then verify:
```python
a = 10
b = 3
print(a // b, a % b, a / b)
print(type(a // b), type(a / b))
```

**Q20.** Write a program: Ask for a principal amount, interest rate (%), and number of years. Calculate Simple Interest and final amount.
`SI = (P × R × T) / 100`

---

## Challenge Level (Questions 21-25)

**Q21.** You have N apples and want to pack them in boxes of 12. Ask the user for N. Print how many full boxes you can make and how many apples are left over.

**Q22.** Ask the user for a number of seconds. Convert it to hours, minutes, and seconds and print it in format `HH:MM:SS`.
> Hint: 3661 seconds = 1 hour, 1 minute, 1 second

**Q23.** A student scores marks in 3 subjects: Physics, Chemistry, Math. Each has a weightage: Physics = 40%, Chemistry = 30%, Math = 30%. Ask for marks in each (out of 100) and calculate the weighted final score.

**Q24.** Write a digit reversal program: Ask for a 4-digit number. Reverse its digits and print. (e.g., 1234 → 4321)
> Hint: Use `%` and `//` operators

**Q25.** The distance between two cities is `d` km. A car's fuel efficiency is `e` km/litre. Fuel costs ₹`p` per litre. Ask the user for d, e, and p. Calculate the total fuel cost for the trip.

---

> **Answers are intentionally not provided** — the struggle of solving them yourself is where the REAL learning happens. Show your solutions to a mentor or check them by running in Python.

---

## How to Study This Guide Effectively

1. **Read first, then type** — Never copy-paste code. Type every example yourself.
2. **Make mistakes on purpose** — Try the "wrong" versions to see what errors look like.
3. **Modify examples** — Change values, try different inputs. Curiosity builds understanding.
4. **Do practice questions** — Reading without doing = 0% retention.
5. **Teach someone else** — If you can explain it to a friend, you truly understand it.

---

> **Week 1 Complete! You have covered the foundation of ALL Python programming.**
> Next Week: Conditions (if/elif/else), Loops (for, while), and Lists.
> Keep going. Every expert was once exactly where you are now. 🐍🚀
