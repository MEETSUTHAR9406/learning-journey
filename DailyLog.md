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

# Day - 26 - Flexbox & Fibonacci
(29/07/2025)

==========================================================================================

## Web Development
---
- Dove into **CSS Flexbox**! Layouts are starting to feel less like a puzzle and more like building with LEGOs.
- Learned that Flexbox is a one-dimensional layout model, which makes it super easy to align items in a row or column and distribute space among them.
- Created both the `.html` structure and the corresponding `.css` to practice arranging items, which is a game-changer for responsive design.

## C++
---
- Tackled a classic combinatorial problem: calculating **nCr** (the number of combinations).
- Completed **Exercise 3**, which was to print the **Fibonacci sequence** up to a given number of terms.

---

# Day - 27 - Loops & Number Systems
(30/07/2025)

==========================================================================================

## Web Development
---
- Dedicated the day to **reviewing CSS**. Went over Flexbox again to really solidify the concepts and revisited other layout properties to make sure everything was fresh in my mind.

## C++
---
- Practiced a variety of fundamental problems:
    - **Binary to Decimal** conversion.
    - A simple program to check if a number is **Odd or Even**.
    - Calculating the **sum of numbers from 1 to N**.
- Got familiar with the **do-while loop**, understanding how it guarantees at least one execution.
- Updated **Exercise 1** (printing prime numbers up to N) with better comments for clarity.

---

# Day - 28 - CSS Grid & Prime Functions
(31/07/2025)

==========================================================================================

## Web Development
---
- Learned about **CSS Grid**, the powerful two-dimensional layout system. It's amazing for creating complex, grid-based layouts with both rows and columns. 
- Practiced managing tracks (rows and columns), placing items, and creating responsive grids.
- Completed an additional exercise to put Grid into practice on a sample webpage layout.

## C++
---
- Wrote a program to check if a given number is **prime or not**, but this time I structured the logic inside a reusable **function**.
- Implemented **Decimal to Binary** conversion, the reverse of yesterday's exercise.

---

# Day - 29 - Bitwise Operators
(1/8/2025)

==========================================================================================

## Web Development
---
- A pretty straightforward day focused on **reviewing** previous HTML and CSS concepts to keep them sharp.

## C++
---
- Opened up a new topic: **bitwise operators**. It's fascinating to see how you can manipulate individual bits of data.
- Learned about the core bitwise operators: `AND (&)`, `OR (|)`, `XOR (^)`, `NOT (~)`, `Left Shift (<<)`, and `Right Shift (>>)` .

---

# Day - 30 - Bitwise Operations
(2/8/2025)

==========================================================================================

## Web Development
---
- Another day spent **reviewing** and consolidating web development knowledge.

## C++
---
- Got hands-on practice with the bitwise operators learned yesterday.
- Specifically performed operations using:
    - **Bitwise OR (`|`)**
    - **Bitwise AND (`&`)**
    - **Bitwise Shift (`<<` and `>>`)**

---

# Day - 31 - Scope & Precedence
(3/8/2025)

==========================================================================================

## Web Development
---
- A quick **review** session on the web development front.

## C++
---
- Dived into some important C++ theoretical concepts:
    - **Operator Precedence**: Learned the order in which C++ evaluates different operators in an expression.
    - **Scope**: Understood the difference between local and global variables and where they can be accessed.
    - **Data Type Modifiers**: Explored modifiers like `signed`, `unsigned`, `short`, and `long` to alter the range of values a data type can hold.

---

# Day - 32 - CSS Transform & UI Cloning
(4/8/2025)

==========================================================================================

## Web Development
---
- Learned how to use the CSS **`transform` property** to `translate`, `rotate`, `scale`, and `skew` elements. It's really cool for adding depth and interactivity.
- Started a new project: cloning the UI of the **UltraEdit download page**. 
- Successfully built the navigation bar and used **CSS Grid** for the main content area. Made it about halfway through the page.

## C++
---
- A day dedicated to **reviewing** previous C++ topics and exercises.

---

# Day - 33 - Arrays & Pass by Reference
(5/8/2025)

==========================================================================================

## Web Development
---
- Followed a tutorial to create a **glowing button** effect with CSS. It was a fun exercise in using shadows and animations, though not built from scratch myself. 

## C++
---
- Introduced to a fundamental data structure: the **array**.
- Wrote a program to find the **minimum and maximum** elements within an array.
- Learned about **pass by reference**, a crucial concept for allowing functions to modify the original array arguments directly, which is much more efficient than copying.

---

# Day - 34 - Transitions & Animations
(6/8/2025)

==========================================================================================

## Web Development
---
- Explored CSS **`transitions`** and **`animations`**.
- Understood that transitions provide a smooth change between states (like on hover), while animations allow for more complex, multi-step sequences using `@keyframes`.

## C++
---
- A solid **review** session, going over arrays and function concepts from yesterday.

---

# Day - 35 - Array Algorithms
(7/8/2025)

==========================================================================================

## Web Development
---
- Spent the day **reviewing** CSS animations and other recent topics.

## C++
---
- Practiced more array manipulation algorithms:
    - Implemented **linear search** to find an element in an array.
    - Wrote a function to **reverse the elements** of an array in place.
- Solidified my understanding of the **for loop** for iterating over arrays.

---

# Day - 36 - Bouncing Ball Animation
(8/8/2025)

==========================================================================================

## Web Development
---
- Created a **bouncing ball animation** using CSS! 
- This was a great practical exercise that combined the `animation` property with `@keyframes` to create continuous, realistic motion.

## C++
---
- Another day of **reviewing** C++ fundamentals, especially array-based problems.

---

# Day - 37 - Sum of Array
(9/8/2025)

==========================================================================================

## Web Development
---
- A quick **review** day for web development concepts.

## C++
---
- Wrote a C++ program to calculate the **sum of all numbers** within an array. A simple but essential algorithm to know.

---

# Day - 38 - Netflix Clone & CSS Filters
(10/8/2025)

==========================================================================================

## Web Development
---
- Learned about the CSS **`object-fit`** and **`object-position`** properties, which are super useful for controlling how images and videos fit within their containers without getting distorted.
- Explored CSS **`filter`s** like `blur()`, `brightness()`, and `grayscale()` to apply graphical effects to elements.
- **Started a major new project: a UI Clone of Netflix!**  Created a new folder in my `fullstack-journey` repository to get things started.

## C++
---
- A day dedicated to **reviewing** various C++ topics covered so far.

---

# Day - 39 - Vectors & Netflix Clone Progress
(11/8/2025)

==========================================================================================

## Web Development
---
- Made some good progress on the **Netflix UI clone**. It's starting to take shape.

## C++
---
- Learned about C++ **`std::vector`**, the dynamic array of the C++ world.
- Studied common vector **methods and functions**, such as:
    - `push_back()` to add elements.
    - `pop_back()` to remove elements.
    - `size()` to get the number of elements.
    - `begin()` and `end()` for iterators.

---

# Day - 40 - Netflix Navbar & C++ Practice
(12/8/2025)

==========================================================================================

## Web Development
---
- Focused on the **Netflix UI Clone** and almost completed the navigation bar. It's looking pretty close to the real thing!

## C++
---
- Updated Exercise1
