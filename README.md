# Simple Shell project

## Description
This project is a simple UNIX command line interpreter, also known as a shell. The shell provides a command-line interface for users to interact with the operating system. It reads commands from the user, executes them, and displays the output.

### Features
- Display a prompt and wait for the user to enter a command. The prompt is displayed again after executing each command.
- Accept command lines that consist of a single word. No arguments will be passed to programs.
- Handle errors gracefully. If an executable cannot be found, an error message is displayed, and the prompt is shown again.
- Support for interactive and non-interactive modes.
- Support for command lines with arguments.
- Handle the "end of file" condition (Ctrl+D).
- Implement built-in commands such as exit and env.
- Handle the PATH environment variable to search for executables in the system directories.
- Implement the cd command to change the current working directory.
- Implement the setenv and unsetenv commands to modify or remove environment variables.
- Support for command separators (;) and logical operators (&& and ||)

### Usage
To compile the shell, use the following command:
```
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```
To run the shell in interactive mode, execute the compiled binary:
```
./hsh
```

The shell will display a prompt where you can enter commands. The prompt will be shown again after executing each command.

To run the shell in non-interactive mode, you can pipe commands into it.
For Example:
```
echo "/bin/ls" | ./hsh
```

Interactive mode:
```
$ ./hsh
($) /bin/ls
file1 file2 file3
($) exit
$
```

Non-interactive mode:
```
$ echo "/bin/ls" | ./hsh
file1 file2 file3
$
```
### Files Description

## Authors
- Ataboh Hamza
- Youseff R.R
