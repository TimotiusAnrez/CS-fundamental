# Chapter 2: Variables, Expressions and Statements

## Constants

Fixed values such as numbers, characters, and strings are called constants because their value does not change

ie:
-   Numeric constants: 123
-   String constants: "Hello world" / 'Hello from python' (anything inside double quotation or single quotation marks)

## Variables

A variable is a named place in the memory where we store data or value that later will be retrived to be used using the variable name.

We may use whatever name we like other than reserved words to named our variable.

you can change the content of a variable in a later statement.

ie:
```python
x = 2 
y = 3
z = 5

# variable x has a value of 2, y has 3, and z has 5
```

### Variables naming best practice

- Start your variable name with a letter or underscore

- must consist of letters, numbers, and underscore

- Case Sensitives

Good:
    -   spam, egs, spam23, _speed

Bad:
    -   23spam, #sign, var.12

different:
    -   spam Spam SPAM

### Mnemonic Variable Names

since we have the power to name the variable however we like, makes variables names kinda confusing for other people. Hence following best practice will makes it simpler for other people to understand your program.

Name variable that can help us memorize or remember what we inted to do, will not only helping us debugging our program if there is an error or bugs but can also help other people to understand your program better.

ie:
```python
xyq1231 = 1029281.293
xzq1231 = 1029188.293
xqq1231 = 1029199.293
# bad naming since we don't know what this is used for and we a single mistake of calling the wrong variable will lead to a dissaster

print(xzq1231)
# a bug appear if we want to print xyq231 instead of xzq1231

rortation = 102981.293
# this gives us a clue what this value means hence a better variable name

gearA_rotation = 102981.293
# this gives us a better description
```

Chosing a good name will make reader understand your program better.


## Assignment statements

we assign value to a variable using the assignment statement (=)

an assignment statement consists of an expression on the right hand side and a variable to store the result

```python
x = 2
# x value assigned

x = x + 2 / 100 * 25
# x value got reassigned

print(x)
```

## Expressions

Expressions is a more complex calculation

because of the lack of mathematical symbols on computer keyboards we use "computer-speak" to express classic math operations

```
+ = addition
- = substraction
* = multiplication
/ = division
** = power
% = reminder
```

exponentiation (raise to a power) looks different than in math

### Order of Evaluation

When we string operators together - Python must know which one to do first

This is what we call operator precedence

```
-   () always in top priority

-   ** second

-   * , / , %  third

-   + , - last priority

always read left to right
```

## Types

- in Python variables, literals, and constat have a type

- Python knows the difference between an integer number and a string

- Eg. "+" means addition if there is a number on the right side of it, and concatenante (adding character or string to existing strings) if the right side of "+" is a string or character

### Types Matters

```python
eee = 'hello' + 'there'
eee = eee + 1

# will cause typeError 
# reason being because python cannot convert 'int' object to str implicitly

# Traceback error means force exit program because of an error
```

rules: 
-   You Cannot add a number or integer to strings
-   Python have a built in function called type(value)
        -   type built in function will tell python what the value type is

## Several Types of Numbers

Numbers have two main types:
    -   Integers
        
        Integers are whole numbers
            ie: -14, -2, 0, 1, 100, 20020201

    -   Floating Point Numbers

        Float have decimal parts (percision)
            ie: -2.5, 0.5, 1.8, 98.6 

Other number types are variations on floats and integers

### Type Conversions

When you put an integer and floating point in an expression, the integer will implicitly converted to a float

    -   You can control this via built-in functions int() and float()