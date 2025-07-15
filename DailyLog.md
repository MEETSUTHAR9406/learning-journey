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
