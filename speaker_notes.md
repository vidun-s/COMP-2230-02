# Speaker Notes: Course Introduction and Lab 1 Big O Analysis

## Opening and GitHub Repo Setup

"Good evening, everyone! Welcome to COMP 2230-02: Data Structures, Algorithm Analysis, and Program Design. Today we're going to get you set up and running with your first lab on Big O analysis.

Before we dive into Java programming, let's make sure everyone has their own personal repository set up. This will be your workspace for the entire course.

To create your personal repository:

1. Go to GitHub.com and sign in
2. Click the '+' icon and select 'New repository'
3. Name it something like 'COMP-2230-my-work'
4. Make it public or private as you prefer
5. **Important**: Do NOT initialize with README, .gitignore, or license
6. Click 'Create repository'

Now, you have two main options to get the course materials:

**Option 1 - Clone and Push:**
- Open your terminal and run: `git clone https://github.com/ShivaniTyagiCS2026/COMP-2230-02.git`
- Then: `cd COMP-2230-02`
- Connect to your new repo: `git remote set-url origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git`
- Push: `git push -u origin main`

**Option 2 - Download ZIP:**
- Go to the course repo and click 'Code' → 'Download ZIP'
- Extract the files
- Upload them to your new GitHub repository

This gives you complete independence - you can modify freely without affecting the original course repo."

## Java Introduction Overview

"Now that you have your repository, let's talk about Java. Java is a high-level, object-oriented programming language that we'll use throughout this course for implementing data structures and algorithms.

Key concepts you'll need:
- Classes and Objects: Everything in Java is organized into classes
- Main Method: `public static void main(String[] args)` is your program's entry point
- Variables: Declare with types like `int x = 5;`
- Methods: Functions inside classes
- Packages: For organizing code

In this course, we'll focus on clean, readable code with comments. We'll start with procedural programming and move into object-oriented concepts as we implement data structures.

The Java 101 introduction folder covers:
- Basic syntax (variables, data types, operators)
- Control flow (if-else, loops)
- Methods (functions)
- Classes and objects
- Arrays
- Input/output

Take some time to explore these folders and run the examples."

## Running Lab 1 Lecture Examples

"Let's move into Lab 1: Big O Analysis. Big O notation describes algorithm performance and complexity. We'll focus on time complexity today.

First, let's look at the lecture examples. Open your terminal and navigate to the lab01_big_o_analysis folder. Then go into lecture_example.

Let's run LectureExample1.java first. This demonstrates O(n) complexity.

Compile it: `javac LectureExample1.java`
Run it: `java LectureExample1`

You'll see it prints numbers from 0 to 9 and shows the total. The code has F(n) = 2n + 1 operations - one initialization plus two operations per loop iteration (increment and print). As n grows, the dominant term is 2n, so it's O(n).

Try changing n to different values and see how the output changes.

Now let's look at LectureExample2.java - this shows O(n²) complexity with f(n) = 3n² + 2n + 1000*log(n) + 5000. The dominant term is 3n².

And LectureExample3.java shows O(n³) with f(n) = 3n³ + 2n² + 5n + 1.

Run these and observe how they behave with different input sizes.

The ConditionalExample.java shows how Big O takes the maximum complexity - max(O(n), O(1)) = O(n).

NestedLoopExample.java demonstrates O(n*m) complexity for nested loops."

## Running the Main Lab Files

"Now let's run the four main files you mentioned.

First, HelloWorld.java - the classic first program:

```bash
javac HelloWorld.java
java HelloWorld
```

Simple output: 'Hello, World!'

Next, ConstantTime.java - demonstrates O(1) complexity. It accesses an array element by index, which takes the same time regardless of array size.

Run it and note the time taken.

LinearTime.java - O(n) complexity. It sums all elements in an array with a loop. Time grows linearly with input size.

Try doubling the array size and see how the time changes.

QuadraticTime.java - O(n²) complexity. Nested loops that perform operations for each pair of elements. This gets slow very quickly - for n=5 it's 25 operations, for n=10 it's 100.

Keep the array small here!"

## Directing to Practice

"Finally, let's look at the practice folder. There's SumExample.java which compares three different ways to compute the sum of numbers from 1 to n:

1. Loop method - O(n) time, O(1) space
2. Recursive method - O(n) time, O(n) space
3. Formula method - O(1) time, O(1) space

Run this with a large n (like 100,000) and compare the execution times. The formula method should be fastest for large inputs.

Questions to think about:
- Which method has the best time complexity?
- Which uses the most space?
- For small n vs large n, which would you choose?

This wraps up our introduction. You now have your repository set up, understand basic Java concepts, and have run examples of different time complexities. For homework, work through the practice examples and answer the questions in the code comments. See you next time!"