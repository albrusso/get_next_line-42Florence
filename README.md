# get_next_line [42Cursus]

## Overview

**get_next_line** is a function that reads a line from a file descriptor and returns it as a string. This project is part of the 42 curriculum and focuses on efficient file handling and memory management in C.

## Features

- Reads a line from a specified file descriptor.
- Handles multiple file descriptors simultaneously.
- Efficiently manages memory for large files.
- Written in **C** and adheres to the 42 coding standards.

## How to Use

To use **get_next_line** in your project:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/get_next_line.git

2. Compile the library:
   ```bash
   make

3. Include the header in your code:
   ```bash
   #include "get_next_line.h"

4. Call the function to read a line:
   ```bash
   char *line;
   int fd = open("file.txt", O_RDONLY);
   while (get_next_line(fd, &line) > 0)
   {
    printf("%s\n", line);
    free(line);
   }
   close(fd);

## License
This project is for educational purposes as part of the 42Cursus and adheres to the rules of the 42 school. Feel free to review and adapt the code, but do not copy it directly for personal submissions.
