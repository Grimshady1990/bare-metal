# First C Observation

My first attempt at a simple c program created some errors when compiled
surprisingly they are quite verbose and easy to understand the first was
a unknown type name where i accidentally typed init instead of int, I'm not
sure what int means yet in other languages it means integer but that doesn't
seem correct in this context.

Next I forgot to put a semi-colon before the return the output was very clear
helping me easily fix it.

And the final error was not spotted by the compiler as it was a logical error
resulting in the output "hello/n". There's no mystery to what I did wrong there

The compiler command is gcc not sure how this works but what I do know it
takes a input file (hello.c) and a output file (-o hello).
I can then run this output file to run the program (./hello).

Below is the entire journey from the terminal

```
…/labs/hello-c main  ? ❯ gcc hello.c -o hello
hello.c:3:1: error: unknown type name ‘init’; did you mean ‘int’?
    3 | init main(void) {
      | ^~~~
      | int
hello.c: In function ‘main’:
hello.c:4:20: error: expected ‘;’ before ‘return’
    4 |   printf("hello/n")
      |                    ^
      |                    ;
    5 |   return 0;
      |   ~~~~~~

…/labs/hello-c main  ? ✗ nvim hello.c

…/labs/hello-c main  ? ❯ gcc hello.c -o hello
hello.c:3:1: error: unknown type name ‘init’; did you mean ‘int’?
    3 | init main(void) {
      | ^~~~
      | int

…/labs/hello-c main  ? ✗ nvim hello.c

…/labs/hello-c main  ? ❯ nvim hello.c

…/labs/hello-c main  ? ❯ gcc hello.c -o hello

…/labs/hello-c main  ? ❯ ./hello
hello/n
…/labs/hello-c main  ? ❯ nvim hello.c

…/labs/hello-c main  ? ❯ gcc hello.c -o hello

…/labs/hello-c main  ? ❯ ./hello
hello

…/labs/hello-c main  ? ❯ ls
Permissions Size User Date Modified Name
.rwxr-xr-x   16k grim 10 Feb 04:35  󰡯 hello
.rw-r--r--    72 grim 10 Feb 04:35   hello.c
```

### Open questions
- What does `int main(void)` return to the operating system?
- How does `gcc` transform source code into an executable?
- What exactly does `#include <stdio.h>` do?
