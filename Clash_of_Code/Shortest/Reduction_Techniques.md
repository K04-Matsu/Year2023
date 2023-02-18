## CoC, Shortest Mode
#### During our IB DP year 2, every class we started our class with a competitive coding game "Clash of Codes(CoC)". "Shortest" was one of the game modes that are included in the CoC, and the purpose of this mode is to solve the problem using minimal code length as possible. In order to do so, students were required to improve their skills in reducing the code length through learning some techniques.
#### Below are some of the techniques we learned throughout 

### Variable Grouping
Instead of:
```.py
variable1 = "Hello "
variable2 = "World"
variable3 = "!"
print(variable1+variable2+variable3)

# Output:
""" Hello World! """
```

We can group the variable:
```.py
variable1, variable2, variable3 = "Hello ", "World", "!"
print(variable1+variable2+variable3)

# Output:
""" Hello World! """
```

### Ternary operators
Instead of:
```.py
variable1 = input()
if condition == 0:
    expression = 100
else:
    expression = 5
```

We can use Ternary operators to one-line it:
```.py
variable1 = input()
expression = 100 if variable1 == 0 else 5 # expression = 5
```

### List comprehension
Instead of:
```.py
list_of_squares = []
for item in range(10):
    list_of_squares.append(item**2)
print(list_of_squares)
#Output
""" [0, 1, 4, 9, 16, 25, 36, 49, 64, 81] """
```

We can use list comprehension to create the list in one line:
```.py
list_of_squares = [item ** 2 for item in range(10)]
print(list_of_squares)
#Output
""" [0, 1, 4, 9, 16, 25, 36, 49, 64, 81] """
```
Another example is,
Instead of:
```.py
for item in list_of_squares:
    if (item % 2) == 0:
        list_of_squares.remove(item)
print(list_of_squares)

#Output:
""" [1, 9, 25, 49, 81] """
```

We can use list comprehension to one-line both loop and if-statement:
```.py
[list_of_squares.remove(item) for item in list_of_squares if (item % 2) == 0]
print(list_of_squares)

#Output:
""" [1, 9, 25, 49, 81] """
```

### Nested Functions
Instead of:
```.py
variable = input()
variable = float(variable)
variable = round(variable)
print(variable)

#Input(1.618)
#Output:
""" 2 """
```

We can nest the functions:
```.py
print(round(float(input())))

#Input(1.618)
#Output:
""" 2 """
```

### Rewriting function names
Instead of:
```.py
var1 = round(float(input()))
var2 = round(float(input()))
var3 = round(float(input()))
print(var1+var2+var3)
```
We can rewrite the name of the functions:
```.py
r = round
f = float
i = input
var1 = r(f(i()))
var2 = r(f(i()))
var3 = r(f(i()))
print(var1+var2+var3)
```

