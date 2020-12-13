# Lab #1: The Python Ecosystem

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Goals

## Acknowledgements

Chapter 11 "Debugging" in Automate Boring Stuff (249-266)

Chapter 2 "Variables, Expressions and Statements" in Allen Downey Think Python (11-20)

# Table of Contents

# Different types of Python environments

In the Fall 2020 iteration of Elements I, we used the browser-based IDE [Replit](https://repl.it/).

What is an IDE? "An integrated development environment (IDE) is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of at least a source code editor, build automation tools and a debugger" ([Wikipedia](https://en.wikipedia.org/wiki/Integrated_development_environment)).

An IDE can include features like syntax highlighting, code completion, version control, and debugging.

There are a WIDE range of IDEs that are proprietary or open-source, tailored to a specific language or able to work across languages.

Some common IDEs include Eclipse, Geany, Brackets, Atom, PyCharm, Spyder, RStudio, etc. For more in IDEs, visit Wikipedia's ["Comparison of integrated development environments"](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments) page.

Replit (generally) worked for (most of) our needs in Elements I. But it ran into problems with more complex programs or programs involving external files/datasets/etc. 

So in this semester, we're going to install Python on your local computer, using a distribution called Anaconda.

What is Anaconda? "Anaconda is a open-source distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment. The distribution includes data-science packages suitable for Windows, Linux, and macOS. It is developed and maintained by Anaconda, Inc., which was founded by Peter Wang and Travis Oliphant in 2012" ([Wikipedia](https://en.wikipedia.org/wiki/Anaconda_(Python_distribution))).

The Anaconda environment includes a number of specific tools and programs, including:
- JupyterLab
- Jupyter Notebook
- Qt Console
- Spyder
- Glue
- Orange
- RStudio
- Visual Code Studio

This semester, we'll be using the Jupyter Notebook and Spyder components of Anaconda.

# Installing Anaconda

Windows/PC instructions:
- Anaconda Documentation, ["Installing on Windows"](https://docs.anaconda.com/anaconda/install/windows/) *Anaconda* (2020).
- ProgrammingKnowledge, ["Install Anaconda Python, Jupyter Notebook and Spyder on Windows 10"](https://youtu.be/5mDYijMfSzs) *YouTube video* (4 September 2018).

Mac OS instructions:
- Anaconda Documentation, ["Installing on macOS"](https://docs.anaconda.com/anaconda/install/mac-os/) *Anaconda* (2020).
- Understanding Data, ["Easily Install Anaconda Python Distribution On Mac OS X"](https://youtu.be/V6ZAv7hBH6Y) *YouTube video* (16 October 2019).


Chromebook instructions:
- Alex P. Miller, ["Data Science on a Chromebook: How to run Jupyter, Python, and R locally in ChromeOS"](https://alex.miller.im/posts/data-science-chromebook-pixelbook-jupyter-python-r/) *personal blog* (6 March 2019).
- Noebrian, ["Installing Anaconda on a Chromebook"](https://chromebook.home.blog/2019/01/20/installing-anaconda-on-a-chromebook-no-dev-beta-or-crouton-needed/) *ChromeBooks* (20 January 2019).

<blockquote>QX: Something about installation process in relation to available/provided documentation</blockquote>

# Python in Spyder

"Spyder is a free and open source scientific environment written in Python, for Python, and designed by and for scientists, engineers and data analysts. It features a unique combination of the advanced editing, analysis, debugging, and profiling functionality of a comprehensive development tool with the data exploration, interactive execution, deep inspection, and beautiful visualization capabilities of a scientific package" ([Spyder documentation](https://www.spyder-ide.org/)).

Spyder's core components include:
- Editor
- IPython console
- Variable explorer
- Plots
- Debugger
- Help

These robust Python features in Spyder will be incredibly useful as we start to do more work with datasets, visualizations (plots), and debugging in more complex programming environments.

Open the Anaconda navigator and select the option to launch Spyder.

NOTE: When we were working in Replit, all files that were part of our Python project were in the same virtual workspace. 

That's not going to be the case when working in a desktop IDE like Spyder. 

Think of this as the difference between working with files in Google Drive versus on your local computer. 

You can set a working directory, which is where Spyder will look for external files you are wanting to access from within a Python program. The working directory is also where Python will save `.py` files you build.

Click on the folder icon in the top-right hand corner of Spyder (next to the arrow icon) to set a working directory. It doe--where you save `.py` files and other files (think data files) you might be wanting to access as part of a Python program.

Now, files don't have to be in your current working directory for you to access them in Python. But you'll need to provide the full file path (i.e. location information or directory information for where that file is located on your computer).

Go ahead and create an `EoC_II` folder and set that folder as your working directory in Spyder. It might also be a good idea to start creating lab-specific sub-folders within your `EoC_II` parent folder. 

This will help with organization as we move through labs and work with a variety of sample files and datasets.

Spyder has three default panes that show up when you launch the program.

IMAGE

Your `.py` file shows up on the left-hand side of the program window. This is where you will write Python code. You can have multiple `.py` files open in Spyder and navigate between the tabs. 

The top-right pane has four default options:
- Variable explorer, which lets you see named variables in your program
- Help, which provides additional documentation, information, or resources
- Plots, which will show visualizations generated by your program
- Files, which will show all files currently open or active in your Spyder workspace

The bottom-right pane is the Console, which lets you execute and test Python commands. You can have multiple consoles open simultaneously.

So how is the Console different from your `.py` file?

In the `.py` file you are writing a Python program that will run or execute when the file is called. You make updates to that file, save changes, etc.

The Console lets you execute Python commands but is not saving those commands as part of a `.py` file. 

Great for testing. Less great for building out complex programs.

Work through the ["First Steps with Spyder" resources](https://docs.spyder-ide.org/current/first-steps-with-spyder.html) provided by Spyder. That includes two 3.5 minute videos that introduce you to the basics of the Spyder IDE and how to get started with Python in Spyder.

<blockquote>QX: How is Spyder different than previous IDEs? What do you see as strengths/advantages? What do you see as possible challenges?</blockquote>

<blockquote>OPTIONAL: Take one of your Python files or programs from Elements I and load it into Spyder. Explore how the program runs in a different IDE. In particular, explore Spyder's options to run portions or a selection of the larger program. How does this change the way you interact with the program?</blockquote>

# Debugging

To paraphrase an old programming joke, writing code is 90% of the work of programming. Debugging is the other 90%.

You've been working on a program for hours, your head hurts, and something still isn't working. We all know a version of that feeling.

There's no easy solution that will prevent all problems (or "bugs") in your code. But having strategies for testing your code, recognizing and making sense of error messages, and methodically debugging your code can help immensely.

Python errors will usually fall into three types:
- Syntax: refers to the structure of a program and rules about that structure. Syntax errors involve things like indentation, parenthesis, etc. The Python interpreter expects the language to be structured a specific way, and throws a syntax error when it's not.
- Runtime errors, or exceptions: appears after a program has started running. These errors indicate something unexpected has happened that interrupts or stops the program execution. Things that can cause a runtime error include:
  * Misspelled or incorrectly capitalized variables or function names
  * Dividing by zero
  * Mismatched data types (i.e. attempting to perform operations on data of the wrong type)
  * Attempting to use a type conversion function on a value that can't be converted
- Semantic: relates to meaning. Semantic errors have to do with the meaning (or purpose/intent) of your code. Semantic errors don't show up as error messages-but the program will not do what you expect it to do. 

The debugging strategies discussed here will focus on semantic errors but are useful for all types of errors.

# Step-wise debugging in Spyder

Spyder will catch many syntax and runtime errors. 

Hover over a red `X` by any of your lines of code to see more information about a possible error.

Spyder integrates the enhanced `ipdb` debugger, which gives you robust options for troubleshooting or debugging your code.

Specifically, the debugger will let you run a program line by line, running a single line of code and waiting for you to tell it to continue.

Running your program through this kind of debugging is immensely valuable for tracking down bugs or catching complex issues in a program.

This mode of debugging includes the following possible steps or "moves":
- Continue (run the program until the next breakpoint)
- Step in (executes the next line of code; if the next line of code is a function, the debugger will 'step into' the first line of that function)
- Step over (executes the next line of code, but will not go line-by-line through the function; the debugger 'steps over' the function code and waits for the function call to return)
- Step out (lets you step out of a function if you used step in and want to 'step out' of the function)
- Stop (stops debugging and terminates the program)

FIGURE 3

FIGURE 4

Let's use this approach and Spyder functionality to debug a number adding program.
```Python
print('Enter the first number to add: ')
first = input()
print('Enter the second number to add: ')
second = input()
print('Enter the third number to add: ')
third = input()
print('The sum is ' + first + second + third)
```

First run the program without the debugger enabled. What happens?

Debug the file going line-by-line. Remember to use `Step Over` to execute functions without going into each line of the function code.
- Functions in this sample program include `print()` and `input()`
- You can always `Step Out` if you accidently step into a function

<blockquote>QX: What type of error does this program return (syntax, runtime, semantic) and why? How would we go about modifying the program to address this error?</blockquote>

# Other approaches to debugging

If you've enver put a `print()` statement in your code to output a variable's value while the program is running, you have used a form of `logging` to debug your code.

Python's `logging` module lets you record custom messages that output as part of your program. 

These `log` messages describe when the program reaches a point where a logging function is called and what variables have been specified at that point.

Step one is to import the `logging` module and set up basic configuration for the module at the top of your `.py` file.
```Python
import logging
logging.basicConfig(level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')
```

This configuration information instructs Python to create a `LogRecord` object when a logging function is called, and to include specific information about that event in the `LogRecord` object.

So how would we use the `logging` module when writing a program?

Say we were creating a function that calcualted the factorial of a given number.
- Factorial 4 is 1 x 2 x 3 x 4 = 24
- Factorial 7 is 1 x 2 x 3 x 4 x 5 x 6 x 7 = 5040

```Python
import logging
logging.basicConfig(level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')
logging.debug('Start of program')

def factorial(n):
  logging.debug('Start of factorial(%s%%)' % (n))
  total = 1
  for i in range(n + 1):
    total *= i
    logging.debug('i is ' + str(i) + ', total is ' + str(total))
  logging.debug('End of factorial(%s%%)' % (n))
  return total

print(factorial(5))
logging.debug('End of program')
```

Anytime we call the `logging.debug()` function, the configuration information from the start of the file governs the log formatting and messages.

What happens when we run this program? What kinds of log messages do we get, and what information do they give us?

Is this program doing what we expect? Where would you go next with debugging or addressing the error?

## But why can't I debug using `print()`

It can seem unwieldy to configure the `logging` module and write lines of code dedicated just to logging what's happening in your program.

But think about the factorial example. Log messages led us right to the program's issue. 

Trying to debug using `print()` calls means you'll have to go back through each line of your program to remove `print()` statements used for debugging (while also making sure you aren't removing `print()` statements that are a component of the actual program).

Think of the `logging` module as a report that generates alongside your program output as it executes. The program executes and you also have useful log information about what happened along the way.

Once you're done debugging the program, you can add the `logging.disable()` function to the start of your program to supress the log messages without actually having to modify your program.

<blockquote>Visit Python's <a href="https://docs.python.org/3/howto/logging.html">Logging HOWTO</a> documentation to learn more about the logging module.</blockquote>

<blockquote>QX: Thoughts on this approach to identifying what's happening in your program. What seems appealing, what seems challenging, when could this be useful?</blockquote>

# Python in Jupyter notebooks

# Project Prompts

Run Python refresh lab in both environments. Include `.py` file and Jupyter notebook `.ipynb` file that documents your experience working through the prompts. 

<blockquote>QX: Compare your experience working in both IDEs. What seems appealing about each, what seems challenging about each. Your preference or situations where you'd prefer one over the other</blockquote>

# Lab Notebook Questions
