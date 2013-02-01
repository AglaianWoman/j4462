# Getting started with Python

Python is a rich and fully featured language that can be used for almost any application you can imagine, from building websites to running robots. A thorough overview of the language would take weeks or months, so our class is going to concentrate on the absolute basics -- basic programming principles and syntax quirks that you're likely to encounter as you start to program in Django. This isn't intended to be a comprehensive Python tutorial. It's only meant to give you the basic skills you'll need to succeed in this course. That said, I would highly encourage you to explore the language further and will provide materials to do so at the end of this guide.

## How to run a Python program

Most Python code is run directly from the command line, which explains why it is so important that you master some command line basics. Recall from the [command line tutorial](https://github.com/cjdd3b/j4462/blob/master/python-basics/command-line-basics.md) that Python files have the file extension ".py". Any time you see a ".py" file, you can run it from the command line simply by typing ```python filename.py```, where filename is the name of whatever the file is. That's it. And it works for both OSX and Windows.

Python also comes with a very neat feature called an **interactive interpreter**, which essentially allows you to execute Python code one line at a time, sort of like working from the command line. We'll be using this a lot in the beginning to demonstrate concepts, but in the real world it's often useful for testing and debugging. To open the interpreter, simply type ```python``` from your command line, and you should see a screen that looks like this:

IMAGE

We'll get into more detail about that later.

## Programming basics

No matter whether you're working in Python or another language, there are a handful of basic concepts you need to understand if you're going to be writing code. We'll walk through those here.

### Variables

Variables are like containers that hold different types of data so you can go back and refer to them later. They're fundamental to programming in any language, and you'll use them all the time. Here's an example

```
greeting = "Hello, world!"
print greeting
```

In this case, we've created a **variable** called ```greeting``` and assigned it the **string value** "Hello, world!". If we use the ```print``` command on the variable, Python will output "Hello, world!" to the terminal because that value is stored in the variable.

In Python, variable assignment is done with the = sign. On the left is the name of the variable you want to create (it can be anything) and on the right is the value that you want to assign to that variable. Variables can also contain many different kinds of data types, which we'll go over next:

### Data types

You may remember from earlier data journalism classes that data comes in different types and flavors. There are integers, strings, floating point numbers (decimals), and other types of data that languages like SQL like to deal with in different ways. Python is no different. In particular, there are six different data types you will be dealing with on a regular basis: strings, integers, floats, lists, tuples and dictionaries. Here's a little detail on each.

**Strings**: Strings contain text values like the "Hello, world!" example above. There's not much to say about them other than that **they are declared within single or double quotes** like so:

```
greeting = "Hello, world!"
goodbye = "Seeya later, dude."
favorite_animal = 'Donkey'
```
Note that either single or double quotes are allowed.

**Integers**: Integers are whole numbers like 1, 2, 1000 and 1000000. They do not have decimal points. Unlike many other variable types, **integers are not declared with any special type of syntax**. You can simply assign them to a variable straight away, like this:

```
a = 1
b = 2
c = 1000
```

**Floats**: Floats are a fancy name for numbers with decimal points in them. **They are declared the same way as integers** but have some idiosyncracies we'll discover later:

```
a = 1.1
b = 0.99332
c = 100.123
```

**Lists**: Lists are collections of values or variables. **They are declared with brackets like these [], and items inside are separated by commas**. They can hold collections of any type of data, including other lists. Here are several examples:

```
list_of_numbers = [1, 2, 3, 4, 5]
list_of_strings = ['a', 'b', 'c', 'd']
list_of_both = [1, 'a', 2, 'b']
list of lists = [[1, 2, 3], [4, 5, 6], ['a', 'b', 'c']]
```

**Tuples**: Tuples are a special type of list that cannot be changed once it is created. That's not especially important right now. All you need to know is that **they are declared with parentheses ()**. For now, just think of them as lists.

```
tuple_of_numbers = (1, 2, 3, 4, 5)
tuple_of_strings = ('a', 'b', 'c', 'd')
```
