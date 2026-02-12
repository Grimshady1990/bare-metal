# Week 0

In this introductory lesson we learnt about binary code, how they can be
expanded in bytes.

How bytes can be interpreted in many different ways to create different
outputs

We also looked at the importance of pseudocode and its place in being able 
to translate our ideas into computer readable language.

## Binary / Bits

Binary is system of switches that are either on or off represented as either
1s or 0s, These ones and zeros can be combined to create patterns that can represent
either a letter, number, or a colour amongst many other things.

## Bytes

Combining 8 of these switches or bits creates something called a byte and the bits
value doubles in size numerically from right to left which are called weights, a byte looks something
like this.

128 64 32 16 8 4 2 1

This can be used to create 256 different values by adding the numbers together
you would think there was only 255 values but we must remember that zero is
also a value.

Weights:128 64 32 16 8 4 2 1
                             =0
Bits:    0  0  0  0  0 0 0 0

Lets say we wanted output the value of 215, we would turn on the following
switches or use the following bits.

Weights: 128 64 32 16 8 4 2 1
                             = 215
Bits:     1  1  0  1  0 1 1 1

These bytes can represent multiple values where the below example represents 65
numerically it can also represent the character A, you can view the ASCII table 
that gives all the different values available for each byte.
https://www.ascii-code.com/

Weights: 128 64 32 16 8 4 2 1
                             = 65 and/or A
 Bits:    0  1  0  0  0 0 0 1

There are many different ways bytes can be interpreted depending on how the
individual program has been designed to interpreted the bytes, for example
RGB uses the colours red, green and blue at different intensity to create a
huge array of different colours.

Red,green and blue are all given there own byte value between 0-255
then they are combined to create one of 16.7 million different colours and
shades or to be more precise.

256 * 256 * 256 = 16,777,216 different colours

This truly shows how one bit can dramatically become so much more.

We also discussed pseudocode which is a way to walk step by step
throw a program or a process using natural language. Syntax can become
a little confusing pseudocode allows us to plan what we want our program
to do before we start writing code for example

```
Human is asked for thier name

If human submits name

Output "Hello, name"

```
This is a very simple example is good enough to explain how pseudocode works.

Pseudocode is a extremely powerful tool and must be fully grasped before being
able to convert our pseudocode into actual computer readable code.

This is why our first project in the CS50 is to create a program using and
piece of software called Scratch.

Scratch was created by MIT and uses a module based system that uses
human readable descriptors for things like conditions, loops and functions
in the form of blocks you can click together and build simple programs.

In my next session I will be rolling up my sleeves and diving into this
project and hopefully create something fun.
