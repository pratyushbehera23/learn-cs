# Py

## Basic

- Variables
- Conditions
  - Boolean
  - Chained
- Operators
- Control flow
- Loops and iterations
- Basic Data structures : list,sets,str,..
- Functions
- Mutable and immutable data types
- Common methods
- I/O operations

<!-- Intermediate: -->
- Object oriented class OOPs:
  - Constructor
  - Method
  - Inheritance
  - Encapsulation
  - Polymorphism
- Data structure
- Algorithms
- Comprehensions
- Lambda functions
- Collection, map, filter modules
- *args and **kwargs
- Advanced class behavior
- Dunder methods
- Pip
- Python environments
- Making your own modules
- Async IO (asynchronous program...)

<!-- Advanced: -->
- Decorators
- Generators
- Context managers
- MetaClasses
- Concurrency and Parallelism
- Testing
- Build and manipulate Packages
- Cython

<!-- Master: -->
- ...
- use modules Tensorflow, keras,...

### Py🔍

Software design
Software development
Object oriented programming
Problem solving technique
Threading
Rest api
Machine Learning
Web development
Artificial intelligence
Scripting
...

## Modules/packages/Libraries

- Data Science
  - NumPy (mathematical operations)
  - SciPy
  - Selenium (bot)
  - BeautifulSoup (web scraping, bot)
    Mechanical soup
    Scrappy
    Pandas (organizes manipulates data)
    Matplotlib (scientific graphs & plots)
    Plotly
    Seaborn
    Scikit Learn
    PyCaret
    TensorFlow (ML)
    Keras
    PyTorch (ML)
    PyQt5
    DearPyGUI
    Kivy (mobile development)
    kivyMD (mobile development)
    Django (web development)
    Flask (web development)
- Natural language processing (NLP):
    nltk
    gensim
    flashtext
- Computer vision (CV):
    OpenCV
    SimpleCV
- Graphical user interface (GUI):
    tkinter
    wxPython
    PyQt
elasticsearch
requests
tweepy
textblob
vaderSentiment
newspaper3k

--

flow chart
DFD
UML

Time complexity
Space

System architecture

CPU resistars

```py
# Memory address:
id(var)  # only in python

# If same value in two different variables then it will allocate the same space. # saves memory

"""
Documentation is done inside function using multiple line comment
"""
print(functionName.__doc__)  # to print documentation

# List comprehension in python:
L1 = [x for x in range(100)]
L2 = [x for x in range(50) if x%2 == 0]

# Lambda functions in python:
x = lambda y : y+2
x(4)  # 6

# Map  and  filter
Mylist = [2,43,4,5,125,94,8,30]
Newlist = map(lambda x : x+2, Mylist)

# *args  and  **kwargs
def new_func(*args,**kwargs):
    print(args, kwargs)
new_func("hello", x="Bye")
```
