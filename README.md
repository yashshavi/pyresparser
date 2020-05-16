# Formatting Document #
This document provides the rules for Formatting of code. This document specifies the do's and don'ts for code formatting with the help of examples. The document covers Vertical Formatting, Horizontal Formatting and Liter's used in code for different language.

## Vertical Formatting:
**1. LOC**

LOC in a file should be less than 100.

**2. NewsPaper Metaphor**

Proper name of the files and functions. Name should be able to represent the high level overview of the concepts that
it will be containing.
```bash
""" The following example shows correct usage of NewsPaper Metaphor """
login.py

""" name of the function is giving the high level concept overview
that is the function is used for login
"""

def login(username, password):
    """ do tasks to login""

```

**3. Vertical openness between concepts**

1. Single lineBreak between concepts.
```bash
"""Correct"""
def login(username, password):
    """do tasks"""

def signup():
    """do tasks"""

```
```bash
"""Incorrect"""
def login(username, password):
   """do tasks"""
def signup():
    """do tasks"""
```

2. Single lineBreak before commenting the method.

**4. Vertical Density**

No lineBreak for comments in between method.

```bash
"""Correct"""
def login(username, password):
    status = submit(username, password)
    #check status after submiting uername and password
    if status:
        print('login')
    else :
        print('invalid username or password')
```

```bash
"""Incorrect """
    def login(username, password):
    status = submit(username, password)

    #check status after submiting uername and password

    if status:
        print('login')
    else :
        print('invalid username or password')

```

**5. Variable declaration**
At the top of a module or functions where it will be going to use (for c#)

```
//Example
 public void input():
    int a, int b;
    //do tasks
```


## Horizontal Formatting:
**1. Number of characters**

Number of characters in a single line should not exceed 100.

**2. Horizontal openness and density**

1. one whitespace between operator and operands.

```bash
"""Correct"""
c = a + b
```

```c#
"""Incorrect"""
c=a+b
```

2. one whitespace after comma while declaring multiple variables in a single line.

```c
//Example
int a, b;
```

 3. no whitespace between name of function and parenthesis.
```bash
"""correct"""
    def function_name(arg1, arg2)
```

```python
"""Incorrect"""
def functiona_name ( arg1,arg2)
```

 4. one whitespace after comma in arguments in a function.
```python
"""correct"""
def functiona_name(arg1, arg2)
```

```python
"""Incorrect"""
def functiona_name(arg1,arg2)
```

## Linter and Checkstyle Configuration:
**1. For Python**

Pylint

## contributors
Design - Yashshavi Kashyap
Rules - Anurag sharma, Heena Vasdani, Renu saini, Neha Mathur, Yashshavi Kashyap
