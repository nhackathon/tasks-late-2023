# Nokia Hackathon (late 2023)

**General Information:**

Every task has it's own "workspace", it's own task folder, please stay in these folders while working on the solutions.
You can put any necessary requirments to the _requirments.txt_ it will be installed automatically if it is not empty.
Points will firstly based on correction and completion of the tasks, then implementation, functionality, code prettyness and readibility will be taken to account as well. You can work in more than one file and use abstraction too.

Folder structure:

- _input.txt_
- _main.py_, which is the the main entry point for the automatized test runner, please do not remove this file, it must not have required parameters and always have to create an _output.txt_ file which can be evaluated afterwards the _main.py_ is run

**Disclaimer:**

- The run time of your solutions must not exceed 10 seconds. When checking the solutions if a code is running past this 10 seconds it will be automatically shut down
- Make sure you do not modify the _.github_ folder
- Make sure you do not modify or delete the _main.py_ file

## 1. Palindrome Checker

**Task Folder:**
palindrome_checker

**Description:**

Your task is to develop a program that checks if a given string is a palindrome while taking into account alphanumeric characters and ignoring upper and lower case. Additionally, the program should count the number of unique characters in the string.

**Input:**

The input is a list of string that may contain letters, digits, punctuation, symbols, and spaces. The string can be a combination of uppercase and lowercase characters.

**Output:**

The program should provide the following:

1. Whether the input string is a palindrome.
2. The count of unique alphanumeric characters in the string.

**Example:**

_input.txt_

```
racecar
hello
1232112321
worldmadamhelloworld
1234567890
```

_output.txt_

```
YES, 4
NO, -1
YES, 3
NO, -1
NO, -1
```

## 2. Matrix Operations

**Task Folder:**
matrix_operations

**Description:**

Your task is to develop a program that can perform a set of matrix operations on matrices of different sizes. These operations include matrix addition and multiplication. The program should be versatile enough to handle matrices with various dimensions.

**Input Format:**

The input consists a list of matrices with its own keys sizes and values, then a list of operations.

**Output:**

The program should produce the result of the specified matrix operation.

**Example:**
_input.txt_

```
matrices

A
2 1
3 4

B
1 0
5 6

operations

A + B
A * B
```

_output.txt_

```
A + B
3 1
8 10

A * B
7 6
23 24
```

**Note:**

Ensure that the program handles matrices of different sizes correctly and performs the operations accurately.

## 3. Maze Solver

**Task Folder:**
maze_solver

**Description:**

Your task is to develop a program that can navigate through a 2D maze grid, starting from a designated point and reaching a goal while avoiding obstacles. The maze grid consists of open pathways, walls, a starting point, and a goal. The program should find the shortest and quickest path from the starting point to the goal.

**Input Format:**

The input is a 2D grid that represents the maze. It consists of characters to denote the maze elements. Common characters include:

- 'S' for the starting point
- 'G' for the goal
- '.' for open pathways
- '#' for walls or obstacles

**Output:**

The program should provide the path, from the starting point to the goal. This path should be represented by the movement directions like: 'U' for up, 'D' for down, 'L' for left, 'R' for right.

**Example:**

_input.txt_

```
A
# # # # # # #
# S . . . . #
# # . # # . #
# . . # . . #
# . . . # # #
# . # G . . #
# # # # # # #
```

In this example, the maze is represented by a 2D grid. 'S' marks the starting point, 'G' is the goal, '.' represents open pathways, and '#' indicates walls or obstacles.

_output.txt_

```
A
R D D D R D
```

The program outputs the path as a sequence of movements: right (R), down (D), left (L), and up (U).

**Note:**

Ensure that the program correctly navigates through the maze, avoiding obstacles and finding a path to the goal.

## 4. Dobble Generator

**Task Folder:**
dobble_generator

**Description:**

Your task is to write a generator which can generate a "Dobble deck". The game "Dobble" consists of a deck of cards, each containing `n` different symbols. When you choose any two cards from the deck, it is guaranteed that they will have one and only one symbol in common.

**Input Format:**

Every line of the input file contains the number of symbols on each cards.

**Output:**

Should contain the number of symbols (as a reference) and below the generated output, similarly like in the example. If the provided number of symbols is not valid instead of the generated list you should write `invalid` after the number of symbols (reference) like this:

```
n
invalid
```

**Example:**
_input.txt_

```
3
4
```

_output.txt_

```
3
1 - [1, 2, 3]
2 - [1, 4, 5]
3 - [1, 6, 7]
4 - [2, 4, 6]
5 - [2, 5, 7]
6 - [3, 4, 7]
7 - [3, 5, 6]

4
1 - [1, 2, 3, 4]
2 - [1, 5, 6, 7]
3 - [1, 8, 9, 10]
4 - [1, 11, 12, 13]
5 - [2, 5, 8, 11]
6 - [2, 6, 9, 12]
7 - [2, 7, 10, 13]
8 - [3, 5, 9, 13]
9 - [3, 6, 10, 11]
10 - [3, 7, 8, 12]
11 - [4, 5, 10, 12]
12 - [4, 6, 8, 13]
13 - [4, 7, 9, 11]
```

**Constraints:**

- Its essential to note that the same value cannot be a common element in all pairs of cards.

**Note:**

For more information about the Dobble game, you can refer to the official game rules.
