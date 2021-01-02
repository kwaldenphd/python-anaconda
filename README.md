# Lab #1: The Python Ecosystem

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Goals

## Acknowledgements

Information and exercises in this lab are adapted from the following text:

Al Sweigart's [*Automate the Boring Stuff With Python*](https://nostarch.com/automatestuff2) (No Starch Press, 2020).
- Chapter 11, "Debugging" (249-266)

The author consulted the following texts when writing this tutorial:
- Allen Downey, [*Think Python: How to Think Like a Computer Scientist*](https://www.oreilly.com/library/view/think-python-2nd/9781491939406/) (O'Reilly, 2015).
  * Chapter 2 "Variables, Expressions and Statements" (11-20)
- Quinn Dombrowski, Tassie Gniady, and David Kloster, "Introduction to Jupyter Notebooks," The Programming Historian 8 (2019), https://doi.org/10.46430/phen0087

# Table of Contents

- [Different types of Python environments](#different-types-of-python-environments)
- [Installing Anaconda](#installing-anaconda)
- [Python in Spyder](#python-in-spyder)
  * [Installing packages in Spyder] ADD THIS SECTION
- [Debugging](#debugging)
  * [Stepwise debugging in Spyder](#stepwise-debugging-in-spyder)
  * [Other approaches to debugging](#other-approaches-to-debugging)
  * [But why can't I debug using `print()`](#but-why-cant-i-debug-using-print)
- [Python in Jupyter notebooks](#python-in-jupyter-notebooks)
  * [Installing packages in Jupyter notebooks] ADD THIS SECTION
- [Project prompts](#project-prompts)
- [Lab notebook questions](#lab-notebook-questions)
  * [Notebook questions from this section of the lab](#notebook-questions-from-this-section-of-the-lab)
  * [Notebook questions from the Python Refresh Lab Procedure](#notebook-questions-from-the-python-refresh-lab-procedure)

# Different types of Python environments

1. In the Fall 2020 iteration of Elements I, we used the browser-based IDE [Replit](https://repl.it/).

2. What is an IDE? "An integrated development environment (IDE) is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of at least a source code editor, build automation tools and a debugger" ([Wikipedia](https://en.wikipedia.org/wiki/Integrated_development_environment)).

3. An IDE can include features like syntax highlighting, code completion, version control, and debugging.

5. There are a WIDE range of IDEs that are proprietary or open-source, tailored to a specific language or able to work across languages.

5. Some common IDEs include Eclipse, Geany, Brackets, Atom, PyCharm, Spyder, RStudio, etc. For more in IDEs, visit Wikipedia's ["Comparison of integrated development environments"](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments) page.

6. Replit (generally) worked for (most of) our needs in Elements I. But it ran into problems with more complex programs or programs involving external files/datasets/etc. 

7. So in this semester, we're going to install Python on your local computer, using a distribution called Anaconda.

8. What is Anaconda? "Anaconda is a open-source distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment. The distribution includes data-science packages suitable for Windows, Linux, and macOS. It is developed and maintained by Anaconda, Inc., which was founded by Peter Wang and Travis Oliphant in 2012" ([Wikipedia](https://en.wikipedia.org/wiki/Anaconda_(Python_distribution))).

9. The Anaconda environment includes a number of specific tools and programs, including:
- JupyterLab
- Jupyter Notebook
- Qt Console
- Spyder
- Glue
- Orange
- RStudio
- Visual Code Studio

10. This semester, we'll be using the Jupyter Notebook and Spyder components of Anaconda.

# Installing Anaconda

11. Windows/PC instructions:
- Anaconda Documentation, ["Installing on Windows"](https://docs.anaconda.com/anaconda/install/windows/) *Anaconda* (2020).
- ProgrammingKnowledge, ["Install Anaconda Python, Jupyter Notebook and Spyder on Windows 10"](https://youtu.be/5mDYijMfSzs) *YouTube video* (4 September 2018).

12. Mac OS instructions:
- Anaconda Documentation, ["Installing on macOS"](https://docs.anaconda.com/anaconda/install/mac-os/) *Anaconda* (2020).
- Understanding Data, ["Easily Install Anaconda Python Distribution On Mac OS X"](https://youtu.be/V6ZAv7hBH6Y) *YouTube video* (16 October 2019).


13. Chromebook instructions:
- Alex P. Miller, ["Data Science on a Chromebook: How to run Jupyter, Python, and R locally in ChromeOS"](https://alex.miller.im/posts/data-science-chromebook-pixelbook-jupyter-python-r/) *personal blog* (6 March 2019).
- Noebrian, ["Installing Anaconda on a Chromebook"](https://chromebook.home.blog/2019/01/20/installing-anaconda-on-a-chromebook-no-dev-beta-or-crouton-needed/) *ChromeBooks* (20 January 2019).

<blockquote>QX: Something about installation process in relation to available/provided documentation</blockquote>

# Python in Spyder

14. What is Spyder? "Spyder is a free and open source scientific environment written in Python, for Python, and designed by and for scientists, engineers and data analysts. It features a unique combination of the advanced editing, analysis, debugging, and profiling functionality of a comprehensive development tool with the data exploration, interactive execution, deep inspection, and beautiful visualization capabilities of a scientific package" ([Spyder documentation](https://www.spyder-ide.org/)).

15. Spyder's core components include:
- Editor
- IPython console
- Variable explorer
- Plots
- Debugger
- Help

16. These robust Python features in Spyder will be incredibly useful as we start to do more work with datasets, visualizations (plots), and debugging in more complex programming environments.

17. Open the Anaconda navigator and select the option to launch Spyder.

18. NOTE: When we were working in Replit, all files that were part of our Python project were in the same virtual workspace. 

19. That's not going to be the case when working in a desktop IDE like Spyder. 

20. Think of this as the difference between working with files in Google Drive versus on your local computer. 

21. You can set a working directory, which is where Spyder will look for external files you are wanting to access from within a Python program. The working directory is also where Python will save `.py` files you build.

22. Click on the folder icon in the top-right hand corner of Spyder (next to the arrow icon) to set a working directory. It doe--where you save `.py` files and other files (think data files) you might be wanting to access as part of a Python program.

23. Now, files don't have to be in your current working directory for you to access them in Python. But you'll need to provide the full file path (i.e. location information or directory information for where that file is located on your computer).

24. Go ahead and create an `EoC_II` folder and set that folder as your working directory in Spyder. It might also be a good idea to start creating lab-specific sub-folders within your `EoC_II` parent folder. 

25. This will help with organization as we move through labs and work with a variety of sample files and datasets.

26. Spyder has three default panes that show up when you launch the program.

IMAGE

27. Your `.py` file shows up on the left-hand side of the program window. This is where you will write Python code. You can have multiple `.py` files open in Spyder and navigate between the tabs. 

28. The top-right pane has four default options:
- Variable explorer, which lets you see named variables in your program
- Help, which provides additional documentation, information, or resources
- Plots, which will show visualizations generated by your program
- Files, which will show all files currently open or active in your Spyder workspace

29. The bottom-right pane is the Console, which lets you execute and test Python commands. You can have multiple consoles open simultaneously.

30. So how is the Console different from your `.py` file?

31. In the `.py` file you are writing a Python program that will run or execute when the file is called. You make updates to that file, save changes, etc.

32. The Console lets you execute Python commands but is not saving those commands as part of a `.py` file. 

33. Great for testing. Less great for building out complex programs.

34. Work through the ["First Steps with Spyder" resources](https://docs.spyder-ide.org/current/first-steps-with-spyder.html) provided by Spyder. That includes two 3.5 minute videos that introduce you to the basics of the Spyder IDE and how to get started with Python in Spyder.

<blockquote>QX: How is Spyder different than previous IDEs? What do you see as strengths/advantages? What do you see as possible challenges?</blockquote>

<blockquote>OPTIONAL: Take one of your Python files or programs from Elements I and load it into Spyder. Explore how the program runs in a different IDE. In particular, explore Spyder's options to run portions or a selection of the larger program. How does this change the way you interact with the program?</blockquote>

# Debugging

35. To paraphrase an old programming joke, writing code is 90% of the work of programming. Debugging is the other 90%.

36. You've been working on a program for hours, your head hurts, and something still isn't working. We all know a version of that feeling.

37. There's no easy solution that will prevent all problems (or "bugs") in your code. But having strategies for testing your code, recognizing and making sense of error messages, and methodically debugging your code can help immensely.

38. Python errors will usually fall into three types: syntax, runtime, and semantic.

39. Syntax refers to the structure of a program and rules about that structure. 

40. ***Syntax errors*** involve things like indentation, parenthesis, etc. The Python interpreter expects the language to be structured a specific way, and throws a syntax error when it's not.

41. ***Runtime errors***, or ***exceptions***: appears after a program has started running. These errors indicate something unexpected has happened that interrupts or stops the program execution. 

42. Things that can cause a runtime error include:
- Misspelled or incorrectly capitalized variables or function names
- Dividing by zero
- Mismatched data types (i.e. attempting to perform operations on data of the wrong type)
- Attempting to use a type conversion function on a value that can't be converted

43. Semantic: relates to meaning. 

44. ***Semantic errors*** have to do with the meaning (or purpose/intent) of your code. Semantic errors don't show up as error messages-but the program will not do what you expect it to do. 

45. The debugging strategies discussed here will focus on semantic errors but are useful for all types of errors.

## Stepwise debugging in Spyder

46. Spyder will catch many syntax and runtime errors. 

47. Hover over a red `X` by any of your lines of code to see more information about a possible error.

48. Spyder integrates the enhanced `ipdb` debugger, which gives you robust options for troubleshooting or debugging your code.

49. Specifically, the debugger will let you run a program line by line, running a single line of code and waiting for you to tell it to continue.

50. Running your program through this kind of debugging is immensely valuable for tracking down bugs or catching complex issues in a program.

51. This mode of debugging includes the following possible steps or "moves":
- Continue (run the program until the next breakpoint)
- Step in (executes the next line of code; if the next line of code is a function, the debugger will 'step into' the first line of that function)
- Step over (executes the next line of code, but will not go line-by-line through the function; the debugger 'steps over' the function code and waits for the function call to return)
- Step out (lets you step out of a function if you used step in and want to 'step out' of the function)
- Stop (stops debugging and terminates the program)

FIGURE 3

FIGURE 4

52. Let's use this approach and Spyder functionality to debug a number adding program..

```Python
print('Enter the first number to add: ')
first = input()
print('Enter the second number to add: ')
second = input()
print('Enter the third number to add: ')
third = input()
print('The sum is ' + first + second + third)
```

53. First run the program without the debugger enabled. What happens?

54. Debug the file going line-by-line. Remember to use `Step Over` to execute functions without going into each line of the function code.
- Functions in this sample program include `print()` and `input()`
- You can always `Step Out` if you accidently step into a function

<blockquote>QX: What type of error does this program return (syntax, runtime, semantic) and why? How would we go about modifying the program to address this error?</blockquote>

## Other approaches to debugging

55. If you've enver put a `print()` statement in your code to output a variable's value while the program is running, you have used a form of `logging` to debug your code.

56. Python's `logging` module lets you record custom messages that output as part of your program. 

57. These `log` messages describe when the program reaches a point where a logging function is called and what variables have been specified at that point.

58. Step one is to import the `logging` module and set up basic configuration for the module at the top of your `.py` file.
```Python
import logging
logging.basicConfig(level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')
```

59. This configuration information instructs Python to create a `LogRecord` object when a logging function is called, and to include specific information about that event in the `LogRecord` object.

60. So how would we use the `logging` module when writing a program?

61. Say we were creating a function that calcualted the factorial of a given number.
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

62. Anytime we call the `logging.debug()` function, the configuration information from the start of the file governs the log formatting and messages.

<blockquote>QX: What happens when we run this program? What kinds of log messages do we get, and what information do they give us?</blockquote>

<blockquote>QX: Is this program doing what we expect? Where would you go next with debugging or addressing the error?</blockquote>

## But why can't I debug using `print()`

63. It can seem unwieldy to configure the `logging` module and write lines of code dedicated just to logging what's happening in your program.

64. But think about the factorial example. Log messages led us right to the program's issue. 

65. Trying to debug using `print()` calls means you'll have to go back through each line of your program to remove `print()` statements used for debugging (while also making sure you aren't removing `print()` statements that are a component of the actual program).

66. Think of the `logging` module as a report that generates alongside your program output as it executes. The program executes and you also have useful log information about what happened along the way.

67. Once you're done debugging the program, you can add the `logging.disable()` function to the start of your program to supress the log messages without actually having to modify your program.

<blockquote>Visit Python's <a href="https://docs.python.org/3/howto/logging.html">Logging HOWTO</a> documentation to learn more about the logging module.</blockquote>

<blockquote>QX: Thoughts on this approach to identifying what's happening in your program. What seems appealing, what seems challenging, when could this be useful?</blockquote>

# Python in Jupyter notebooks

68. What is Jupyter?

69. "Project Jupyter is a non-profit, open-source project, born out of the IPython Project in 2014 as it evolved to support interactive data science and scientific computing across all programming languages. Jupyter will always be 100% open-source software, free for all to use and released under the liberal terms of the modified BSD license" (["About Us"](https://jupyter.org/about), *Jupyter.org*)

70. Project Jupyter receives funding from a range of non-profit foundations and corporate partners that include:
- Alfred P. Sloan Foundation
- Gordon and Betty Moore Foundation
- Google
- Microsoft

71. Institutional partners for Project Jupyter include:
- Apple
- Bloomberg
- Netflix
- Cal Poly
- Berkeley
- Amazon Web Services (AWS)

72. The name Jupyter is a reference to the three core languages supported by the project: **Ju**lia, **Py**thon, and **R**.

73. And what is a Jupyter notebook?

74. According to "[The Jupyter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html)" documentation:

<blockquote>The notebook extends the console-based approach to interactive computing in a qualitatively new direction, providing a web-based application suitable for capturing the whole computation process: developing, documenting, and executing code, as well as communicating the results. The Jupyter notebook combines two components:
 <ul>
  <li>A web application: a browser-based tool for interactive authoring of documents which combine explanatory text, mathematics, computations and their rich media output.</li>
  <li>Notebook documents: a representation of all content visible in the web application, including inputs and outputs of the computations, explanatory text, mathematics, images, and rich media representations of objects</li>
 </ul>
 </blockquote>

75. A Jupyter notebook is a file (the notebook document) that displays or renders in a web browser.

76. We'll be launching Jupyter Notebooks through Anaconda. 

77. The web application component of the notebook will be hosted on your local computer and the notebook document will save to a file directory on your local computer.

FIGURE ONE

FIGURE FIVE

78. It may take some time for the notebook to open in a browser window.

FIGURE 6

79. When in a new notebook document, you have four main components to the user interface:
- Notebook name
- Menu bar
- Toolbar
- Code cell

80. The notebook name is what the `.ipynb` file created via the Jupyter notebook will be saved as.

81. Click on the default notebook name (usually `Untitled`) to rename the notebook.

82. The menu bar includes drop-down options used to manipulate the notebook functionality.

83. The toolbar icons give you quick access to the most commonly-used features of the notebook environment.

84. Code cells are the default type of cell.

85. But why are there cells?

86. Jupyter notebooks consist of a sequence of cells.

87. A cell is a multiline text input field. 

88. You can execute the contents of a cell by using `Shift-Enter`, clicking the `Play` button in the toolbar, or the `Cell` and `Run` icons in the menu bar.

89. How a cell executes is determined by its type.

90. There are three types of Jupyter notebook cells.

91. ***Code cells*** allow you to edit and write code with full syntax highlighting and tab completion.

91. ***Markdown cells*** allow you to document the computational process using descriptive text formatted using the markdown language.

92. ***Raw cells*** allow you to write output directly. These cells are not evaluated by the notebook and render unmodified.

93. You can edit or work within a code cell until you get the desired output, then move on to a new cell.

94. You can use markdown cells along the way to document your process using narrative text (alongside or in addition to code comments used in code cells).

95. To learn more about formatting text in markdown, visit Adam Pritchard's ["Markdown Cheatsheet"](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) resource page.

96. You can download a Jupyter notebook as a `.ipynb` file (this is the default option).

97. You can also use the `File` - `Download as` menu options to download the notebook in a number of other formats, including `.py`, `.pdf`, or `.html`.

98. There's a lot to love about Jupyter notebooks. 

99. A few challenges or drawbacks:
- Version control especially in collaborative environments is virtually impossible
- Jupyter lacks the debugging tools and autocompletion features of an IDE
- Testing and debugging code is virtually impossible
- Installing third-party packages or modules can be tricky 
- Jupyter's non-linear workflow limits transparent reproducible code
- Jupyter doesn't play well with external big data applications (spark/dask/distributed)

<blockquote>Citation: Alexander Mueller, <a href= "https://towardsdatascience.com/5-reasons-why-jupyter-notebooks-suck-4dc201e27086">"5 reasons why jupyter notebooks suck"</a>, <i>Towards Data Science</i> (24 March 2018)</blockquote>

100. So when could you use Jupyter notebooks? 

101. Jupyter notebooks are fantastic tools for exploration. 

102. They also work well for documenting process, or in situations when you might need to alternate between code and other kinds of text (like say in a lab notebook).

# Project Prompts

Run [Python refresh lab procedure](https://github.com/kwaldenphd/python-refresh/blob/main/lab-procedure.md) in both environments. Include `.py` file and Jupyter notebook `.ipynb` file that document your experience working through the prompts. 

<blockquote>QX: Compare your experience working in both IDEs. What seems appealing about each, what seems challenging about each. Your preference or situations where you'd prefer one over the other</blockquote>

# Lab notebook questions

## Notebook questions from this section of the lab

## Notebook questions from the [Python Refresh Lab Procedure](https://github.com/kwaldenphd/python-refresh/blob/main/lab-procedure.md)

QA: In your own words, explain the difference between the `print(hello)` command we just used and `print(“hello”)`.

QB: Describe the syntax three commands that we just used in your own words. Define the function and method for each example.

QC: Explain how each of these two programs (above) work in your own words.

QD: Why does `print(2/3)` return 0? How would you modify your code to return the decimal number?

QE: Explain `concatenation` in your own words. Why must we convert numbers to strings in the program above? Refer to this example and the previous example.

QF: Create your own list using the program above as an example. Share your code in your notebook as well as the result. What is the number position for each of the items in your list? How would you return the value of the first item? How would you return the value of the last item?

QG: What is an alternative way to write the `print` command to return the length of the list. *Hint* you’ll combine the last two lines of the example above.

QH: How would you modify this code to output the full range 1-10?

QI: How would you rewrite the code to include only the even numbers from 1 to 10?

QJ: Either include a snippet of your version of this program in your notebook and explain your code, AND/OR explain how the example version of this program works.

QK: What do you expect this code to output? Explain how this program works in your own words.

QL: Did the program return the results that you expected? Explain the output in your own words.

QM: Explain what this program will output and why.

QN: What did the program output? Explain this program in your own words.

QO: Modify the code to change the range to have the user guess between 1 and 100. Then, change the conditional statement to return a “really close” message if they are within a 3 digit range of your number. Include the code in your notes and explain how the program works in your own words.

QP: Create a dictionary for one of the items in your collection using the tags and information from your XML file. Write a `print` command and explain the output of your program in your own words.	

QQ: Try the following two programs. What did the programs output? Explain how each program works in your own words.
  
```Python
for tag in book.keys():
  print(tag)
```
and 

```Python
for data in book.values(): 
    print(data)
```  
  
QR: Explain the `if` functions in your own words. What does this program output? Why?

