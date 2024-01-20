# Custom Linux Terminal

A basic Linux terminal implemented in C, showcasing command execution, pipes, and I/O redirection. Utilizes fork(), execvp(), and tokenization for command handling, offering insights into system calls and Linux processes.

## Tech Stack

- <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a>
- <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a>

## How to Use

1. Compile the program using `g++ filename.cpp`.
2. Run the executable with `./a.out`.
3. Enter Linux commands with optional pipes and I/O redirection.

Feel free to explore and experiment with different commands!

## Code Snippet

```cpp
// Relevant code snippet showcasing tokenization and command execution.
int cpid = fork();
if (cpid == 0) {
    // Child process
    if (!checknormal(arr)) {
        // Handle pipes and I/O redirection
        // ...
    } else {
        previous(arr);
    }
    return 0;
} else if (cpid > 0) {
    wait(NULL);
    // _exit(0);
}
