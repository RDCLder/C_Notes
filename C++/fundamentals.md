# C++ Fundamentals

## General

- Hello World!
  ```cpp
  #include <iostream>

  int main()
  {
    std::cout << "Hello World!";
    return 0;
  }
  ```
  - Line 1 has a preprocessor directive
  - Line 3 has the main method
    - Entry point for the application when executing
    - ```int``` indicates return type of integer
    - Return value of 0 indicates code executed successfully (generally true for most functions)
  - Line 5 uses the ```cout``` (pronounced "see-out") method from the ```std``` namespace
    - Sends ```"Hello World!"``` string as output to console
    - ```::``` are used to indicate that a proceeding method belongs to the preceding namespace
  - Line 6 returns value of 0 to indicate successful function execution
    - Other numbers would indicate that something went wrong

## Compilation

- Portability
  - Capacity of compiling code across different compilers or platforms without major changes
    - Platforms can be:
      - Computer hardware
      - Operating systems
      - CPU architectures
      - Device form factors
    - Compilation is the process of translating code into machine code that is executable by computers

- Cross-platform portabiliy is desirable to save time
  - Traditionally, cross-platform code had to be written in the native language for the platform which is time-consuming
  
- Compilation Process
  - Preprocessor
    - Takes C++ source code and evaluates preprocessor directives (e.g. libraries to include)
    - Produces preprocessed source file
  - Compiler
    - Takes preprocessed source code, compiles into object files.
    - Checks that your code conforms to all syntax and semantic rules (e.g. no type errors)
    - Accepts promises from the code about things defined in other source files
  - Linker
    - Takes object files, links them into an executable program
    - Ensures that all of the promises to the compiler are kept
    - e.g. If your program uses the ```cout``` function found in the iostream set of files, the linker makes sure that the code for that function is included in the ```.exe``` file
