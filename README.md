# 202 The *args parameter

## Objectives
* understanding *args to create functions with list input

In the past, we have seen that a function can be created that accepts input parameters as *positional arguments*.  For example, consider the code below:

```
def functionName(num1,num2):
  pass
  # more code goes here
```

You can see here that the function takes in 2 positional arguments as input parameters, but this function can only accept 2 parameters.  This is great if the input is keeping track of things like the length and width of a rectangle, but what if these are supposed to be scores for a student on a test, or shoe sizes for a classroom?  We would want to be able to keep entering data until we are out of things to enter.

### *args positional argument

One of the ways that we can submit data to a function is to provide it with a list:

```
def functionList(myList):
  pass
  for i in myList:
    print(i)

data = [3,4,5,6,7]
functionList(data)
```

You can see from this example that we can send a variable amount of data to the function if we send it as a list, and then wen can do something with that list in the function itself.  However, **we can also use a variable number of input parameters using the *args parameter**.

```
def functionList(*myList):
  pass
  for i in myList:
    print(i)

data = [3,4,5,6,7]
functionList(3,4,5,6,7)

