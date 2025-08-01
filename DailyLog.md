# DailyLog is about my Learning throughout the day.<br><br>

#Day - 1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-  Learned about Void Pointer and NULL pointer.<br>
(04/07/2025)<br><br>

==========================================================================================<br><br>

## Void Pointer: A generic pointer<br>
It is a Pointer that can hold any data type address, but we need to exclusively define it.<br><br>

### Example:<br><br>

<pre><code>int x = 10;
void *ptr = &x;

printf("%d", *(int *)ptr); // 10
printf("%d", *ptr); // Can't do like this.
</code></pre>

## NULL Pointer: It is like defining NULL to pointer then assigning values whenever need it.<br>
// If we don't declare NULL then it might print Garbage Value.<br><br>

### Example:<br><br>

<pre><code>int *ptr = NULL;
int choice = 1;

if(choice) {
  ptr = (int *)malloc(sizeof(int));
  *ptr = 42;
}

if(ptr != NULL) 
  printf("%d", *ptr); // 42
else
  printf("This pointer is NULL.");
</code></pre>

<br>

#Day - 2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-  Learned about Dangling Pointer & Wild Pointer.   <br>
(05/07/2025)<br><br>

==========================================================================================<br><br>

## Dangling Pointer: It is like freeing the Pointer and then trying to access it.<br>
If we try to access it we might get Garbage Value.<br><br>

### Example:<br><br>

<pre><code>int a = 10;
int *ptr = (int *) malloc(sizeof(int));
free(ptr);
printf("%d", *ptr); // This is Dangling Pointer
ptr = NULL; // This becomes NULL Pointer now
</code></pre>

## Wild Pointer : It is like not assigning value to the pointer but then trying to dereference it.<br><br>

### Example:<br><br>

<pre><code>int a = 24;
int *ptr;

printf("%d", *ptr); // This is a Wild Pointer.
</code></pre>

<br>

#Day - 3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-  Did Matrix Multiplication.<br>
(06/07/2025)<br><br>

==========================================================================================<br><br>

## Matrix Multiplication  <br>
- Tried doing Matrix Multiplication of 2D matrix and got succeeded.  <br>
- Used functions and user inputs to get the size of the Matrix.<br><br>

## Preprocessor Directives  <br>
Learned about:  <br>
<code>#include</code>, <code>#define</code>, <code>#undef</code>, <code>#ifdef</code>, <code>#ifndef</code>, <code>#if</code>, <code>#else</code>, <code>#elif</code>, <code>#endif</code><br><br>

<b>#include</b> <br>
- To include another file.  <br>
<pre><code>#include &lt;stdio.h&gt;
#include "myfile.h"
</code></pre>

<b>#define</b><br>
- To define a constant or macro.<br>
<pre><code>#define PI 3.14
</code></pre>

<b>#undef</b><br>
- To undefine a macro which was defined earlier.<br>
<pre><code>#undef PI
</code></pre>

<b>#ifdef</b><br>
- To check if macro is actually defined.<br>
<pre><code>#define DEBUG

#ifdef DEBUG
  printf("It is defined.");
#endif
</code></pre>

<b>#ifndef</b><br>
- To check if macro is not defined. If not defined you can define it.<br>
<pre><code>#ifndef PI
#define PI 3.14
#endif
</code></pre>

<b>#if, #else, #elif, #endif</b><br>
- Used for conditional compilation for macros.<br>
<pre><code>#define VALUE 5

#if VALUE == 5
  printf("The value is 5\n");
#elif VALUE == 10
  printf("The value is 10\n");
#else 
  printf("Value is something else.");
#endif // Closes all blocks like #if, #ifdef, #ifndef.
</code></pre>


#Day - 4 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-  Did Matrix Multiplication.<br>
(07/07/2025)<br><br>

==========================================================================================<br><br>


## Palindrome Numbers  <br>
- Tried the logic of Palindrome numbers using functions.  <br>

## File Input/Output <br>
Learned about:  <br>
<code>fopen()</code>, <code>fclose()</code>, <code>fgetc()</code>, <code>fgets()</code>
- Tried making a bill replacing string in Pre-written file.


#Day - 5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-  Did Matrix Multiplication.<br>
(08/07/2025)<br><br>

==========================================================================================<br><br>


## File Input/Output <br>
Learned in detail about:  <br>
<code>fopen()</code>, <code>fclose()</code>, <code>fgetc()</code>, <code>fgets()</code>, <code>fputc()</code>, <code>fputs()</code>
- Completed making a bill replacing string in Pre-written file.

<b>fopen()</b><br>
- To open any file either <b>Text file</b> or <b>Binary file</b>
- There are many mods by which we can open files, <b>r, w, r+, w+ rb</b>

<b>fclose</b><br>
- After opening a file and completing task you must close the while which was opened.
- fclose automatically closes the file which was opened earlier.


#Day - 6 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-  Learned about File Modes in detail & Command line Arguments.<br>
(09/07/2025)<br><br>

==========================================================================================<br><br>


<b>fgetc()</b><br>
- To get a single character from the file.

<b>fgets</b><br>
- fgets() is almost same as fgetc() the difference is that while fgetc() was used to get a single character, fgets() is used to get string of characters.

<b>fputc()</b><br>
- To enter a single character in a file. 
- If the file is in "w" write mode then first it cleans the file and then writes the content.

<b>fputs()</b><br>
- Same as fputc(), The main difference is that fputs() is used to pass the string of characters to file.
- Also same here, If the file is in "w" write mode then first it cleans the file and then writes the content.

## Command Line Arguments <br>

## 🔢 Command Line Arguments

I practiced how to use **command line arguments in C**.

### Code Overview
I created a calculator program that:
- Accepts an **operation type** (`add`, `subtract`, `multiply`, `divide`)
- Accepts **two numbers**
- Performs the selected operation using `argv[]` and `atoi()`

### Example Command:
./calculator add 10 5

# Day - 7         -  Practiced C problems & patterns.  
(10/07/2025)

==========================================================================================

## C Problem Solving
- Print N natural numbers  
- Sum of digits of a number  
- Reverse a number  
- Check even or odd  
- Check prime or not  
- Factorial using loop  
- Print Fibonacci series up to N  
- Check palindrome number  
- Print multiplication table of N  
- Count number of digits in a number  
- Find max of 3 numbers using if-else  
- Simple calculator (menu-based)  
- Patterns:
- Check if character is vowel or consonant  
- Sum of first N odd numbers

  _Practiced locally, not yet uploaded to GitHub._


# Day - 8         -  Started Web Development + Practiced C Array  
(11/07/2025)

==========================================================================================

## Web Development  
- Created base folder structure for `HTML`, `CSS`, and `JS`.  
- Started learning basic HTML: tags, structure, usage.

## C Practice  
- Find second largest element in an array.  
- Organizing files & folders (many commits due to setup work).

# Day - 9         -  Continued HTML/CSS and String Exercises in C  
(12/07/2025)

==========================================================================================

## Web Development  
- Practiced basic HTML & CSS.  
- Used tags for headings, paragraphs, images, lists, and links.

## C Programming  
- Check if string is palindrome  
- Count vowels, consonants, digits in a string 

# Day - 10 - CSS Selectors + Practiced Advanced C Programs 
(13/07/2025)

==========================================================================================

Web Development
------------------

- Learned in detail about **CSS Selectors**  
  - Universal selector (`*`)  
  - Element selector (`p`, `h1`, etc.)  
  - ID selector (`#id`)  
  - Class selector (`.class`)  
  - Grouping selectors  
  - Descendant & Child selectors  
  - Pseudo-classes like `:hover`, `:first-child`, `:nth-child()`  

C Programming
----------------

- Find GCD and LCM of two numbers  
- Convert lowercase to uppercase (without `strupr()`)  
- Copy one string to another (without `strcpy`)  
- Count frequency of each element in an array  
- Find missing number in array of 1 to N  
- Check Armstrong number  
- Find all prime numbers between 1 to N  
- Transpose a matrix  
- Check if two strings are anagrams  

---

# Day - 11 - CSS Box Model & More String Exercises in C  
(14/07/2025)

==========================================================================================

Web Development
------------------

- Explored **Box Model**, including:  
  - Content  
  - Padding  
  - Border  
  - Margin  

- Learned about **Color Properties**  
  - Named colors  
  - Hex  
  - RGB  
  - HSL  

- Did a small **HTML/CSS exercise** using `div` and background-color  

C Programming
----------------

- Merge two sorted arrays  
- Reverse a string using function  

---

# Day - 12 - CSS Display Properties + Made a Project in C  
(15/07/2025)

==========================================================================================

Web Development
------------------

- Learned about **CSS Display Properties**  
  - `block`, `inline`, `inline-block`, `none`  
- Studied **Specificity** and selector weight  
- Covered basic **sizing units**:  
  - `px`, `em`, `rem`, `%`, `vh`, `vw`  

C Programming
----------------

**Student Record System Project**

- Created a menu-based student record system using `struct` and arrays  
- Features implemented:  
  - `struct Student` with fields: `roll_no`, `name`, `marks`  
  - Array of `Student` to hold multiple records  
  - Functions for:  
    - Add new student  
    - Display all students  
    - Search by name or roll number  
    - Update student details

# Day - 13 - List Styling & Completed StudentRecordSystem + FileIO  
(16/07/2025)

==========================================================================================

Web Development
------------------

- Learned about `list-style-type`, `list-style-position`, and `list-style-image` for custom bullets.
- Explored `text-shadow` and `box-shadow` for adding depth and effects to elements.
- Understood the usage of `outline` vs `border`, and how `outline-offset` works.
- Tried different combinations of list styles and shadows for practice.
- Practiced using `ul`, `ol`, and `li` with nested lists and icons.

C Programming
----------------

- Reviewed the `StudentRecordSystem.c` project.
- Added basic error checking for user input.
- Analyzed how `struct`, `FILE *`, and loops work together in a mini system.

---

# Day - 14 - Web Dev Revision + Made Tic-Tac-Toe  
(17/07/2025)

==========================================================================================

Web Development
------------------

- Revisited key HTML tags (`form`, `input`, `label`, `nav`, `section`, etc.).
- Reviewed and tested all previous CSS topics like display types, positioning, and specificity.
- Updated old files to improve code structure, added comments, and cleaned unused code.
- Practiced a few mini-layouts with `flexbox` and added hover effects.

C Programming
----------------

- Completed **Tic-Tac-Toe** project (Single-player vs Computer).
- Used 2D arrays to create the game board.
- Implemented a basic AI for the computer moves (random empty cell selection).
- Created a menu loop so users can play multiple games without restarting.
- Improved user interface in console using clean prompts and board redraws.
- Added simple score tracking (wins/losses/draws in a session).

# Day - 15 - CSS Position & Overflow + Started C++
(18/07/2025)

==========================================================================================

Web Development
------------------

- Learned about the CSS **overflow** property (`hidden`, `scroll`, `auto`).
- Studied the **position** property (`static`, `relative`, `absolute`, `fixed`).
- Completed **Exercise 3**, which involved creating a responsive card element.
- Applied various CSS styles to complete the design of the exercise card.

C/C++
------------------

- Created a new `cpp-programs` folder to begin learning C++.
- Marked a fresh start into C++ programming, moving from C.

---

# Day - 16 - Media Queries & C++ Basics
(19/07/2025)

==========================================================================================

Web Development
------------------

- Learned about **Media Queries** to create responsive web layouts.
- Completed **Exercise 4**, which focused on building a responsive navigation bar.

C/C++
------------------

- Studied the basic theory and syntax differences between C and C++.
- Wrote and executed the first C++ program, `helloworld.cpp`.

---

# Day - 17 - CSS Float/Clear & C++ Fundamentals
(20/07/2025)

==========================================================================================

Web Development
------------------

- Learned about the **float** property to allow elements to float next to each other.
- Understood how to use the **clear** property to stop elements from wrapping around a float.

C/C++
------------------

- Learned about **variables** and taking user **inputs**.
- Practiced using **type casting** to convert data types.
- Worked with different C++ operators:
  - **Arithmetic** Operators
  - **Relational** Operators
  - **Logical** Operators
  - **Unary** Operators
- Wrote a simple program to find the **sum of two** numbers.

# Day - 18 - C++ Control Flow & Web Dev Review
(21/07/2025)

==========================================================================================

## Web Development
---
- Reviewed all previously learned HTML and CSS concepts to reinforce understanding.

## C++
---
- Learned about control flow structures: `if-else`, `if-else-if`, `for` loops, and `while` loops.
- Practiced using the **ternary operator** for concise conditional statements.
- Wrote programs for:
    - Checking if a number is **even or odd**.
    - Determining if a character is **uppercase or lowercase**.
    - Calculating the **sum of numbers from 1 to N**.
    - Calculating the **sum of odd numbers from 1 to N**.

---

# Day - 19 - C++ Loops & Patterns
(22/07/2025)

==========================================================================================

## Web Development
---
- Conducted another thorough check of previous HTML/CSS topics to ensure solid fundamentals.

## C++
---
- Learned about the **do-while loop** and the concept of **nested loops**.
- Wrote programs to solve classic problems:
    - Checking if a number is **prime**.
    - Printing a **simple pyramid pattern** using nested loops.

---

# Day - 20 - Academic Focus
(23/07/2025)

==========================================================================================

- No new topics were covered in Web Development or C++ due to academic commitments with the start of college.

---

# Day - 21 - C++ Pattern Programming
(24/07/2025)

==========================================================================================

## Web Development
---
- Paused web development studies to focus on academic priorities.

## C++
---
- Continued practicing **nested loops** by creating various patterns:
    - **Square** pattern.
    - **Triangle** patterns using stars, numbers, and characters.
    - **Floyd's Triangle**.

---

# Day - 22 - More C++ Patterns
(25/07/2025)

==========================================================================================

## Web Development
---
- No new web development topics were covered.

## C++
---
- Practiced creating more complex patterns, including the **reverse triangle pattern**.

---

# Day - 23 - C++ Functions & Advanced Patterns
(26/07/2025)

==========================================================================================

## Web Development
---
- No new web development topics were covered.

## C++
---
- Learned about **functions** in C++ for creating modular and reusable code.
- Implemented functions to:
    - Calculate the **sum of numbers from 1 to N**.
    - Find the **factorial** of a number.
- Expanded pattern programming skills with:
    - **Inverted triangle** and **pyramid** patterns (using stars, numbers, and characters).
    - **Hollow diamond** pattern.
    - Consolidated different pattern variations into single, more flexible programs.

---

# Day - 24 - Advanced CSS & Layout Exercises
(27/07/2025)

==========================================================================================

## Web Development
---
- Learned about more **advanced CSS selectors**.
- Completed **Exercise 4**, which involved creating a navigation bar with an external stylesheet.
- Completed **Exercise 5**, creating a page layout with:
    - A navigation bar and footer.
    - A main content area with two distinct sections.
    - A floating icon using `position: fixed` that remains visible on top of all other elements.

## C++
---
- Practiced creating more complex patterns, including the **reverse triangle pattern**.
- Also, Revised old methods properly.
- Tried some exercises locally.

---

# Day - 25 - C++ basic exercises.
(28/07/2025)

==========================================================================================

## Web Development
---
- No new web development topics were covered.

## C++
---
- Did some exercise, One to find the sum of the digits of a number and second one of Learned the topic PassbyValue.

---
