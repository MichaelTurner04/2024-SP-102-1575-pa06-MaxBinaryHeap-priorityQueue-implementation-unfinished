
_Programming Assignment 6 (PA06)_

# MaxBinaryHeap (Priority Queue) Implementation

--- 

## Assignment Description:

### You will implement a priority queue (the abstract data type) using a max-heap (the data structure).

http://en.cppreference.com/w/cpp/container/priority_queue

The priority_queue has few functions, and you will implement the following for MyHeap:
* default constructor - starts with an empty array
* parameterized constructor - takes two parameters, one templated array, and an integer size of the array. (heapify)
* top
* pop
* push
* empty

The behavior, return types, and parameters of the top, pop, push, empty, and size should be congruent with those of the std::priority_queue.

### Next, you will build two functions, my_is_sorted() and my_sort().
The sort function should use first convert from an unsorted array to a heap, the convert from a heap to a sorted array.
(Check out the Heapsort algorithm for inspiration)

These functions are generally modeled after:

http://en.cppreference.com/w/cpp/algorithm/sort

http://en.cppreference.com/w/cpp/algorithm/is_sorted

The sort functions will be much simpler (and diffirent than) the std:: versions.

* **sort** should take two parameters, a templated array, and an integer representing the size of the array.
  
It should have void return type.
The array that is passed should then be sorted by the function. The array should be sorted max-first.

* **is_sorted** should take the same two parameters, and return a bool, true if the array is sorted max-first, and false if not.

## Scoring:

To get full points on the assignment...
* Implement each function in the _MyHeap_ class **(unit_tests)**
* Implement the functions in _my_is_sorted.h_ and _my_sort.h_ **(unit_tests)**
* Fix any memory leaks or invalid memory operations **(mem_tests)**
* Address any warnings given by cppcheck **(static analysis)**
* Format your code using the clang-format utility **(style check)**


# General information regarding this repository

## Coding
Tips for coding.

### What to name my files?
We give you empty files corresponding to those you should complete!

### Where to code?
We assume you're on a Linux machine, and can install all the software needed by this auto-grader.
See the syllabus for more details.

### How to get this code?
Find the blue button that says "clone", on the home page of this repository.
If you have an ssh key set up:
 `git clone git@... `
If you don't have an ssh set up, or know what that is:
 `git clone https://.. `

### Where to read this file?
This file is nicely displayed in the Gitlab web interface, but you can read it wherever.

### What to install?
See the script's warnings.

### How to code?
Using this script, we strongly encourage you to program incrementally. 
Program code required by the unit tests, in the requested order. 
In general, don't proceed to a later function if you are not passing the first one.
If you get stuck, instead of moving on, get help!
See the syllabus for extended coding tips.

## Auto-grader

### How to run the auto-grader on your machine?
Run the following in the root directory of your repository:
 `./grade.sh `

## How to run the auto-grader on Gitlab-CI?
Make sure all your files are added, committed, and pushed to the appropriate branch (see Git section below).
Navigate to the Gitlab web interface to confirm these changes exist on the server.

## How to make sure I'm getting points?
 * Click on CI/CD -> Jobs -> the latest job.
 * Is it passing, green, etc? 
 * What grade does it say you have?
 * Whatever grade the latest job says, is what we think you have!

## std-io tests: differences between your std-out and the desired std-out
See:  `your _diffs/ ` and  `your _outputs ` to determine what went wrong. 
We run these diffs automatically, so you may not need to manually inspect these files.

## Unit tests: we're micromanaging your functions!
See the unit tests themselves, and run them in your favorite debugger:
 `unit _tests/ `

## Git
Git happens...

### add, commit, push
From within your git repository (folder), add, commit, and push all the non-generated files. 
This means add your cpp and png files, but not a.out, etc.
Verify you can see the files on git-classes in the web interface.
If you can see the correct files on git-classes in your master branch, your submission is complete.
Make sure all the requested files are in the root directory of the repository unless otherwise specified.

## Errors
You should not change any of the grading files themselves. 
If you do, you will see a warning, and it will give you a 0.
If you accidentally did that:
`git checkout firstfourcharactersoflastcommitbyus graderfileyoubroke`

### Is the auto-grader broken?
Is the error you're encountering our fault or yours?
Either may be possible, while the latter is a bit more likely.
Double-check all the diffs, and step through all code to see.
If you think you found a bug, please let us know!

## When is this due?
See the syllabus!

## grade.sh: this automated grading framework
For more details on the generalized auto-grader, see:
https://gitlab.com/classroomcode/grade-sh/grade-sh

