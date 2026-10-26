*This project has been created as part of the 42 curriculum by rarayano.*

## Description
The **get_next_line** project is a fundamental milestone in the 42 curriculum. The goal is to write a function that returns a line read from a file descriptor, ending with a newline character (`\n`) or EOF (End Of File).

### Key Features
* **Buffer Management:** The function uses a defined `BUFFER_SIZE` to read chunks of data, ensuring memory efficiency.
* **Static Variables:** It utilizes a static variable to maintain state between function calls, allowing it to "remember" any leftover data from the previous read.
* **File Descriptor Support:** It handles reading from multiple file descriptors (if the bonus is implemented) or standard input.

The challenge lies in managing memory allocation carefully to prevent leaks and handling the edge cases of varying buffer sizes and line lengths.

## Instructions
Create a main function inside get_nextline.c or create a seperate file.
compile all of them using command bellow

```bash
cc -W -W -W *.c 
```
to compile with buffer modification use command bellow
```bash
cc -W -W -W -D BUFFER_SIZE=number_of_your_choice *.c 
```

## Resources


### AI Usage Disclosure
Artificial Intelligence (claude sonnet 4.5 and gemeni) was used as a pedagogical tool during the development of this project for the following tasks:
* **Concept Clarification:** Explaining the technical behavior and memory persistence of `static` functions and variables within the C scope.
* **System Call Mechanics:** Understanding the specific parameters and return values of `read()`, `open()`, and `close()`, particularly regarding the `O_RDONLY` flag.
