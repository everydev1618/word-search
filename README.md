A word search puzzle presents a grid of seemingly random letters and a list of
words. The goal of the puzzle is to find and mark all the words from the list
hidden within the grid, searching along straight lines (horizontal, vertical and
diagonal).

The goal for this hack night is to write a Ruby program that generates word
search puzzles, given a list of words and the desired width and height for the
puzzle. A call to the script will look like this:

```
genpuzzle.rb words.txt 6x8
```

The first argument is the list of words, one word per line in a text file. The
second argument is the dimensions of the puzzle, width by height.

Your program should output two files. The first file, search.txt, should contain
the puzzle itself. All characters should be separated by spaces to allow the
puzzle solver room to mark found words. As an example, here is a 6x8 puzzle
containing the words from “zero” to “nine”.

```
e a e g g w
e e n i n t
r n o h h f
h q e g i r
t z i v u q
o e e o e l
w r f g e s
t o u s i x
```

The second file, solution.txt, should contain the same puzzle with the answers
marked, like this:

```
e . e . . .
| |
e e-n-i-n t
| | /
r n o . h f
| \ / /
h . e g i r
| X / /
t z i v u .
|/ / X
o e e o e .
| | / \
w r f . . s
| |
t o . s-i-x
```


Adapted from Ruby Quiz #159, please do not search for solutions to the problem.

