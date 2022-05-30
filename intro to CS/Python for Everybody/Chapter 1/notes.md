# Chapter 1

## Reserved words in Python

False
None
True
And
As
Assert
Break
Class
If
Def
Del
Elif
Else
Except
Return
For
From
Global
Try
Import
In
Is
Lambda
While
Not
Or
Pass
Raise
Finally
Continue
Nonlocal
With
Yield

each of this words contain a purpose that is exclusively for python. Which is why we can't use it for our own purpose other than what purpose python already set.

## Statement and Assignment

```python
x = 2 
# this is an assignment
# x is a variable
# = is an operator for assignment
# 2 is a consstant value

x = x + 2
print(x)
# print is a statement
```

## Program steps and flow

-   like a receipt / instruction, a program is a sequence of steps to be done in order
-   some steps are conditional and can be skipped
-   some steps need to be repeated
-   and some steps need to be used over and over again as needed several times or places throughout  the program

### Sequentional steps

really straight forward and only run in one way

```python
x = 2
x = x + 2
print(x)
```


### Conditional steps

steps that will run if condition are met, and skipped if condition are not met.

```python
x = 5

if(x = 5)
    print(x)
```

### Repeated steps

steps that will be repeated if the conditioned are met and ussually have exit conditioned (if not it will run forever, infinite loop) that will exit the repeated process.

```python
x = 5

while x > 0 
    print(x)
    x = x - 1

print("done")
```