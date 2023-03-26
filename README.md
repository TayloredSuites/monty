# Stacks, Queues && LIFO and FIFO

- ## About the Repository

This repo contains the basics of stacks, queues, LIFO, FIFO and the bizzare bytecode language Monty. At the end of it, one should know what the difference between a stack and a queue is and when to use each. It will touch on the common implementations, and other such things. Want to know what that really means? Take a step into the project.

#### The Monty language
Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

Monty byte code files

Files containing Monty byte codes usually have the .m extension. Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument:
```c

eagle@ubuntu:~/monty$ cat -e bytecodes/000.m
push 0$
push 1$
push 2$
  push 3$
                   pall    $
push 4$
    push 5    $
      push    6        $
pall$
eagle@ubuntu:~/monty$

```
Monty byte code files can contain blank lines (empty or made of spaces only, and any additional text after the opcode or its required argument is not taken into account:
```m

eagle@ubuntu:~/monty$ cat -e bytecodes/001.m
push 0 Push 0 onto the stack$
push 1 Push 1 onto the stack$
$
push 2$
  push 3$
                   pall    $
$
$
                           $
push 4$
$
    push 5    $
      push    6        $
$
pall This is the end of our program. Monty is awesome!$
eagle@ubuntu:~/monty$

```

- ## Required Software / Hardware

-  Ubuntu 20.04 LTS using `gcc`, using the options `gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty`
-  [Betty linter](https://github.com/holbertonschool/Betty/blob/master/betty-style.pl)
-  C standard library
-  No more than 5 functions per file

![Libraries courtesy Sitesbay.com](https://www.sitesbay.com/cprogramming/images/header-files-in-c.png)

- ## Findings / Observations

These are yet to be discovered. You can always feel free to tell me in an issue if you like.

- ## Contributions

I guess you know a better way to do this or would like to collaborate, I am here.

:smile:
