# C Fundamentals

## General

- Hello World
  ```c
  printf("hello, world\n");
  ```

- Store integer in variable
  ```c
  int counter = 0;
  ```
  
- Increment by 1
  ```c
  counter = counter + 1;
  ```
  ```c
  counter += 1;
  ```
  ```c
  counter++;
  ```
  
- Conditional Printing
  ```c
  if (x < y)
  {
    printf("x is less than y\n");
  }
  ```
  ```c
  if (x < y)
  {
    printf("x is less than y\n");
  }
  else
  {
    printf("x is not less than y\n");
  }
  ```
  
- Flow Control
  ```c
  while (true)
  {
    printf("hello, world\n");
  }
  ```
  ```c
  for (int i = 0; i < 50l i++)
  {
    printf("hello, world\n");
  }
  ```

## C Command Line Interface

- **clang**
  - The CLI for C
  - Initiate with ```clang``` keyword

- C files must be converted to machine code before being executed
  - In the directory of the file, run the following
    ```clang <fileName>```
  - This will compile the source code into binary and store it in a file called ```a.out``` in the same directory
  - Running ```./a.out``` will execute the binary file
  
- Creating a named output file
  - Syntax:  ```clang -o <outputFileName> <inputFileName>```
  - e.g.  ```clang -o hello hello.c```
    - Produces ```o.out```
  
