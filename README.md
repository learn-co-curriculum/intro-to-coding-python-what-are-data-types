# What are Data Types?

## Learning Goals

- Explain data type.
- Create common data type representations in Python.

## Introduction

A computer does not understand information like humans do. For example when we
look at a text or string like `Hi! My name is Al!` or a number like `10`, we can
distinguish between them easily. We understand that strings and numbers have
different properties and are used in various contexts.

The computer cannot distinguish between different types of information
automatically. There are unique ways to represent values so that the computer
can differentiate them. Each unique type of value is assigned a “data type” to
classify or organize them, allowing us to know what contexts a certain value can
be used.

## The Common Data Types in Python

We will look at the most common data types used in Python:

- `str`: Represents text or string values.
- `int`: Represents integer number values (whole numbers like `1`, `5`.
- `float`: Represents floating-point numbers (decimal numbers like `1.556`,
  `3.14`).
- `bool`: Represents the idea of correctness, i.e., whether something is true or
  false.

## String Values

We use the values of the `str` data type to represent textual information to the
computer. The first Python program we ran displayed the text “Hello, world!” in
the console. We saw how trying to display the words without the quotation marks
caused an error.

In most programming languages, we use `''` (single quotation marks) or `""`
(double quotation marks) to represent strings or textual information. Here are
some examples in Python (remember to run code examples in the code editor!):

```python
print("") # empty string
print("one") # one word
print("1") # this is still a string!
print("This is a string") # multi-word string
print("I'm learning Python!") # using both single and double quotations
```

Here’s the output of the above code:

```
one
1
This is a string
I'm learning Python!
```

A few things to note:

- The text is displayed exactly as it is written, i.e., the string values are
  case-sensitive.
- Numbers wrapped in quotation marks are treated as strings.
- Single and double quotations can be used together. The opening and closing
  quotation marks must be the same. For example, we can’t start a string with a
  `"` and close it with a `'`.

## Observing the Type of a Value

Python provides us with a `type` function to determine the data type of a value.
Here’s how we can use it:

```python
print(type("Hello!"))
```

Here’s the output:

```python
<class 'str'>
```

A couple things to note:

- We can ignore the `class` keyword for now.
- The data type is displayed right after the `class` keyword. It is telling us
  that the value `"Hello!"` has a data type of `str`.

## Numbers

When we ran the code `print("1")` the type was listed as `str`. So how do we
tell the computer that we want to represent a number?

We can represent numbers by writing them without the quotations. Run the
following code and observe the output:

```python
print(type(1)) # <class 'int'>
print (type(-5)) # <class 'int'>
print(type(-1.5)) # <class 'float'>
print(type(3.1415926535)) # <class 'float'>
```

The output:

```
<class 'int'>
<class 'int'>
<class 'float'>
<class 'float'>
```

A few notes on the code:

- Numbers written without quotations are interpreted as numerical values.
- The `int` data type represents positive and negative whole numbers.
- The `float` data type represents positive and negative decimal numbers.

## Bool

Human languages have the concept of correctness. For example, the sentence
“elephants can fly” is incorrect or false. Similarly, computers also understand
this concept. Programming languages provide a boolean data type (`bool` in
Python) to express this concept.

In Python, the following values represent this concept:

- `True`: indicates correctness in Python.
- `False`: indicates incorrectness in Python.

Here are the values in Python code:

```python
print(True)
print(False)
print(type(True)) # <class 'bool'>
print(type(False)) # <class 'bool'>
```

Output:

```
True
False
<class 'bool'>
<class 'bool'>
```

Note that the values are case-sensitive. They have to be written with the first
letter in uppercase and the rest of it in lowercase. If we wrote `true`,
`false`, or any other variations, it would cause an error.

```python
# wrong code
print(type(true))
```

The above code would raise the following error:

```
Traceback (most recent call last):
  File "main.py", line 2, in <module>
    print(type(true))
NameError: name 'true' is not defined. Did you mean: 'True'?
```

## Conclusion

We have learned about the common data types in Python and how to identify the
data type of a give value by using the `type` function. We will see in the
following lessons how different types of values allow different operations.
