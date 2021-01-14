# 1.2 Programming With Python

## Overview

In this class, students will practice and review fundamental programming concepts of object oriented programming using Python. 

## Class Objectives

By the end of class, students will:

* Define and implement variables, data types, conditionals and loops in Python 
* Create a Python script that uses `for` loops and conditionals
* Create a Python script that can read and write from a CSV file
* Create a Python script that uses a custom function and list comprehension

## Class Outline

| | Topic | Time |
| -- | -- | -- |
| 1. | [Python Programming Praxis](#Section1) | 25 Mins |
| 2. | [Practicing Python Loops](#Section2) | 60 Mins |
| 3. | [Break](#Break) | 15 Mins |
| 4. | [Input and Output Scripts in Python](#Section3) | 20 Mins |
| 5. | [Getting the Most Out of Python Functions](#Section4) | 45 Mins |
| 6. | [Getting to know Git and End Class](#Section5) | 15 Mins |
| 7. | [Skill Drill](#Skill_Drill) | |

> Total Time: 180 mins

## Instructor Prep

<details>
  <summary><strong>⭐ Notes for Today </strong></summary>
<br>

* Today's class will review the fundamentals of Python programming in order to ensure that everyone is on the same page before moving on to more applied Python concepts. Although some students may use Python on a regular or semi-regular basis, not all students will have used Python recently. These students will benefit greatly from today's activities. For those students who *do* use Python, you can be open and honest that today will be an easy day that they should enjoy alongside their peers. However, reassure those students that this class will quickly ramp-up as we move onto more complex topics. 

* When the lesson plan calls for files to be sent to students there are a few ways to do so. For the first couple of days it may be easiest to use Slack, but as the files and directories get more complex you may look to try alternate methods such as pushing and pulling from GitHub/GitLab and sending out the link, using a file storage like Google Drive, or zipping up files and continuing to Slack out. 
  
  * **Note:** At the end of today's class, we will teach students how to use Github and GitLab. Please start to transition to this workflow as soon as you and the students are comfortable. The more exposure students receive to Git environments, the better.  

* For the first units of the course, each Student-Do will include bonus "stretch goals". Any student who has completed the required goals for the activity is encouraged to challenge themselves and attempt the bonuses in the time allotted. These bonuses are designed to further explore the functionality and use-cases of our analytical tools and empower students to expand their technical prowess. Be aware that many of these bonuses will not be directly covered in the previous activities and will require some form of reading through documentation, Stack Overflow or Googling. 

</details>

<details>
  <summary><strong>⭐ General Class Notes </strong></summary>
<br>

* For each class, you will be provided a Lesson Plan outline (this document), activity folders to accompany each activity (including solved and unsolved versions of the materials), as well as a [slideshow](https://docs.google.com/presentation/d/1csMP22c5Hb-GRIy__tjp1tsb3jJB5CTsTTjwOHrksrY) that can be used to help facilitate the presentation for the day. You are encouraged to use the slideshow to help students follow along with the class activities and to assist the engagement of students who are more visual learners.

* Feel free to distribute these slides to the students before or after class. However, the links to the slideshows are for instructor-use only. When distributing slides to students, please first export the slides to a PDF file and then send out the PDF file.

* Have fun and enjoy the ride!

</details>

## Slideshow

The lesson slides for this document are available on Google Drive here: [1.2 Slides](https://docs.google.com/presentation/d/1csMP22c5Hb-GRIy__tjp1tsb3jJB5CTsTTjwOHrksrY)

---

## Class Activities

### 1. <a name="Section1"></a> Python Programming Praxis

| Activity Time:       0:25 |  Elapsed Time:      0:00  |
|---------------------------|---------------------------|

<details>
  <summary><strong>📣 1.1 Instructor Do: Python Programming Intro (0:05)</strong></summary>
 <br>

Welcome students to class and provide an overview of today's topics and activities: 

  * Today's class will focus solely on Python programming concepts and review. Starting next class we will begin our journey into applied data science with Pandas!

  * Some students may already use Python on a regular basis. If so, this class should be an easy-going day. But don't worry, things will start to pick up next class.

  * Some students may have used Python in the past and have forgotten syntax or general Python structure. This class should serve as a pleasant review.

  * Some students may not have used Python much at all or they may not feel entirely confident in programming. If so, this lesson will be a crash course. We we will be building upon these concepts rapidly throughout the following units.  

</details>

<details>
  <summary><strong>🎉 1.2 Everyone Do: Python Programming Pop Quiz (0:20)</strong></summary>
<br>

In this activity, the class will work together to review the different components and major concepts of object-oriented programming in Python. For each quiz question, the slideshow will provide be a question slide followed by the answer slide.

We will start by reviewing the general structure of code:

1. Generally speaking, what are **variables** in Python?

   * A **variable** is a symbolic name that references a value stored in the memory of a Python program.

2. What are the eight most common **data types** in Python and what are they used for? (In any order.)

    * **Integers** store whole numbers which can be positive or negative values, with no decimal points. They do not have a size limit.

    * A **float** or floating point number is a number with decimal places. It can represent either a positive or negative number. 

    * A **list** is an ordered collection of mutable items. This means that any object stored within a list can be retrieved via index, and the objects stored within the list can be changed.

    * A **set** is an unordered collection of unique, immutable items. This means that items in a collection are not position aware and cannot be retrieved by an index. Additionally items stored within a set are immutable meaning once they are stored in the set they cannot be changed. Lastly, if we try to store two or more of the same objects already stored in the list, the size of the list will not change.

    * A **tuple** is an ordered collection of immutable items. Therefore tuples strike a balance between the positional awareness of a list with the rigid immutability of a set.

    * A **dictionary** is an unordered collection of mutable, indexed key-value pairs. This means that in order to retrieve the values stored in the dictionary, you must access them using the associated "key".

    * A **string** is an array of bytes that represent a collection of Unicode (text) characters.

    * A **boolean** is a binary variable that represents two states: true and false. 

3. Identify and define the following operators:

    * `%` - modulus

      * Modulus returns the whole number remainder after dividing by the value following the modulus.

    * `**` - exponential

      * Raises the number preceding the exponential operator by the number that follows.

    * `//` - floor division 

      * Rounds down to the largest integer when dividing.

    * `==` - equal to

    * `>=` - greater than or equal to

    * `<=` - less than or equal to

    * `!=` - not equal to

    * `and` - the `and` operator checks if both statements are true

    * `or` - the `or` operator checks if either statements are true

    * `not` - the `not` operator inverses the logic of the statement

    * `+=` - the `addition assignment` will add the object/value on the right of the operator to the object/value on the left and reassign the the variable on the left to our new value.

    * `-=` - the `subtraction assignment` will subtract the object/value on the right of the operator to the object/value on the left and reassign the variable on the left to our new value.

    * `is` - the `is` operator tests if two objects are identical. This is at the programming level, and a step beyond the simpler `==` operator.

    * `in` - the `in` operator checks if a variable is contained within a collection

4. What is a **class** in Python?

    * A **class** acts as a blueprint in Python and defines the structure of an object. Each time a class is instantiated, it contains a copy of all of the predefined variables, functions and logic.

5. What is a **function** versus a **method** in Python?

    * A **function** is a specific set of instructions that is assigned a name in the Python program. Every time a function is called, the instructions are executed by the program. Functions can have zero to many arguments that point to other objects and variables in memory.

    * A **method** is a special type of function in Python that is defined within an object or class. Therefore whenever the method is called, all of the class's information is accessible by the method. 

6. What does the output of `",".join(["apple","orange","pear"])` look like?

    * `'apple,orange,pear'`

7. What does the output of `"This was a triumph".split(" ")` look like?

    * `['This', 'was', 'a', 'triumph']`

8. What does the output of `'supercalifragilisticexpialidocious'[0:5]` look like?

    * `super`

9. What does the output of the following block of code look like:

    ```python
    var1 = "fox"
    var2 = "dog"

    f"The quick brown {var1} jumped over the lazy {var2}
    ```

   * 'The quick brown fox jumped over the lazy dog'

Be sure to an answer any student questions before moving on.

</details>

---

### 2. <a name="Section2"></a> Practicing Python Loops

| Activity Time:       0:60 |  Elapsed Time:      0:25  |
|---------------------------|---------------------------|

<details>

  <summary><strong>📣 2.1 Instructor Do: Round and Round We Go with Loops (0:30)</strong></summary>
<br>

Now that students have had a chance to review the structures in Python programming, we need to review one of the most critical concepts in data science programming - loops! In addition to our for and `while` loop review, we will also cover conditionals, try-except blocks, and raising exceptions, which are often used in conjunction with our loops. 

* Introduce loops by covering the following: 

  * One of the most widely used components in a Python script are their loops. Loops allow us to repeat logic within our code from once to an infinite number of times. Depending on which type of loop we use, our Python code will handle its logic differently. 

  * In the data industry we are constantly challenged with making robust analysis scripts and pipelines that are easy to read and even easier to use. By building Python scripts that incorporate loops and their accompanying program, we can create analysis tools that run complex statistical analyses, build and query giant databases and even predict future outcomes using data models. 

#### `for` Loops Demonstration

In the following demonstration, we will cover different types of loops. We will also cover the major components of Python programming that are often used in conjunction with loops such as conditional statements, continue/break statements and try-except blocks. 

* You can either use the slideshow to walk through this activity or use the [activity notebook](Activities/01-Ins_Loops/Loops_Demo.ipynb) to demonstrate live. 

*  Note: As you work through the demonstration, feel free to provide your own personal example of when you would use a combination of conditionals, loops and try-except blocks. 

1. Begin by covering the **`for` loop**. The `for` loop is a generalized statement that can loop through iterator objects, strings and lists. These loops are versatile and adaptable to our needs. 

    * Most commonly in Python you will see `for x in range()` or `for <variable> in <string or list>:`. 

    * When provided with a single number, the `range()` function will always start the loop at 0. However when provided with two numbers, the code will loop from the first number until it reaches one less than the second number.

        ```python
        # Loop through an iterable range object with single argument
        for x in range(10):
          print(x)

        # Loop through an iterable range object with two arguments
        for x in range(0,10):
          print(x)
        ```

   * Alternatively, Python can loop through all of the letters within a string or all of the values stored within a list by using the syntax `for <variable> in <string or list>:`.

      ```python
      # Loop through a string character by character
      for character in "Hello World":
        print(character)

      # Loop through a list of objects
      for produce in ["apples","oranges","pears","plums"]:
        print(produce)
      ```

    * Within our **`for` loop**, or any code for that matter, we may need to change the logic or flow of our code depending on the condition of our variables in memory. **Conditional statements** are used to determine which actions should be taken by the Python program depending on whether or not the **if statement** returns `True` or `False`. 

    * Conditional statements can be as simple as a comparison between two variables using a comparison operator such as `==` or as complex as an if-statement evaluating an entire custom method or function embedded within the program. Regardless of how complex the logic within the conditional statement is, all Python scripts handle conditional statements the same way:

      * If an if-statement evaluates to be `True`, the Python program will run the code block from the if-statement. 
      
      * If an if-statement evaluates to be `False`, the Python program will look for and run the code block from an associated else-statement.

      * If no else-statement exists, the Python program will simply continue on with the next set of logic statements. 


2. The second type of loop in Python is the **while-loop**. A **while-loop** runs through its indented code as long as the while statement is `True`. In Python, any non-zero number, a non-empty collection such as a list, a conditional statement that evaluates as `True`, or a boolean variable equal to `True` are all considered to be logically `True` statements and therefore can be used within the **while statement** to run the **while-loop**. 

   * **Note**: To avoid using up all of the RAM on the computer, we are forcing our `while` loops to exit. Be sure to point out that without the exit logic, we would need to interrupt the Python kernel to stop our program from running indefinitely. 

      ```python
      # Demonstrate different logically true statements in Python and use them in a while statement. 
      # First demonstrate the nonzero number.
      value = 1
      counter = 0
      while value:
          print('I am running')
          
          counter += 1
          if counter == 10:
              value = 0

      # Then demonstrate a non-empty collection
      collection = ["This","is","a","list","of","words"]
      while collection:
        print(collection.pop(0))

      # Now demonstrate a conditional statement that returns True
      value = 10
      while value > 2:
        print(value)
        value -= 2

      # Lastly demonstrate a while-loop using a boolean variable
      counter = 0
      test = True
      while test:
        print("Running...")
        counter += 1 
      counter += 1 
        counter += 1 
        if counter == 10:
          test = False
      ```

3. When programming in Python, we'll eventually need to iterate through more programming logic within a larger loop. These internal loops are known as **nested loops**. 

   * We can nest `for` loops within other `for` loops, `for` loops within while-loops, while-loops within `for` loops and even while-loops inside of other while-loops!

      ```python
      # Demonstrate a nested for-loop in a while loop
      value = True
      while value:
          for x in range(10):
              print("System is running...")
          print("Done!")
          value = False    
        value = False    
          value = False    
      ```

4.  Sometimes when we build a loop in Python, we may not want the Python program to run through every iteration of a loop. Other times we may want our Python program to run through every iteration, but not perform all of the logic in the loop if specific conditions are met. Thankfully, we can alter the flow of our Python loops using **break** and **continue statements**.

    * The **break statement** exits out of the loop that contains the break statement and continues onto the first statement after the body of the loop.

    * Break statements are particularly useful with while-loops because they allow us to leave our while-loop without changing the while statement. When it comes to nested while-loops, keeping our while statement intact could prove highly useful!

      ```python
      # Demonstrate a break statement in a while loop
      for x in range(5):
        counter = 1
        while True:
          print(f"For loop number {x} running now. Step {counter}")
          
          if counter % 5 == 0:
            break

          counter += 1
      ```
    * The **continue statement** exits out of the current iteration of the loop and immediately moves onto the next iteration in the same loop that contains the **continue statement**.

    * Continue statements are often found within `for` loops due to the limited number of iterations performed by a `for` loop. For example, if we had a `for` loop with particularly complicated logic, we may want the `for` loop to skip an iteration if the data did not match our expectations.

      ```python
      # Demonstrate a continue statement in a for-loop
      for pen in ["red","blue","red","green","blue"]:
          
          if pen == "green": 
        if pen == "green": 
          if pen == "green": 
              continue

          print(f"The pen is {pen}")
      ```

5. When we build and run loops in Python, especially large loops, we may come across an **edge-condition** or a set of values that were not initially accounted for. These edge conditions can cause the Python program to **raise an exception** and error out, which may be undesirable. 

    * We can handle these exceptions and prevent our program from erroring out and stopping prematurely by using a **try-except** block.

    * A **try-except** block has two components: the **try block** and the **except block**. The **try block** contains all of the programming logic you want Python to test. The **except block(s)** list all of the logic to perform if a matching exception is found. 

    * Take a moment to emphasize how powerful this is. Try-except blocks allow programmers to anticipate and recover from errors.

    * Although optional, it is generally best practice to specify the precise errors to handle.

      * In cases where the programmer wants to handle a particular error in a particular fashion, specifying the exception type is best practice.

      * Especially in cases where a programmer wants to intercept any error — like for logging purposes — it is fine to catch a general exception.

    * Without a try-except block, a program will error out if an exception is raised by the program and there is no matching exception block or a general exception block.

    * Point out that there are numerous types of exceptions, many of which are defined in the [Python documentation](https://docs.python.org/3/library/exceptions.html). However when building our scripts, we will know what exceptions to handle because the name of the exception that killed the program will be printed to the command line.

      ```python
      # Demonstrate a try-except block with a specific exception block
      try:
        numerator = 1
        denominator = 5
        while True:
          denominator -= 1
          print(f"Our fraction is {numerator}/{denominator} which equals {numerator/denominator}")
      except ZeroDivisionError:
        print("You cannot divide by zero!")
      
      # Demonstrate a try-except block with the wrong specific exception block
      try:
        numerator = 1
        denominator = 5
        while True:
          denominator -= 1
          print(f"Our fraction is {numerator}/{denominator} which equals {numerator/denominator}")
      except ValueError:
        print("You cannot divide by zero!")

      # Demonstrate a try-except block with multiple exception blocks
      try:
        numerator = 1
        denominator = 5
        while True:
          denominator -= 1
          print(f"Our fraction is {numerator}/{denominator} which equals {numerator/denominator}")
      except ValueError:
        print("You cannot divide by zero!")
      except:
        print("That was a close one!")
      ```

6. Alternatively, when we are building our loops in Python, we may want to stop our program from performing tasks if special conditions are met. For example, maybe we don't want our program to update a database with new values if our update contained missing information. In these cases, we could have our Python program **raise an exception**. 

  * When we raise an exception, we tell our Python program to stop whatever it is doing and produce an error that we define using a **raise statement**. Raise statements can be whatever type of exception we want, and we can even use raise statements within a try-catch block to make our program handle errors and issues gracefully.

    ```python
    # Demonstrate a try-except block with a raise
    try:
        numerator = 1
        denominator = 5
        while True:
            denominator -= 1
            if denominator == 0:
                raise ValueError
            print(f"Our fraction is {numerator}/{denominator} which equals {numerator/denominator}")
    except ValueError:
        print("You cannot divide by zero!")
    except:
        print("That was a close one!")
    ```

Address any questions before proceeding. 

</details>

<details>

  <summary><strong>✏️ 2.2 Student Do: House of Pies (0:20)</strong></summary>
<br>

In the first student activity of the day, students will create a looped function that prompts the user for a selection from a list of pies, then displays a running tally of the current pie inventory.


* **Files:**

  * [README](Activities/02-Stu_HouseOfPies/README.md)

  * [02-Stu_HouseOfPies/HouseOfPies_Unsolved.ipynb](Activities/02-Stu_HouseOfPies/Unsolved/HouseOfPies_Unsolved.ipynb)


#### Instructions

1. Create a dictionary that stores a value of `10` for each of the following pie names: 

   * `Pecan`, `Apple`, `Blueberry`, `Pumpkin`, `Chocolate`

   * **Note:** This dictionary will act as your "inventory of pies". 

2. Create a series of print statements that will welcome and display a list of pies to the user in the following way:

    ```
    Welcome to the House of Pies! Here are our pies:
    ---------------------------------------------------------------------
    (1) Pecan, (2) Apple, (3) Blueberry, (4) Pumpkin, (5) Chocolate
    ```

3. Create a while-loop that performs the following logic:

    * First prompt the user to make a numerical selection using `input()`, store the user's selection to a variable. 

      * **Hint:** If you have never used the `input()` function before, check out some helpful documentation [here](https://www.w3schools.com/python/ref_func_input.asp).

      * A good input statement should include some text explaining the user prompt such as, `Please make a selection:`

    * Create a series of `if-else` statements that convert the numerical selection to the correct name of the pie. 

      * **Hint**: When using a series of if and else statements, try using `elif` which combines `else if` into one step. You can read more about `elif` statements [here](https://www.w3resource.com/python/python-if-else-statements.php). 

    * Simulate an order by removing a pie from your inventory that matches a user selection. 
      
      * In the context of this activity, a pie is sold when it's inventory equals zero.

      * If you try to remove a pie that is sold out, you need to raise an exception and print the following statement back to the user: `Sorry that pie is sold out.`

      * If the pie is not sold out, remove one pie from your inventory and print the following statement back to the user: `Order received.`

#### Bonus

4. When you raise an exception in your `while` loop, print out the names of any non-zero pies remaining in the inventory as a suggestion to the user. 

5. Update your `while` loop logic to stop running when all inventory equals zero.

</details>

<details>

  <summary><strong>⭐ 2.3 Review: House of Pies (0:10)</strong></summary>
<br>

Take some time to walk through the solution to the previous activity and make sure you answer any student questions before moving on. 

* Be sure to point out the following talking points:

  * When using the `input()` function, the input is stored as a string. Therefore, be sure when changing the selection to our dictionary keys that you are comparing strings not integers!

  * In our inventory logic, we never confined the input to specific values. Therefore the user could theoretically type an invalid number, the incorrect spelling of a pie name, or a random set of characters.  To address this issue, we need to make sure that our code handles any general exception. 

</details>

---

### <a name="Break"></a> Break

| Activity Time:       0:15 |  Elapsed Time:      1:25  |
|---------------------------|---------------------------|

---

### 3. <a name="Section3"></a> Input and Output Scripts in Python

| Activity Time:       0:45 |  Elapsed Time:      1:40  |
|---------------------------|---------------------------|

<details>

  <summary><strong>📣 3.1 Instructor Do: Scripting In Python (0:15)</strong></summary>
<br>

This activity will cover how to import and export CSV files in Python using the `csv` library. Although this is a more brute-force approach compared to Pandas (which we will teach in the next unit), it will reinforce concepts such as importing, reading and writing to files, indices, and delimiters.

Use the slideshow to introduce the concept of importing modules and libraries:

* While reading in text files can be useful in some circumstances, in the data industry it is more likely that you will encounter CSV files.

  * CSV stands for **Comma** **Separated** **Values**. A CSV file is essentially a table that has been converted into text format with each row and column being separated by specified symbols.

  * Typically, each row is located on a new line and each column is separated by a comma. 

    ![Example CSV](Images/01-ReadCSV_ExampleFile.png)

* If we wanted to import a CSV file into our program, we would have to read in our files using the `open()` function as a series of strings. Once imported, we would also have to split up the string, remove any extra spaces, and remove the newline characters each time we wanted to retrieve data from a specific line in our CSV. 
  
    * This workflow can become very tedious, very quickly. Even worse, printing out raw lines from a CSV file can be incredibly hard to read if our CSV file contains a large number of columns - 10, 100, even 1000 columns are not unheard of!
  
  * Rather than create all of the CSV handling logic by hand, we can **import** a **module** or **library** in Python to do most of the hard work for us. A Python **module** is a collection of pre-defined classes, modules and functions that we can import into our own Python program. A **library** is the overarching collection of modules. 

    * **Note:** When searching for documentation, you will often find that people use **library** and **module** interchangeably. Although this isn't technically correct, it is acceptable.

  * Python libraries can either be built-in to the Python program, or remote libraries installed into our Python environment using the terminal commands `pip` or `conda`. In today's demonstration, we will be using built-in libraries such as `csv` and `os`, which require no installations. 
  
#### Python Scripting Demonstration

In this demonstration, we will use Python modules to write scripts that import and manipulate data from CSV files. You can either continue using the slideshow to walk through this demonstration or use the [activity notebook](Activities/03_Ins_ReadWriteCSV/ReadWriteCSV.ipynb) to demonstrate live

1. Let's begin by importing the `csv` and `os` modules. 

   * The `csv` module allows users to easily pull in data from external CSV files and perform some operations upon them. Most notably, the `csv` module handles all of the string manipulation so we can just concentrate on accessing the table values. 
  
   * In conjunction with the built-in `os` module, we can easily create dynamic paths to external CSV files that function across different operating systems and import these CSV files into our programs.

      ```python
      # First we'll import the os module
      # This will allow us to create file paths across operating systems
      import os

      # Module for reading CSV files
      import csv
      ```

2.  To import our CSV file using the `csv` module, we will use the `csv.reader()` method in conjunction with the `open()` function to translate the object being opened by Python. 

   * It is critical to note that the `delimiter=','` parameter indicates that each comma within the CSV should be seen as moving into a new column for a row.

    ```python
    # Set path for importing our CSV file
    csvpath = os.path.join('Resources', 'accounting.csv')

    # Import our CSV file using csv.reader()
    with open(csvpath) as csvfile:

        # CSV reader specifies delimiter and variable that holds contents
        csvreader = csv.reader(csvfile, delimiter=',')
    ```

    * The output of the `csv.reader()` method is an iterable `csv.reader` object, which contains a list of our CSV elements in that row. 

 3.  Point out that if our table contains a header row, we will need to capture the first element in our iterator object using the `next()` function. 

      ```python
      # Read the header row first (skip this step if there is no header)
      csv_header = next(csvreader)
      print(f"CSV Header: {csv_header}")
      ```

   * The code then loops through each row of the CSV and prints out the contents. Make sure to point out how each value is being shown as a string and how all of the rows are lists.

      ```python
      # Read each row of data after the header
      for row in csvreader:
          print(row)
      ```

4. Since the elements in our `csv.reader` object are lists, we can modify them in real-time. What if we wanted to mask the Social Security numbers so that only the last four digits are visible?

   * Point out that we can retrieve a substring in Python by using the substring syntax `string[start:stop]`. In this case we are telling Python to start at the 8th character (remember base 0!) and retrieve the rest of the string.

      ```python
      # Set path for importing our CSV file
      csvpath = os.path.join('Resources', 'accounting.csv')

      # Import our CSV file using csv.reader()
      with open(csvpath) as csvfile:

        # CSV reader specifies delimiter and variable that holds contents
        csvreader = csv.reader(csvfile, delimiter=',')

        # Read the header row first (skip this step if there is no header)
        csv_header = next(csvreader)
        print(f"CSV Header: {csv_header}")

        # Read each row of data after the header, mask the SSNs
        for row in csvreader:
            row[2] = row[2][7:]
            print(row)
      ```  

    * Alternatively, we can use a negative number syntax such as `row[2][-4:]` to tell Python to retrieve the fourth from the last character to the end. 

      ```python
      # Set path for importing our CSV file
      csvpath = os.path.join('Resources', 'accounting.csv')

      # Import our CSV file using csv.reader()
      with open(csvpath) as csvfile:

          # CSV reader specifies delimiter and variable that holds contents
          csvreader = csv.reader(csvfile, delimiter=',')

          # Read the header row first (skip this step if there is no header)
          csv_header = next(csvreader)
          print(f"CSV Header: {csv_header}")

          # Read each row of data after the header, mask the SSNs
          for row in csvreader:
              row[2] = row[2][-4:]
              print(row)
      ```

5. The `csv` and `os` libraries can also help us write our new CSV rows to a new file. In addition to the `open()` function that opened a reading connection to the CSV file, we need to open up a writing connection to an output file using another `open()` function in conjunction with `csv.writer()` method.

   * Similar to `csv.reader()` method, we use the `csv.writer()` method to handle all of the merging and newline character building for our output file. 

    * **Note:** When writing to a file using the `open()` function, we use an optional second argument `'w'`.

   * To start writing to a CSV file, we create our `csv.writer` object and then write each individual row using the `csv.writer.writerow()` method.

      ```python
      # Set path for importing and exporting our CSV file
      csvpath = os.path.join('Resources', 'accounting.csv')
      outpath = os.path.join('Resources', 'accounting_masked.csv')

      # Import our CSV file using csv.reader() and export with csv.writer()
      with open(csvpath) as csvfile:
          with open(outpath,'w') as outfile:
              # CSV reader specifies delimiter and variable that holds contents
              csvreader = csv.reader(csvfile, delimiter=',')

              # CSV writer also specifies delimiter and variable that exports contents
              csvwriter = csv.writer(outfile, delimiter=',')

              # Read the header row first (skip this step if there is no header)
              csv_header = next(csvreader)
              csv_header[2] = "Masked_SSN"
              csvwriter.writerow(csv_header)
              print(f"CSV Header: {csv_header}")

              # Read each row of data after the header, mask the SSNs
              for row in csvreader:
                  row[2] = row[2][-4:]
                  csvwriter.writerow(row)
                  print(row)
      ``` 


Be sure to answer any student questions before moving on.

</details>

<details>

  <summary><strong>✏️ 3.2 Student Do: Solving Data Problems with Scripts (0:20)</strong></summary>
<br>

In this activity, students will practice importing, updating and exporting values from data files. 

* **Files**:

  * [README](Activities/04-Stu_SolvingDataWithScripts/README.md)

  * [04-Stu_SolvingDataWithScripts/SolvingDataWithScripts_Unsolved.ipynb](Activities/04-Stu_SolvingDataWithScripts/Unsolved\SolvingDataWithScripts_Unsolved.ipynb)

#### Instructions

1. First, import the `os` and `csv` libraries into your notebook.

2. Use `os.path.join` to build both the path to your tab-delimited `netflix_ratings.txt` file, and an outfile named `netflix_ratings_cleaned.csv` in the `Resources` folder of this activity.

3. Once you have created your paths, open a connection to the tab-delimited import file and the comma-delimited export file using the `open()` function.

4. Create your instances of `csv.reader()` and `csv.writer()` methods to import and export your files.

   * **Hint:** The table file we are importing is not comma-delimited. Rather, it is `\t` tab-delimited. How would you modify your `csv.reader()` method to accommodate this difference? 

5. Read in your column header row and remove the `ratingLevel` column from your list of column headers.

6. Write out your new header row to the new comma-delimited outfile.

7. Iterate through each row of your import file and apply the following changes. Once you apply these changes to each row, print the row in your Python notebook and write the row out to the new comma-delimited outfile.

   * Concatenate the second and third columns in each row using a hyphen `-` to make a single `rating` column. Set this concatenated string to the second column in each row.

   * Remove the third column from each row.

   * Check if the fifth column in each row is equal to `"NA"`. If so, replace the fifth column value with a value of `"50"`.

#### Bonus

8. If you are familiar with importing and exporting using `csv`, or if you want an additional challenge, try exporting your table into a **JavaScript Object Notation** (**JSON**) format using the `csv` library along with the built-in `json` library. A few notes on using the `json` library:

   * If you export to a `json`, change your filename to `netflix_ratings_cleaned.json`. 

   * Instead of using the `csv.reader()` to handle each row in our import file, use the `csv.DictReader()` class. This class will convert each row into an ordered Python dictionary. A Python dictionary is very similar to the structure of a JSON object and is required when using the `json` library to export. 

   * The `json` library does not write each row to the output file individually like `csv.writer()`. Instead you will write the entire file out at once using the `.write(json.dumps())` method from your connected output file. Therefore, you will need to create an empty dictionary at the top of your Python notebook and fill it with each row.
  
   * Because each row is converted to a dictionary, you must concatenate the `rating` and `ratingLevel` column, set `row["rating"]` to this concatenated value, and drop the `ratingLevel` using the `row.pop("ratingLevel")` method. 

   * Similarly, your rows are using the header names as the key for your row dictionary. Therefore, in order to check whether or not the fifth column is equal to `"NA"`, you must use the `user rating score` instead of the relative index.

   * To see a great example of exporting a CSV file to a `JSON` file using the `json` library, check out this article: [Programiz: Python JSON](https://www.programiz.com/python-programming/json). 



</details>

<details>

  <summary><strong>⭐ 3.3 Review: Solving Data Problems with Scripts (0:10)</strong></summary>
<br>

Take some time to walkthrough the previous activity and make sure you answer any student questions before moving on.

* Be sure to point out the following talking points:

  * The process of reading, manipulating, cleaning and writing CSV files may seem rather tedious right now. But don't worry. Next week we will cover the `Pandas` module, which has revolutionized how data scientists interact with tabular data within Python. 


</details>

---

### 4. <a name="Section4"></a> Getting the Most Out of Python Functions

| Activity Time:       0:25 |  Elapsed Time:      2:25  |
|---------------------------|---------------------------|

<details>

  <summary><strong>🎉 4.1 Everyone Do: Customizing your Python Experience (0:25)</strong></summary>

<br>

In this final programming activity, we will review the structure of a custom function in Python and practice designing and using a custom function. We will also introduce the concept of lambda functions and how they are used in map and apply functions. Lastly, we will bring everything together and apply both defined custom functions and lambda functions to list comprehension. 

Use the slideshow to introduce custom functions:

  * At this point, we should feel comfortable importing functions and methods from outside sources into our Python programs. However, it is imperative that we learn how to implement our own functions and methods in order to make our programs more efficient, easier to read and less repetitive. 

    * Within the field of coding there is a popular acronym: DRY.  It stands for **D**on't **R**epeat **Y**ourself** and essentially states that code should avoid having similar or repeating lines whenever possible.

    * By creating our own custom functions, we make our code more reusable and predictable, which means less time troubleshooting and testing in the long run.


#### Custom Functions Demonstration

In this demonstration, we will create more advanced Python scripts by incorporating custom functions, list comprehension, mapping and lambda functions. You can either continue using the slideshow to walk through this demonstration or use the [activity notebook](Activities/05-Ins_CustomizingPython/CustomizingPython.ipynb) to demonstrate live


1.  To create a new function or method, simply use `def <Function Name>():` and then place the code that you would like to run within the block underneath it.

    * In order to run the code stored within a function, the function itself must be called within the program. Functions will never run unless called upon.

      ```python
      # Create a basic function with no arguments
      def print_hello():
        print(f"Hello!")

      print_hello()
      ```

2. We can also define our own arguments that go into our functions. 

   * We can use **positional arguments** which must be provided in the proper order when using the function. 

      ```python
      # Create a basic function with positional arguments
      def print_name(name):
          print(f"Hello {name}!")

      print_name("Bob Smith")
      ```
   * We can also use **keyword arguments** which have a preassigned value and are often used as **optional arguments**. 

      ```python
      # Create a basic function with keyword arguments
      def print_name(lastname = "", firstname = ""):
          print(f"Hello {firstname} {lastname}!")

      # Printing with default values
      print_name()

      # Printing with non-default keyword arguments
      print_name(firstname="Bob",lastname="Smith")
      ```


3. When it comes to finishing our custom functions and methods, we need to make a decision: Should our function or method return a value when called or not? 

   * If the purpose of our custom function or method is to create a new object, then we should return the new object back to the user using a **return statement**. 
  
   * If our custom function or method is used to modify existing objects in memory, then we may not need to return anything back to the user.

      ```python
      # Demonstrate a custom function that returns a value back to the user
      def print_name(lastname = "", firstname = ""):
          return f"Hello {firstname} {lastname}!"
      text_to_print = print_name(firstname="Bob",lastname="Smith")
      text_to_print
      ```


4.  Let's try looking at a more complicated example using numbers. For example, what if we needed to calculate if a number is divisible by two and also calculate what the whole number and remainder of our division would be? We can build a custom script for that!

    * **Note:** Live-program this function with the students and make them critically think about how we can first calculate the whole number using floor division and then calculate the remainder using modulo.

      ```python
      # Demonstrate a custom function using numerical values
      def divide_with_remainder(number,divide_by=2):
          # Calculate the whole number and remainder when dividing by divide_by
          whole = number // 2
          remain = number % 2
          return (whole,remain)

      whole_number , remainder = divide_with_remainder(9,2)
      print(whole_number)
      print(remainder)
      ```

5. There are multiple ways we can use our custom functions and methods in our Python programs. Point out that we have already shown them two ways in this activity. We can use them to calculate new values and return them to the user. We can also use them to print out status updates to the user. Both of these uses help us limit the amount of code we would otherwise repeat.

   * Ask the students if they can come up with some other ways in which we can use custom functions. 

6. Another way we can limit the amount of code we write is by leveraging custom functions along with **list comprehension**.

    * List comprehension takes the `for` loop elements used in a list and consolidates the logic into a single line. Although list comprehension does not make our program do any less work than the traditional `for` loop, it does make smaller loops easier to read and navigate.
 
    * To use list comprehension, put your loop logic before your for-statement and wrap the entire statement in hard brackets `[]`.

      ```python
      # Demonstrate a simple list comprehension example
      my_list = [1,2,3,4,5,6,7,8,9]
      my_new_list = [x+2 for x in my_list]
      print(my_new_list)
      ```

   * List comprehension can be used to run custom functions too.

      ```python
      # Demonstrate how to use a custom function in list comprehension
      my_division_list = [divide_with_remainder(x) for x in my_list]
      print(my_division_list)
      ```

7. Let's practice putting these concepts together. Pose the following challenge to students:
  
    *  For the next two minutes, try to build a custom function that divides any number by seven then rounds up to the nearest hundredth  using `round(x,2)` where x is our newly divided number. Then, use list comprehension to apply your new custom function to the list `[24,654,3,961,21]`.

      * **Note:** This exercise may or may not take the full two minutes depending on the student body. Feel free to move on and just review this example if they finish early. 

      ```python
      # Create a custom function that divides by seven and rounds to the nearest hundredth 
      def divide_by_seven(num):
        return round(num / 7,3)
      print([divide_by_seven(number) for number in [24,654,3,961,21]])
      ```

    * Notice that we can assign any variable name in our list comprehension, just as we can in our `for` loops. In fact, we can use lists that contain other lists, tuples, or other collections in our list comprehension. As long as we are looping through a list, the possibilities are endless.

8.  A **map function** is another way to simplify our code as we traverse through columns and rows in a table, variables in a list or objects from an iterator object.

    * The **map function** is very similar to functions that use list comprehension because its purpose is to apply a function to each iteration in an iterable object. The major difference is that list comprehension can only work using a list, while a map function can be applied more generally. 

    * The `map()` function has two arguments: `fun` and `iter`.

      * The `fun` object is a function we wish to apply.

      * The `iter` object is the iterable object we want to apply `fun` across. 

    * To demonstrate how `map()` works similarly to our list comprehension example, we can use the following code:

      ```python
      # Recreate the previous list comprehension example using the map function
      list_comprehension = [divide_by_seven(number) for number in [24,654,3,961,21]]
      map_function = map(divide_by_seven,(24,654,3,961,21))
      print(list_comprehension)
      print(list(map_function))
      ```

9. In addition to being able to iterate over more generic iterable objects, map functions can also apply more abstract functions. Abstract functions in Python are known as **lambda functions** and they are smaller, shorthanded version of a custom function. 

   * **Lambda functions** are not stored as a defined function, instead they are executed within our `map()` function and their output is returned just like any normal custom function. 

    * In data science we will use lambda functions within a map function regularly, as it enables us to perform quick transformations in our data without taking the time and effort to store intermediary values. 

      ```python
      # Demonstrate how to implement our previous example as a lambda function within our map function
      map_function = map(lambda x: round(x/7,3),(24,654,3,961,21))
      print(list(map_function))
      ```

    * Notice that the lambda function first defines the arguments in front of the colon `:`. Then anything after the colon acts as the return statement from the abstract function. Finally, our `map()` function applies our iterable object normally. 

Encourage students that custom functions, list comprehension, mapping and lambda functions will become more familiar with time. As we progress through the curriculum, we will use these tools to help us create robust analysis scripts, compelling plots and visualizations and powerful data structures. 


 Be sure to answer any student questions before moving on. 

</details>

--- 

### 5. <a name="Section5"></a> Getting to know Git and End Class 

| Activity Time:       0:10 |  Elapsed Time:      2:50  |
|---------------------------|---------------------------|

<details>
  <summary><strong>📣 5.1 Instructor Do: Demonstrate Git and End Class (0:10)</strong></summary>
<br>

Before we end class, we need to give students a brief overview of Git and Github and get them familiar with the functionality. We will be re-introducing and reviewing Git in later units when students work on their end-of-module projects.

* Explain to students that so far, GitHub has only been used as a sort of drop box to store our files. Although GitHub works well this way, it has far greater capability. Today, we will explain what what Git is and how we can use it to interact with Github on the terminal.

* **Note**: If teaching with VS Code, consider using the [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory) extension to illustrate this section's concepts.

Introduce Git and version control by covering the following: 

* Explain that Git is essentially a way for us to keep track of our work over time.

* Whenever we get another piece of a project working, we can save the change with Git.

* This "save" is called a **commit** and it represents a "checkpoint" for our project.

* If we break something in our code while developing, this system allows us to restore the working code from before.

![A commit is a lot like a changelog note](https://cdn-images-1.medium.com/max/1600/1*zj-d8TopjgBml2QVM-672w.jpeg)


* Since Git remembers these "checkpoints", we can work on several different concerns all at once.

  * Suppose we need to analyze Uber ride data for our project.

  * Explain that we might decide to analyze the average age of riders. Git essentially allows us to write this code, and save it with the name: `age analysis`.

  * Emphasize that this code is different from the code we started with, and that it lives separately from it.

  * In this scenario we have a version of the code, called `main`, which is the "main" version of our code; and a version called `age analysis`, which contains updates.

* Explain that each version of the code lives on a different **branch**.

  * A **branch** is essentially a history of changes.

  * In this case we say that the `age analysis` branch **diverged** from the `main` branch.

* Take a moment to demonstrate the difference between the files on the `age_analysis` and `main` branches.

  * Explain that saving the age analysis code in a different branch gives our teammates a chance to review it for errors and offer suggestions.

  * After the proposed change has been reviewed, we can update the `main` branch to include the changes in `age analysis` by doing a **merge**.

* Explain that historically, the most common name for the main body of a codebase has been **master**. However, **main** has recently been gaining in popularity. In fact, GitHub now uses **main** as the default name for its repositories -  as do the projects in this course. Be aware that you might see instances of both throughout your development career, or hear experienced coders use the term "master branch" out of habit."

* Explain that **merging** two branches turns them into one.

* Explain that this is how we can work on new features or bugfixes without making changes to code we know is working.

  * Explain that this also makes it easier to work with teammates, as people can avoid stepping on each others' toes by working on different branches.

* Finally, take a moment to review Git's "Snapshot model" as it's explained in [Git's official documentation](https://git-scm.com/book/be/v2/%D0%9F%D0%B5%D1%80%D1%88%D1%8B%D1%8F-%D0%BA%D1%80%D0%BE%D0%BA%D1%96-Git-Basics):

  > "...Git thinks of its data more like a set of snapshots of a miniature filesystem. Every time you commit, or save the state of your project in Git, it basically takes a picture of what all your files look like at that moment and stores a reference to that snapshot. To be efficient, if files have not changed, Git doesn’t store the file again, just a link to the previous identical file it has already stored. Git thinks about its data more like a stream of snapshots."

  ![Git Snapshot Model](https://git-scm.com/book/en/v2/images/snapshots.png)

* Next week, students will continue learning about Git when they create a git repo for development work. They will also practice committing, stashing and reverting changing on the command line.  

* Make sure to answer any student questions about Git, or any lingering Python programming questions before ending class.

</details>  

---

### 6. <a name="Skill_Drill"></a> Skill Drill Take Home

<details>
  <summary><strong>📣 6.1 Student Do: Python Programming Skill Drill </strong></summary>
<br>

In today's take-home skill drill activity, students will build a basic script that reads in time-series stock data, calculates percent change for each day and prints out information for the day with the greatest absolute percent change. 

* **Files:**

  * [README](../../../02-Assignments/01-Introduction/02-Programming_With_Python/README.md)

  * [02-Assignments/Unsolved/StockSkillDrill_Unsolved.ipynb](../../../02-Assignments/01-Introduction/02-Programming_With_Python/Unsolved/StockSkillDrill_Unsolved.ipynb)

#### Instructions:

1. Import both the `os` and `csv` libraries to your notebook.

2. In your notebook, set a path for importing the CSV file using `os.path.join()`.

3. Open a connection to the comma-delimited CSV file and read in the CSV file using `csv.DictReader()` class.

4. Create a variable to save our output row named `printrow` and greatest daily percent change named `max_pct`.

5. Iterate through each row and calculate the daily percent change. Be sure to round the percent change to the nearest hundredth. 

   * **Note:** Percent change is calculated by the following formula:

      * (`Closing price` - `Opening price` / `Opening Price`) * 100

6. While looping through each row, determine which day had the absolute greatest percent daily change. 

   * **Hint:** Determine if the absolute daily percent change is greater than the previous greatest percent change. If the newly calculated absolute percent change is greater, store the output row to the `printrow` variable and greatest daily percent change to the `max_pct` variable.

   * **Note:** Absolute values ignore positive or negative direction. Check out [this tutorial](https://www.tutorialspoint.com/How-to-calculate-absolute-value-in-Python) on absolute value for more information. 

7. After looping through all rows, print out the date, stock high, stock low, volume and percent change for the day with the greatest absolute percent change.

</details>  

---

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
