# Command Line Argument Handling in C

## Description
This project contains a C program that demonstrates basic command line argument handling. The program checks the number of arguments provided and prints appropriate messages based on the count.

### Key Features
- **Command Line Arguments**: Parsing and using command line arguments in the C program.

### Code Snippet
```c
#include <stdio.h>

int main(int argc, char **argv)
{
    if (argc < 2) {
        printf("Ha olvidado su nombre\n");
    } else if (argc > 3) {
        printf("Son demasiados parametros\n");
    } else {
        printf("Hola %s %s\n", argv[1], argv[2]);
    }
    return 0;
}
```

This code checks the number of command line arguments passed and prints appropriate messages based on the count.

## How to Use

1.  **Compilation**: The C file can be compiled using a C compiler such as `gcc`.
    
```bash
	gcc A1P3.c -o A1P3` 
```
    
2.  **Execution**: Run the compiled program with the required arguments to see the output.
    
```bash
	./A1P3 arg1 arg2`
```