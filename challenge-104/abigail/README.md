# Solution by Abigail
## [FUSC Sequence](https://perlweeklychallenge.org/blog/perl-weekly-challenge-104/#TASK1)

Write a script to generate first 50 members of FUSC Sequence. Please
refer to [OEIS](https://oeis.org/A002487) for more information._

The sequence defined as below:

~~~~
fusc(0) = 0
fusc(1) = 1
for n > 1:
when n is even: fusc(n) = fusc(n / 2),
when n is odd: fusc(n) = fusc((n-1)/2) + fusc((n+1)/2)
~~~~

### Notes
This challenge is beyond simple. Since we're asked to generate a
fixed number of numbers, we don't need do any calculations, or
even handle a single if statement. A single print statement is enough.
This makes it easy to create solutions in many languages. In some,
we also have an alternative solution, where we actually calculate
the solution.

### Solutions
* AWK
    * [Simple](awk/ch-1.awk)
    * [Calculated](awk/ch-1a.awk)
* Bash
    * [Simple](bash/ch-1.sh)
    * [Calculated](bash/ch-1a.sh)
* [Basic](basic/ch-1.bas)
* [Befunge-93](befunge-93/ch-1.bf93)
* [bc](bc/ch-1.bc)
* C
    * [Simple](c/ch-1.c)
    * [Calculated](c/ch-1a.c)
* [Cobol](cobol/ch-1.cb)
* [C-shell](csh/ch-1.csh)
* [Erlang](erlang/ch-1.erl)
* [Forth](forth/ch-1.fs)
* [Fortran](fortran/ch-1.f90)
* [Go](go/ch-1.go)
* [Java](java/ch-1.java)
* Lua
    * [Simple](lua/ch-1.lua)
    * [Calculated](lua/ch-1a.lua)
* [m4](m4/ch-1.m4)
* Node.js
    * [Simple](node/ch-1.js)
    * [Calculated](node/ch-1a.js)
* [OCaml](ocaml/ch-1.ml)
* [Pascal](perl/ch-1.p)
* Perl
    * [Simple](perl/ch-1.pl)
    * [Calculated](perl/ch-1a.pl)
* [PHP](php/ch-1.php)
* Python
    * [Simple](python/ch-1.py)
    * [Calculated](python/ch-1a.py)
* [R](r/ch-1.r)
* [Rexx](rexx/ch-1.rexx)
* Ruby
    * [Simple](ruby/ch-1.rb)
    * [Calculated](ruby/ch-1a.rb)
* [Scheme](scheme/ch-1.scm)
* [sed](sed/ch-1.sed)
* [SQL](sql/ch-1.sql)
* [Tcl](tcl/ch-1.tcl)

### Blog
[Perl Weekly Challenge 104: FUSC Sequence](https://wp.me/pcxd30-vx)

## [NIM Game](https://perlweeklychallenge.org/blog/perl-weekly-challenge-104/#TASK2)
Write a script to simulate the NIM Game.

It is played between 2 players. For the purpose of this task, let
assume you play against the machine.

There are 3 simple rules to follow:
~~~~
a) You have 12 tokens
b) Each player can pick 1, 2 or 3 tokens at a time
c) The player who picks the last token wins the game
~~~~

### Notes
This is *not* the well known NIM game. In the NIM game, you have multiple sets
of tokens, and on each turn, a player picks a set, and removes any
non-zero number of of tokens from the set. Typically, the player
picking the last token loses.

The game as given is sometimes also known as the NIM game, but it better
known as the subtraction game. With the given parameters and perfect
play, the second player always wins on the third move.

In each of the three moves, we ask the player how many tokens she wants
take, showing the current number of tokens. We keep asking the question
until the player gives a valid answer (1, 2, or 3). The computer takes
3, 2, or 1 tokens, and we subtract 4 from the number of tokens.

After the third move, we print that the computer has won.


### Solutions
* [AWK](awk/ch-2.awk)
* [Bash](bash/ch-2.sh)
* [BASIC](basic/ch-2.bas)
* [Befunge-93](befunge/ch-2.bf93)
* [C](c/ch-2.c)
* [Lua](lua/ch-2.lua)
* [Pascal](pascal/ch-2.p)
* [Perl](perl/ch-2.pl)
* [Python](python/ch-2.py)
* [R](r/ch-2.r)
* [Ruby](ruby/ch-2.rb)
* [Scheme](scheme/ch-2.scm)

### Blog
[Perl Weekly Challenge 104: NIM Game](https://wp.me/pcxd30-w5)
