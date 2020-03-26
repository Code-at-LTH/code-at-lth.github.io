---
layout: panel-with-sidebar
title: EDAF05 - Exercises
id: algodat
---

# EDAF05 - Exercises
## Algoritmer datastrukturer och komplexitet


### How these exercises work

#### Standard in and Standard out in a terminal

The labs in this course are on the format that you should write a program that solves an algorithmic problem, by reading from standard in and writing a correct answer to standard output.

#### Environment assumptions
We assume that you use a terminal with a `bash`-like shell. This is the standard shell for most Linux distributions, and macOS. For windows you can download [GitBash](https://liveoncode.com/installing-gitbash-on-windows-10/).

Let's say you have written some code in a file `Solver.java`, that has a main-function, and you have compiled it with `javac Solver.java`, creating a file `Solver.class`.

There exists an input file that is called `example.in`, and the correct output is in `example.ans`. Then your program will be checked by running `java Solver < example.in > example.out` in your terminal.
This means that the content of `example.in` is sent to your program Solver on `stdin`, and the output is saved in the file `example.out`. Then we can check if your program produced the correct output by using the program `diff`. Running `diff example.out example.ans` will print nothing if the content is the same (your program worked as excepted) and will print the difference between the files if they differ.


#### Good News
There exists a website called Kattis ([open.kattis.com](https://open.kattis.com)), which has a lot of different algorithmic problems, and uses the same execution-model that we do.

The problems on Kattis can be used as exercises for the course. 

If you want to know how to read from `stdin` and print to `stdout` in your preferred programming language you can check out their [help page](https://open.kattis.com/help). There is also som links to for example how judging is done explaining what results you can get when you submit your code:

- Accepted - Your code was correct and you get points
- Wrong Answer - Your code produced an incorrect answer on at least one of the test cases
- Time Limit Exceeded - Your code didn't finish in time
- Run Time Error - Your code crashed while running one of the testcases
- Compile Error - Your code didn't compile

To use Kattis you need an account. You can either log in [via Google/Facebook/LinkedIn](https://open.kattis.com/login), or [create one](https://open.kattis.com/register).

If you have problems solving some of the exercises you can [join our discord](https://discord.gg/NpnXYj4) and ask for help in a dedicated channel for the course!


### Exercises

#### 1. Introduction

- [Hello World!](https://open.kattis.com/problems/hello)
- [Soylent](https://open.kattis.com/problems/soylent)
- [License to Launch](https://open.kattis.com/problems/licensetolaunch)
- [Number Fun](https://open.kattis.com/problems/numberfun)
- [Backspace](https://open.kattis.com/problems/backspace)
- [Baby Bites](https://open.kattis.com/problems/babybites)
- [Drinking Song](https://open.kattis.com/problems/drinkingsong)
- [Thank God it's Friday](https://open.kattis.com/problems/tgif)
- [Opening Ceremony](https://open.kattis.com/problems/ceremony)
- [Eeny Meeny](https://open.kattis.com/problems/eenymeeny)
- [Espresso Bucks](https://open.kattis.com/problems/espressobucks)
