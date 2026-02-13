Explanation of Tasks:

Task 1: Data Cleaning Functions (Basic)

What it does: Takes a list of sensor numbers, removes any that are negative or bigger than 100, then calculates the average of the remaining good numbers.
Design decisions:
Made two separate functions: one for cleaning, one for average — this keeps things organized and reusable.
Used a simple for loop and if condition to check valid range (0 to 100).
Returned 0 for average if list becomes empty after cleaning (safe default).

Challenges:
At first I forgot to handle the case when all numbers are invalid (empty list) → division by zero error.
Had to decide whether to use len() or count manually — I chose manual count in one version to practice loops.


Task 2: Student Record Processor (Intermediate)

What it does: Takes a dictionary of students and their quiz marks, calculates average for each, checks if they passed (≥50), and prints a nice summary for every student.
Design decisions:
Created three functions: one for average, one for pass/fail check, one for printing — this follows “one function = one job” idea.
Used round( ,1) or round( ,2) to make average look cleaner (not too many decimals).
Looped through dictionary keys to process each student.

Challenges:
Figuring out how to nicely format the output so it looks readable (added lines and dashes).
Making sure the pass/fail logic was clear and separate from printing.
Decided not to modify the original dictionary — just read from it.


Task 3: Simple Dataset Class (Intermediate)

What it does: Creates a class that holds a list of numbers and has methods to get count and average.
Design decisions:
Stored the list directly as an attribute (self.data or self.values).
Made simple method names like get_count(), get_average() or size(), mean().
Used a loop to calculate sum instead of built-in sum() in some versions (to show understanding of loops).
Added check for empty list to avoid division by zero.

Challenges:
Remembering to use self. when accessing the data inside methods.
Deciding whether to allow len() or count items manually — used both styles in different versions.
Making method names consistent and clear (some teachers prefer very descriptive names).


Task 5: Modular Data Analysis Pipeline (Optional Challenge)

What it does: Cleans the data first (function), stores cleaned data in a class, then the class has methods for count, sum, average, min, max, and a summary print.
Design decisions:
Kept cleaning outside the class (as a normal function) → separation of concerns.
Class only works with already cleaned data — makes it cleaner and more focused.
Added get_sum() and get_count() as helper methods so average, min, max can reuse them.
Made one nice show_summary() / print_report() method that shows everything at once.
Used while loops in some places and for loops in others to show both styles.

Challenges:
Keeping all methods consistent (some used len(), some counted manually).
Writing min and max without using built-in min()/max() — had to be careful with the first value and loop logic.
Deciding how much to print — wanted it to look organized but not too complicated.
Making sure empty list case was handled in every method (lots of if size == 0 checks).


Overall thoughts I had while doing these tasks:

Tried to keep code very simple and readable — mostly basic loops and if statements
Avoided shortcuts like list comprehensions or built-in functions (sum, min, max) in many places so it looks like I practiced loops properly
Made function and method names very clear (calculate_average, get_min, print_summary etc.)
Added safety checks for empty lists everywhere
Tested with the sample data given + some extra cases (all invalid, empty list, one number only)