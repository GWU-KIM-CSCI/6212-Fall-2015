# Bonus Project

## Description

You are to impliment the Dijkstra's Shortest Path algorithm. Your program
will read in a matrix representation of a directed graph from a file and output
the shortest path distance to standard out using the Dijkstra's Algorithm.

You may use any open source programming language that you are most
comfortable with. Please do not use any language where the compiler and
runtime is not freely available.

## Specification

1. Your program will come with a README.txt file detailing the steps to
compile and execute your program.
2. Your program will be a command line application that takes a single
argument.
    - The single argument will be the name of the file that contains the
      matrix representation of a directed graph
    - The input file will be a n by n matrix where the row represents source vertex
      and column represents destination vertex.
    - The last line of the file will indicate the source vertex.
    - See example input file below.
    - If the specified file does not exist, your program should print an
      error message and exit gracefully.
    - You may assume that all the numbers will be greater than 0.
    - You may safely assume that the file, if exists, is in valid format.
3. Your may chose whatever data structure you see fit for this project.
4. Your program will execute the Dijkstra's Algorithm to calculate the shortest path.
5. Your program will output the array to STDOUT, where single
element in the array is in its own line. In other words, every output of
the array element will be followed by a new line character.
    - ith line will represent the shortest distance from source vertex to ith vertex.
    - See example output.
6. Once output has been produced, your program will exit gracefully.
7. Your program's executable should be named `dijkstra`.


## Sample Execution

The below input file represents the following graph:

<img src="https://i.imgur.com/ppEIwP7.png" />

### Mac or Linux

    $ cat input.txt 
    0 5 1 0
    0 0 0 10
    0 0 0 4
    3 0 0 0
    1
    $ ./dijkstra input.txt
    0
    5
    1
    5
    $ 

### Windows

    C:\> cat input.txt
    0 5 1 0
    0 0 0 10
    0 0 0 4
    3 0 0 0
    1
    C:\> quicksort.exe input.txt
    0
    5
    1
    5
    C:\>

## Submission

1. Your submission will be a ZIP file with the following contents:
    - README.txt file detailing how to compile and execute your code
    - Your source code
2. The name of your zip file will be `[YOUR_LAST_NAME]-project1.zip`.
2. DO NOT INCLUDE ANY BINARY FILES IN THE SUBMISSION! DO NOT INCLUDE `.o`,
`.pyc`, `.class`, or ANY OTHER INTERMEDIARY FILES! INCLUSION OF BINARY
FILES WILL MEAN AUTOMATIC ZERO FOR YOUR GRADE.
3. Further details of where to submit the zip file will be sent out before
the due date.

## Bonus Points

The fastest implimentation of the algorithm will receive extra bonus points.

## Due Date

The project will be due on 11:59PM, day of the final.





